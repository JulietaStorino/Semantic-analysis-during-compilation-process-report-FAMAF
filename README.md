# Semantic analysis during the compilation process
## Languages and compilers - FAMAF - UNC

### authors
* Florencia Luciana Brunello
* Andrés Valentino Ferrero
* Julieta Paola Storino

This report describes the semantic analysis stage in the compilation process, based on "Modern Compiler Implementation in ML". It introduces the main phases of a compiler: lexical analysis (tokenizing source code), syntactic analysis (parsing program structure), and the construction of the Abstract Syntax Tree (AST).

A key part of semantic analysis is the use of symbol tables (environments) to manage identifiers and their associations. The report compares imperative symbol tables—which use a global environment and undo stacks for updates—with functional symbol tables, where every update creates a new, immutable version. The Tiger compiler uses functional environments.

The report details Tiger’s implementation of symbol tables and type associations, describing how the compiler distinguishes between namespaces for types, variables, and functions. It explains the base environments for types and values, and how variable and function declarations are handled.

Type checking is performed during AST traversal, verifying the validity of variables, functions, scopes, and types. The report outlines the recursive functions used for type checking, showing sample ML code for checking arithmetic expressions, variable accesses, and declarations (variables, types, and functions).

In summary, the report provides an overview of semantic analysis and type verification in the Tiger compiler, emphasizing the design and implementation of symbol tables and environments, and how these facilitate the correct handling of identifiers and type information throughout the compilation process. References from compiler literature are included at the end.
