# C-- program syntax recognizer and semantic checker
 A project assignment of Compiler Technology of Programming Languages course in NTU. C-- (pronounced C minus minus) is a C-like programming language. More datailed specification of [C--](https://drive.google.com/file/d/1mqIG6JDIcNYxValdV83zUXzc0i7tExel/view?usp=sharing). 

# Usage
To compile:
1. cd src
2. make
  
To run:  
1. ./parser <source_file> 
2. dot -Tpng -o out.png AST_Graph.gv

# Example
A C-- example program **test.c** is shown below:
```c
int main() {
	a=1+2+3;
}
```
After running program as follow:  
 > ./parser ./test.c

Output files: **AST_Graph.gv** will be generated, then run the following command to convert gv file to png file with graphviz tool:
> dot -Tpng -o out.png AST_Graph.gv

Abstract syntax tree of this program will then be generated with graphic layout as followed:  
![out](https://user-images.githubusercontent.com/89965190/132294798-0d4baf6f-3f3c-48a1-b3f4-87c15df840c9.png){:height="10%" width="10%"}

