2024-07-3119:36
Status: #Incomplete 

Binary search is a searching algorithm for **sorted** data that divides an array by half by checking whether the target is within the range. 

![[binary-and-linear-search-animations.gif]]

## Sample C++ Code 
``` c
int start = 0;
int end = nums.size();
int mid;  

if(target>nums[end-1]){
	return end;
}
//cout<<mid;
while(start<=end){
	mid = (end+start)/2;
	if(nums[mid]==target){
		//cout<<mid;  
		return mid;
	}
	if(nums[mid]<target){
		start = mid + 1;
		//cout<<mid<<endl;
	}
	else{
		end = mid -1;
		//cout<<mid<<endl;
		}
}
cout<<start<<", "<<end;
return start;
```

# Source(s)
https://www.youtube.com/watch?v=vohuRrwbTT4
https://www.youtube.com/watch?v=tgVSkMA8joQ