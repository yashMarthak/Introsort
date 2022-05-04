# INTROSORT

> In c++ library, default sort function uses the intro sort.
- Intro sort is nothing but, combination of three basics sorting algorithm
1) Insertion Sort
2) Quick Sort
3) Heap Sort

- Every sorting algorithm has its advantage and disadvantage.
- So intro sort, uses the advantage of this three basic algorithm to improve the time complexity.
Insertion for small input will not take much time.
- Quick sort for small input will create so many function calls recursion.
As well as heap sort for less depth will work efficiently. So using this all aspects intro sort is 
implemented.
- If input size is less then defined size then insertion sort will be used, else if depth is zero then use heap 
sort else use quick sort

<hr>

> ### How to run
<hr>

1) Make executable

```bash 
$gcc introsort.cpp -o introsort.exe
```
2) Run executable

```bash 
$ introsort.exe
```
or

```bash 
$ g++ -o introsort introsort.cpp
```

> ### Introsort Performance

- Introsort sorting algorithm provides both fast average performance and (asymptotically) optimal worst-case performance. Both the average-case and worst-case time complexity of introsort are <b>O(n.log(n))<b>, where n is the size of the input. 


- The auxiliary space required by the introsort algorithm is <b>O(n)<b> for the call stack when the naive Quicksort algorithm is used. To keep the stack depth bounded by <b>O(log(n))<b>, recur first into the partition’s smaller side, then use a tail call to recur into the other.
