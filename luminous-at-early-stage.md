### Interpreter of data structures and algorithms with visualization function

#### by Yury Lapitsky

#### BSUIR, 2016


> *Show me your flowcharts and conceal your tables, and I shall continue to be mystified. 
>  Show me your tables, and I won’t usually need your flowcharts; they’ll be obvious.*
>
> ------- <cite>Frederick Brooks, The Mythical Man-Month (1975)</cite>

###Introduction

Flowcharts are mostly about presenting **how to implement** algorithm, instead of presenting **the main idea** of algorithm.


There are a lot of ways to present algorithms ideas:

Basic idea of the insetion sort:
http://staff.ustc.edu.cn/~csli/graduate/algorithms/book6/3_a.gif

Insertion sort:
https://upload.wikimedia.org/wikipedia/commons/7/7e/Insertionsort-edited.png

Merge sort:
https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Merge_sort_algorithm_diagram.svg/618px-Merge_sort_algorithm_diagram.svg.png


What if try to consider...
***Algorithm == set of changes applied to the input data to produce output data?***


???

https://git-scm.com/images/branching-illustration@2x.png


Definitely the purpose of git system differs a lot. But the main idea that data change itself much more simple to store
and to use than whole file storing.

### Main idea

So what if we could build the system that could:

- to move from the input data to the output data step by step. 
- each step is a data change.
- data change could be displayed according to it's type (simplified case)


### Implementation steps

- **Choose source language - Python.** 
    - Algorithms itself has a lot of difficulties, and there is no reason to add new.(not C-language)
    - Python is inside TOP-10 popular languages. 
    - Python has a lot of tools to parse itself.
    - MIT choosed Python as an main language for the Introduction for to algorithms

- **Design structure**
    - Separate **Visualization** from **Logic**
    - Command-line component
    - Source code tranformer
    - Data changes analyser
    - Visualizations model builder
    - Visualizer
    
- **Implement components (using methodology)** 

### Current state of the project

- Analyze the places where data changes should be collected [DONE]
- Transform source code to collect necessary data changes [DONE]
- Evaluate transformed source code [DONE]
- Build function calls models
- Do filtration to remove unnecessary data
- Build visualiser models
- Implement drawing of the models


### Difficulties.

- Not all algorithms are suitable for the such approach
- A lot temporary variables that will also be found as a data change. (Filtration needed).
- Effective visualizations should consider grouping of the data changes

### Questions?


### The End

### References

- http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-006-introduction-to-algorithms-fall-2011/

Thank you for your time.

yury.lapitsky@gmail.com

https://github.com/skyylex/Luminous-proof-of-concept


