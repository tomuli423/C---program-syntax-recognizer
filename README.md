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
