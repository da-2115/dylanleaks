### Slides 1-50
#### Notes
- A programming language is a formal notation for describing computation,
- A "user interface" to a computer,
- A more precise tool than any natural language.
- An interpreter consists of two parts:
	- A front end that converts program text (a program in the source language) to an AST (abstract syntax tree).
	- An evaluator (or interpreter) inspects a data structure and performs associated actions.
	- Some examples include: a calculator, JVM (Java Virtual Machine), Basic, Perl, Python, etc.
- A compiler translates program text into a related (target) language, the building blocks are:
	- A front end that converts program text (a program in the source language) to an AST (abstract syntax tree).
	- A set of independent compiler phases, each has assigned a particular task throughout the compilation process (e.g. semantic analysis, optimisation, register allocation, code emission).
	- The evaluator of a compiled language may be an interpreter (e.g. JVM) or simply a hardware machine (von Neumann computer).
- Programming language generations:
	- 1GL: machine code
	- 2GL: symbolic assemblers
	- 3GL: higher-level (machine-independent) languages (e.g. C, C++, Java, Pascal)
	- 4GL: domain-specific language support and generators (e.g. JavaCC, LINQ)
	- 5GL: finite-domain constraint-based logic languages (e.g. Prolog)
- Programming domains
	- Scientific applications: floating-point arithmetic (Fortran, R)
	- Business applications: reports (Cobol)
	- AI: symbolic computation (Lisp, Prolog, R)
	- System programming: operating systems (C/C++, Java, C#)
	- Scripting languages: system configuration (Bash, Python)
- Imperative Programming
	- Oldest style of programming, where the algorithm for computation is expressed in terms of instructions, such as assignments, branching, etc.
	- Execution of the algorithm requires data values to be held in variables - the state which can be accessed and modified to produce - side effects - new state.
- Functional Programming
	- Based on lambda calculus
	- Takes a more mathematical approach
	- Pure functional programming languages do not rely on variables, rather a composition of functions.
	- The most prominent functional programming style languages are Haskell, Lisp, Python.
- Object-Oriented Programming
	- OO languages are based on the ideas of objects, classes and inheritance.
	- The most prominent OO languages include Smalltalk, C++, Java, C# and Python.
- Sequential Languages
	- Instructions are executed in sequential order deduced from the program text.
	- Mostly widely used languages
	- Correspond to the classic Von Neumann computer architecture.
- Parallel Languages
	- A Turing tarpit is any programming language that allows flexibility but is difficult to achieve common tasks with
	- For example, C++ is like Java and may be good for some tasks, but ill-suited for others.

#### Questions
- What is a programming language?
- What is a token?
- What is an Abstract Syntax Tree?
- What is an interpreter?
- What two parts does an interpreter contain?
- What is a compiler?
- What are the building blocks of a compiler?
- What is the difference between an interpreter and a compiler?
- What are two examples of an interpreted language?
- What are the 5 programming language generations?
- What are two examples of a compiled language?
- What is imperative programming?
- What is functional programming?
- What is object-oriented programming?
- What is a sequential language?

##### Take 1 (87%)
- What is a programming language?
Answer: A programming language is the way we wrap the complexity of computation into our minds. Basically, a way to write human readable programs that can run a computer in binary format.
- What is a token?
Answer: A token is a word in a line of a program in a particular programming language, this can be useful for grabbing tokens when a program text is inputted to an interpreter or compiler, to map these tokens to an Abstract Syntax Tree (AST).
- What is an Abstract Syntax Tree?
Answer: An Abstract Syntax Tree (AST) is a data structure that is used heavily in programming language development as it contains a tree of all the instructions in a program file and what order they are in.
- What is an interpreter?
Answer: An interpreter interprets a program written in a particular to another programming language and maps the instructions using an AST.
- What two parts does an interpreter contain?
Answer: A lexer, and a parser.
- What is a compiler?
Answer: A compiler compiles a program written in a particular programming language to a target language.
- What are the building blocks of a compiler?
Answer: Semantic analysis, AST, optimisation, etc.
- What is the difference between an interpreter and a compiler?
Answer: An interpreter sends the program to another language specifically, a compiled language whereas a compiler directly sends it to the target language.
- What are two examples of an interpreted language?
Python, Java
- What are the 5 programming language generations?
1GL, 2GL, 3GL, 4GL, 5GL
- What are two examples of a compiled language?
Answer: C and C#
- What is imperative programming?
Answer: Imperative programming is the earliest Von Neumann based model of programming - where instructions and variables make up the program.
- What is functional programming?
Answer: Based on lambda calculus, functional programming consists purely of a composition of functions.
- What is object-oriented programming?
Answer: Object-oriented programming is based on the idea of classes, objects & inheritance. OO programs consist of different classes and uses message passing to talk between objects.
- What is a sequential language?
Answer: A sequential language is where the instructions of a program in a programming language are executed in sequential order.

### Slides 51-100
#### Notes
- Syntax
	- Syntax is concerned with how expressions, command, declarations, etc are put together to form programs.
	- Syntax is to guide the programmer to understand the language's semantics.
- Semantic Analysis
	- This phase connects variable definitions to their uses,
	- Checks that expressions are well-formed
	- Translates the AST into a possibly simpler intermediate representation more suitable for code generation
	- and triggers the evaluation of the program or maps the AST to a target language.
	- 
#### Questions
