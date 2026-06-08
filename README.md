# DSA_learnings

Data: data is raw, unorganized facts that needs to be processed.

Structure: The way data is organized related it defines the relationship btwn the pieces of data

Data Structure: It is the way of organizing or storing the data in computers main memory so that it can be used efficiently.
ex: menu book we can find what we want by seeing particular section.

Program: Set of instruction that tells a computer what to do . it manipulates the data to achieve a specific task.

Program and data: programs operate on data. The way data is organized significantly impacts the programs efficiency.


Why Organize data?
1.Efficient accessing, searching, sorting
2.easier to update, dlt etc
3.reducing memory usage


Algorithm: step by step procedure or a set of rules to solve a problem. or finite sequence of steps/procedure to solve a specific problem
ex: procedure of making tea.

Properties of Algorithm:-
1.Finiteness: alg terminate after finite no of steps.
2.Definiteness: clear and unambiguous(clearly mentions what to do).
3.Input:well defined inputs.
4.Output:one or well defined outputs.

Importance of Data structure and Algorithm:
1.Efficient data storage and access
2.Scalability:handles large datasets
3.Organization:memory efficient storage of data
4.Problem Solving:

Impact of Efficient Algorithm:
1.Faster processing
2.Resource optimization


TIME AND SPACE COMPLEXITY:-

Analysis of algorithm: it is the process of determining the of resources required by an alg to solve a problem.
It helps to selecting the most efficient alg for specific task.
Readability-easy to read
Scalability-works on  large data also small data

Complexity of analysis :subset of analysing algorithm
It ensures that we select the best algorithm.


Time Complexity:it is expressed in big oh O(n) notation
     
O(n)-->linear search

O(log n)-->binary search

Time Complexity measures the growth rate of an algorithm's execution time as the input size increases
Not actual time
Focus on scaling

Big O Notation -Worst Case
It describes the upper bound of an alg time complexity, representing the worst case scenario. it ensures that won't taken longer than expected

Rules for Calculating Complexity:
Loops
statements
function calls

Space Complexity : it measures the amount of memory an alg uses in relation to the input size

Auxilliary space- extra space used by the alg beyond the input size
In place algorithms - algorithms that use a constant amount of extra space are called in-place algorithms and have an auxiliary space complexity of O(1).

Ex:Bubble sort


ARRAYS IN DATA STRUCTURE:

Array is a collection of more than 1 element of similar datatype, elements are stored in consecutive(continues) location.
In runtime the size of array can't be changed
To access a particular array element=arrayNmae[index]

Syntax of array :
data_type array_name[];
int[] rollno=new int[40]; --> instantiation of array
here rollno is refference

Array Initialzation:
array Initializer -int no=[1,2,3,4,5];

Individual Assignment -int[] no = new int[8];

Runtime Initialization -int[] no = new int[5];
                        for(int i = 0;i<no.length;i++){
                        nu[i]-i+1;
                        }

Memory Representationf Array:
Stack Memory : stores the reference variable that points to the array obj in the heap.
Heap Memory : Stores the actual obj which contains the elements and metadata such as size and data type

example :
public class Array{
public static void main(String[] args){
//int[] numbers;  -->declaration
//numbers=new int[5];  --> Initialization
numbers=new[] {1,2,3,4,5}; --> we can initialize and declare in the same line
System.out.println(numbers);
}
}

NOTE :- default value for int is 0
        default value for array or obj is null
        local(a) variables are diff

types of array:
1.1D array
2.2D array
3.multi dimentional array

1.1D array 
! row multiple columns
Calculation of address of the array =base address+i*size of data type
ex: int a[5]={6,2,4,3,0};
address os 2nd index = 100+2*4 =108              ( here 100 is taken for understanding purpose                                                         address should be in hexadecimal form)
address of 4 is 108
 




