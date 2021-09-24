# C-- program syntax recognizer
 A project assignment of Compiler Technology of Programming Languages course in NTU. C-- (pronounced C minus minus) is a C-like programming language. More datailed specification of [C--](https://drive.google.com/file/d/1mqIG6JDIcNYxValdV83zUXzc0i7tExel/view?usp=sharing). 

In this repository, following files can be found:

|   file name   |                     discription                      |
| :-----------: | :--------------------------------------------------: |
|  src/lexer.l  | lex program that recognizes lexical patterns in text |
| src/parser.y  | YACC file produce parser for given production rules  |
| src/header.h  |             contains AST data structure              |
| src/functions |      contains functions used to generate AST.gv      |
|  src/alloc.c  |              AST node memory allocation              |
| src/Makefile  |                                                      |
|     test/     |        directory containing some sample tests        |

# Usage
To compile:
1. cd src
2. make

To run:  
1. ./parser <source_file> 
2. dot AST_Graph.gv -T png -o <output_file> 

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
 > dot AST_Graph.gv -T png -o out.png 

Abstract syntax tree of this program will then be generated with graphic layout **out.png** as followed:  
![out](https://user-images.githubusercontent.com/89965190/132562744-11a8ea28-7cd4-4a2d-820e-4acf02ae2c28.png)

