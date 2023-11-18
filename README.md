# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by:BOOBESH PM
RegisterNumber: 212222233001
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if (array[i]==k):
            return i
    return -1
    
array = eval(input())
k = eval(input()) 
n=len(array)
array.sort()
result = linearSearch(array,n,k)
if (result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)


```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program for linear search method to match the item in a list
Developed by:BOOBESH PM
RegisterNumber: 212222233001
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if (array[i]==k):
            return i
    return -1
    
array = eval(input())
k = eval(input()) 
n=len(array)
array.sort()
result = linearSearch(array,n,k)
if (result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)


```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: your name BOOBESH PM
RegisterNumber: 212222233001
'''
def BinarySearch(arr, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if arr[mid]==k:
            return mid
        elif arr[mid]>k:
            return BinarySearch(arr,k,low,mid-1)
        else:
            return BinarySearch(arr,k,mid+1,high)
    else:
            return -1
    
arr = eval(input())
arr.sort()
k = eval(input())
result=BinarySearch(arr,k,0,len(arr)-1)
if(result==-1):
    print(arr)
    print("Element not found")
else:
    print(arr)
    print("Element found at index: ",result)
```
## Sample Input and Output
![image](https://github.com/Boobeshkrishna/Search-Algorithm/assets/141472052/614f1ef3-b48b-4a42-8b6e-ff432eb84b78)
![image](https://github.com/Boobeshkrishna/Search-Algorithm/assets/141472052/841739ce-96d3-4c8b-ad3e-f860a7e8cbba)
![image](https://github.com/Boobeshkrishna/Search-Algorithm/assets/141472052/2651dcd8-753c-47a3-afdf-e79145aeaf42)
![3b 1](https://github.com/Boobeshkrishna/Search-Algorithm/assets/141472052/f1adcbff-3767-4459-b11f-91c9fdef75a2)
![3b 2](https://github.com/Boobeshkrishna/Search-Algorithm/assets/141472052/d39243df-e4c2-4d89-aeff-ee4e26f5e30f)
![3b 3](https://github.com/Boobeshkrishna/Search-Algorithm/assets/141472052/97b1e48e-d108-46b2-9689-8e31f7507dbf)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.
