2024-07-3120:05
Status: #Pseudo #CS50 

The internet is a connection of networks physically connected through cables and wires. A router being a node in that network. Hardware knowing what router information it has.

TCP (Transmitting control protocol) Is the fragmentation splits up a file’s information (in order to reassemble) and if there is any information missing it will notice it. It also guarantees delivery. Marking the source address and TCP specifies what kind of service it is sending. Port 80= Website, Port 443 = Encrypted Website, Port 25 = SMTP = email, Port 53 = DNS

IP makes the sources address and recipient address. IPs #.#.#.# = 32bit, now 128bit → IPv6 = 8 clusters of HEX Omitting of 126 bit IP addresses with large chunks of zeroes can be written in the following format. 2001:4567:9807:0:0:0:0:9876 = 2001:4567:9807::9876

IP’s (Internet Protocol) public router address is connected to other routers locally. The central point of their connection is connected to a larger framework that connects networks on a global scale. It has multiple path in case traffic on a specific path is too jammed

DHCP (Dynamic host configuration protocol) assigns IP addresses

Domain name system (DNS) connects IP addresses to (Fully qualified) domain names. Large DNS servers (like Google’s) collect smaller sets of DNS information and pool them together, updating them frequently.

Access points: The IP address is assigned to a router, whose job is to act as a traffic cop that allows data requests from all of the devices on your local network (home/business etc.) to be processed through the same IP address

HTTP Standardizes how the web (built on top of the internet) interacts with the user. It is an application layer protocol (other examples include: FTP, SMTO, DDS, RDP, XMPP etc.) which specifically dictates the format by which clients request web pages from a server and the format via which servers return information to clients.

http(s)://www.example.com/folder/file/html www.=subdomain .com=commercial http(s)


```html
//GET: Requests information from the
server and the client gets response
GET/HTTP/1.1
Host: www.example.com
...

//Response 
HTTP/1.1 200 OK 
Content-Type: text/html
... 
```

![[internet-diagram.gif]]


```html
Seeing these messages using the curl function 
200 0K [success]
301 Moved Permanently [redirection] (safetyschool.org) (harvardsucks.org) 
302 Found [redirection temporarily]
304 Not Modified 
307 Temporary Redirect 
401 Unauthorized [not logged in]
403 Forbidden [not intended for clients to access]
404 Not found [doesn't exist on the server]
418 I'm a Teapot (<https://www.google.com/teapot>) 
* 500 Internal Server Error [server end error] 
503 Service Unavailable [timeout]
... 
