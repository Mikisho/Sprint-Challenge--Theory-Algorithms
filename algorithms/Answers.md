### Answers for Algorithms
  --------------------------------------------
  ********************************************
  ## Excercise I
a. O(n) # it is taking `n` iterations

b. O(logn) # in each iteration `i` is cut in half

c. O(sqrt(n)) # first loop takes Math.sqrt

d. O(nlogn) # here the inner loop is linear and the outer is logarithmic 

e. O(n<sup>3</sup>) # here we consider the outer loops since the inner most loop is constant

f. O(n) # the loop runs if `bunnies === 0`

g. O(n) # the recursion is once per call 

## Excercise II

a. 
```
def findMax(arr, l, h):
    max = arr[l]
    i = low
    for i in range(h+1):
        if arr[i] > max:
            max = arr[i]
    return max
```
b. we assume:
  * there are n-floors and x eggs
  * an egg which is broken must be discarded
  * if an egg breaks when dropped from a given floor, it will also break on any higher floor
  * if an egg survives a fall, it will also survive a shorter fall

  => To solve this problem it would be better to apply `dynamic programming` approach to obtain more efficient result.


## Excercise III
a. In this case the running time of algorithm will be _**O(n<sup>2</sup>)**_ because here we are choosing the first element as partition which makes the array of size n into two arrays of size 1 and n - 1.

b. In this case the running time of algorithm will be _**O(nlogn)**_ because here finding the median of an arry runs in _**O(n)**_ time, which means that the recurrence equation for quicksort in the worest case will be `T(n)=O(n)(find the median) + O(n) (partition) + 2T(n/2) (recurse left and right)` and this is `O(nlogn).`