#### Path Accumulators 
When trying to keep track of a node from a root (or other node), keeping track of the paths taken prevents the same path being taken (looping). Think of these as bungee cords that come from a root and try to find a route. 
- Original recursion - current branch of the data is in the past 
- Prevents cycles (A leads to B and B leads to A)
```(define (distance-from m start end)
    (local [(define R (sqrt (length m)))	  

          ;; trivial:   
          ;; reduction: 
          ;; argument:
           
          (define (fn-for-p p path passed-start?)
            (cond [(equal? p end)   (add1 (position-of start path))]
                  ;if end is reached, then find the distance between start/path
                  ;[(solved? p)      false]
                  [(member? p path) false] ;termination condition/result
                  [else
                   (if (equal? p start)
                       (fn-for-lop (next-ps p) (cons p path) true)
                       ; if the starting node has been found, pass true as acc 
                       (fn-for-lop (next-ps p) (cons p path) passed-start?))]))
                       ; if the starting node is yet to be found pass acc   
          (define (fn-for-lop lop path dist)
            (cond [(empty? lop) false]
                  [else
                   (local [(define try (fn-for-p (first lop) path dist))]
                     (if (not (false? try))
                         try
                         (fn-for-lop (rest lop) path dist)))]))

          ;; CONSTRAINT: p is in lop
          (define (position-of p lop)
            (cond [(empty? p) (error "p was not in lop")]
                  [else
                   (if (equal? p (first lop))
                       0
                       (add1 (position-of p (rest lop))))]))
       
       ... 
    
    (fn-for-p (make-pos 0 0) empty false)))
```
###### (Full Code)
```(define (distance-from m start end)
    (local [(define R (sqrt (length m)))	  

          ;; trivial:   
          ;; reduction: 
          ;; argument:
           
          (define (fn-for-p p path passed-start?)
            (cond [(equal? p end)   (add1 (position-of start path))]
                  ;if end is reached, then find the distance between start/path
                  ;[(solved? p)      false]
                  [(member? p path) false] ;termination condition/result
                  [else
                   (if (equal? p start)
                       (fn-for-lop (next-ps p) (cons p path) true)
                       ; if the starting node has been found, pass true as acc 
                       (fn-for-lop (next-ps p) (cons p path) passed-start?))]))
                       ; if the starting node is yet to be found pass acc   
          (define (fn-for-lop lop path dist)
            (cond [(empty? lop) false]
                  [else
                   (local [(define try (fn-for-p (first lop) path dist))]
                     (if (not (false? try))
                         try
                         (fn-for-lop (rest lop) path dist)))]))

          ;; CONSTRAINT: p is in lop
          (define (position-of p lop)
            (cond [(empty? p) (error "p was not in lop")]
                  [else
                   (if (equal? p (first lop))
                       0
                       (add1 (position-of p (rest lop))))]))
          
          ;; Pos -> Boolean          
          ;; produce true if pos is at the lower right
          (define (solved? p)
            (and (= (pos-x p) (sub1 R))
                 (= (pos-y p) (sub1 R))))


          ;; Pos -> (listof Pos)
          ;; produce next possible positions based on maze geometry
          (define (next-ps p)
            (local [(define x (pos-x p))
                    (define y (pos-y p))]
              (filter (lambda (p1)
                        (and (<= 0 (pos-x p1) (sub1 R))  ;legal x
                             (<= 0 (pos-y p1) (sub1 R))  ;legal y
                             (open? (maze-ref m p1))))   ;open?
                      (list (make-pos x (sub1 y))        ;up
                            (make-pos x (add1 y))        ;down
                            (make-pos (sub1 x) y)        ;left
                            (make-pos (add1 x) y)))))    ;right

          ;; Maze Pos -> Boolean
          ;; produce contents of maze at location p
          ;; assume p is within bounds of maze
          (define (maze-ref m p)
            (list-ref m (+ (pos-x p) (* R (pos-y p)))))]
    
    (fn-for-p (make-pos 0 0) empty false)))
```
#### Visited Accumulators
When trying to keep track of all the nodes that have been checked, visited prevents ... . This is similar to spray paint where if a node has already been "visited," the program proceeds to the next node. This prevents 
- Tail recursion - every node visited in the computation 
- Prevents cycles and joins (two paths to the same node)
```
(define (solvable-no-revisits? m)
  (local [(define R (sqrt (length m)))	  

          ;; trivial: ... 
          ;; reduction: ...
          ;; argument: .. 
          
          (define (fn-for-p p p-wl visited)
            (cond [(solved? p) true] ;is condition met? 
                  [(member? p visited) (fn-for-lop p-wl visited)]
                  ;if path has been visited, skip by "ignoring" current p by: 
                  ; 1. not adding p to visited accumulator
                  ; 2. not adding p's children to worklist accumulator 
                  [else
                   (fn-for-lop (append (next-ps p) p-wl) (cons p visited))]))

          (define (fn-for-lop p-wl visited)
            (cond [(empty? p-wl) false]
                  [else
                   (fn-for-p (first p-wl) (rest p-wl) visited)]))
          ; tail recursive to record all nodes visited. 
          
          ...1
    
    (fn-for-p (make-pos 0 0) empty empty)))
```
###### (Full code)
```(define (solvable-no-revisits? m)
  (local [(define R (sqrt (length m)))	  

          ;; trivial:   
          ;; reduction: 
          ;; argument:
          
          (define (fn-for-p p p-wl visited)
            (cond [(solved? p) true] ;is condition met? 
                  [(member? p visited) (fn-for-lop p-wl visited)]
                  ;if path has been visited, skip by "ignoring" current p by: 
                  ; 1. not adding p to visited accumulator
                  ; 2. not adding p's children to worklist accumulator 
                  [else
                   (fn-for-lop (append (next-ps p) p-wl) (cons p visited))]))

          (define (fn-for-lop p-wl visited)
            (cond [(empty? p-wl) false]
                  [else
                   (fn-for-p (first p-wl) (rest p-wl) visited)]))
          ; tail recursive to record all nodes visited. 
          
          
          ;; Pos -> Boolean          
          ;; produce true if pos is at the lower right
          (define (solved? p)
            (and (= (pos-x p) (sub1 R))
                 (= (pos-y p) (sub1 R))))


          ;; Pos -> (listof Pos)
          ;; produce next possible positions based on maze geometry
          (define (next-ps p)
            (local [(define x (pos-x p))
                    (define y (pos-y p))]
              (filter (lambda (p1)
                        (and (<= 0 (pos-x p1) (sub1 R))  ;legal x
                             (<= 0 (pos-y p1) (sub1 R))  ;legal y
                             (open? (maze-ref m p1))))   ;open?
                      (list (make-pos x (sub1 y))        ;up
                            (make-pos x (add1 y))        ;down
                            (make-pos (sub1 x) y)        ;left
                            (make-pos (add1 x) y)))))    ;right

          ;; Maze Pos -> Boolean
          ;; produce contents of maze at location p
          ;; assume p is within bounds of maze
          (define (maze-ref m p)
            (list-ref m (+ (pos-x p) (* R (pos-y p)))))]
    
    (fn-for-p (make-pos 0 0) empty empty)))
```
#### BFS vs. DFS 

![[Pasted image 20241202111145.png]]
![[Pasted image 20241202113129.png]]

![[Pasted image 20241202114625.png]]
![[Pasted image 20241202114710.png]]


![[Pasted image 20241203140442.png]]
Everything but big band, 
Unlikely for htdf module 1 problem (6 and on)


![[Pasted image 20241203141109.png]]![[Pasted image 20241203141212.png]]

![[Pasted image 20241203141256.png]]Problems that build off of PSET 9-11 
