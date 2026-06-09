<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=6C63FF&height=180&section=header&text=DSA%20Learnings%20📚&fontSize=40&fontColor=ffffff&fontAlignY=38&desc=My%20Personal%20DSA%20Journey%20%7C%20Notes%20%2B%20Code&descAlignY=58&descSize=16" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=6C63FF&center=true&vCenter=true&width=600&lines=Learning+Data+Structures+%26+Algorithms;One+concept+at+a+time+💡;Notes+%2B+Code+%2B+Practice)](https://git.io/typing-svg)

![](https://img.shields.io/badge/Language-Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

</div>

---

## 🗺️ Topics Covered

| # | Topic | Status |
|---|---|---|
| 1 | 📌 Introduction to DSA | ✅ Done |
| 2 | ⏱️ Time & Space Complexity | ✅ Done |
| 3 | 📦 Arrays | ✅ Done |
| 4 | 🔗 Linked Lists | 🔄 Coming Soon |
| 5 | 📚 Stacks & Queues | 🔄 Coming Soon |
| 6 | 🌳 Trees | 🔄 Coming Soon |
| 7 | 🔍 Searching Algorithms | 🔄 Coming Soon |
| 8 | 🔃 Sorting Algorithms | 🔄 Coming Soon |
| 9 | ⚡ Dynamic Programming | 🔄 Coming Soon |

---

## 📌 1. Introduction to Data Structures

> 💡 *"The way data is organized significantly impacts the program's efficiency."*

**Data:** Data is raw, unorganized facts that needs to be processed.

**Structure:** The way data is organized related it defines the relationship btwn the pieces of data.

**Data Structure:** It is the way of organizing or storing the data in computers main memory so that it can be used efficiently.
> ex: menu book — we can find what we want by seeing particular section.

**Program:** Set of instruction that tells a computer what to do. It manipulates the data to achieve a specific task.

**Program and data:** Programs operate on data. The way data is organized significantly impacts the programs efficiency.

### ❓ Why Organize Data?
1. Efficient accessing, searching, sorting
2. Easier to update, delete etc
3. Reducing memory usage

---

### 🧮 Algorithm

> Step by step procedure or a set of rules to solve a problem. Or finite sequence of steps/procedure to solve a specific problem.
> ex: procedure of making tea.

**Properties of Algorithm:**

| Property | Description |
|---|---|
| **Finiteness** | Algorithm terminates after finite no of steps |
| **Definiteness** | Clear and unambiguous (clearly mentions what to do) |
| **Input** | Well defined inputs |
| **Output** | One or well defined outputs |

### 🌟 Importance of DSA
1. Efficient data storage and access
2. **Scalability** — handles large datasets
3. **Organization** — memory efficient storage of data
4. **Problem Solving**

### ⚡ Impact of Efficient Algorithm
1. Faster processing
2. Resource optimization

---

## ⏱️ 2. Time and Space Complexity

**Analysis of Algorithm:** It is the process of determining the resources required by an algorithm to solve a problem. It helps in selecting the most efficient algorithm for a specific task.

- **Readability** — easy to read
- **Scalability** — works on large data as well as small data

**Complexity Analysis:** Subset of analysing algorithm. It ensures that we select the best algorithm.

### 🕐 Time Complexity

> Time Complexity measures the **growth rate** of an algorithm's execution time as the input size increases.
> - Not actual time
> - Focus on **scaling**

| Notation | Meaning | Example |
|---|---|---|
| `O(n)` | Linear | Linear Search |
| `O(log n)` | Logarithmic | Binary Search |
| `O(1)` | Constant | Array Access |

**Big O Notation — Worst Case:**
> Describes the upper bound of an algorithm's time complexity, representing the worst case scenario. It ensures the algorithm won't take longer than expected.

**Rules for Calculating Complexity:**
- Loops
- Statements
- Function calls

### 💾 Space Complexity

> Measures the amount of memory an algorithm uses in relation to the input size.

- **Auxiliary space** — extra space used by the algorithm beyond the input size
- **In-place algorithms** — algorithms that use a constant amount of extra space → `O(1)` auxiliary space
  > ex: Bubble Sort

---

## 📦 3. Arrays

> **Array** is a collection of more than 1 element of similar datatype, elements are stored in consecutive (continuous) location.
> In runtime the size of array **can't be changed**.
> To access a particular element → `arrayName[index]`

### 📝 Syntax

```java
data_type array_name[];
int[] rollno = new int[40];  // instantiation of array
// here rollno is a reference
```

### 🔧 Array Initialization

```java
// Array Initializer
int no[] = {1, 2, 3, 4, 5};

// Individual Assignment
int[] no = new int[8];

// Runtime Initialization
int[] no = new int[5];
for (int i = 0; i < no.length; i++) {
    no[i] = i + 1;
}
```

### 🧠 Memory Representation

| Memory | Role |
|---|---|
| **Stack Memory** | Stores the reference variable that points to the array object in the heap |
| **Heap Memory** | Stores the actual object which contains the elements and metadata (size, data type) |

### 💻 Declaration & Initialization Example

```java
public class Array {
    public static void main(String[] args) {
        // int[] numbers;           // declaration
        // numbers = new int[5];    // initialization
        int[] numbers = new int[]{1, 2, 3, 4, 5}; // declare + initialize

        System.out.println(numbers[0]);
    }
}
```

### ⌨️ Runtime Initialization

```java
public class Array {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int[] numbers = new int[5];

        System.out.println("Enter array Elements:");
        for (int i = 0; i < numbers.length; i++) {
            numbers[i] = sc.nextInt();
        }
        System.out.println(numbers[0]);
    }
}
```

> 📌 **NOTE:**
> - Default value for `int` → `0`
> - Default value for array or object → `null`
> - Local variables are different

### 🛠️ Array Manipulation Methods

| Method | Description |
|---|---|
| `Arrays.sort(array)` | Sorts the elements in an array |
| `Arrays.fill(array, value)` | Fills an array with a specific value |
| `Arrays.copyOf(array, newSize)` | Creates a copy of an array with a specified size |
| `Arrays.binarySearch(array, element)` | Searches for an element in an array |

### 📐 Types of Arrays

1. **1D Array** — 1 row, multiple columns
2. **2D Array**
3. **Multi-dimensional Array**

**Address Calculation (1D Array):**
```
Address of element = Base Address + i × Size of Data Type

Example: int a[5] = {6, 2, 4, 3, 0};
Address of index 2 = 100 + 2×4 = 108
∴ Address of element 4 is 108
(100 is base address for understanding; actual address is in hexadecimal)
```

---

<div align="center">

### ⭐ Keep learning, keep growing!

*"An investment in knowledge pays the best interest."*

[![](https://img.shields.io/badge/GitHub-KAVANAMP-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KAVANAMP)

<img src="https://capsule-render.vercel.app/api?type=waving&color=6C63FF&height=100&section=footer" width="100%"/>

</div>
