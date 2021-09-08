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
A C-- program **test.c** is shown below:
```c
int main() {
	int a=1+2+3;
}
```
After running program as follow:  
 > ./parser ./test.c

Output files: **AST_Graph.gv** will be generated, then run the following command to convert gv file to png file with graphviz tool:
> dot -Tpng -o out.png AST_Graph.gv

Abstract syntax tree of this program will then be generated with graphic layout as followed:  
![out](https://user-images.githubusercontent.com/89965190/132562744-11a8ea28-7cd4-4a2d-820e-4acf02ae2c28.png)

