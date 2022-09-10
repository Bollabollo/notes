# C+ (notes)

## WEEK 1
- Compiling wihout ```-o``` will automatically produces a file named ```a.exe```.
- To **compile**, input this into the integrated terminal: "g++ -std=c++11 filename.cpp -o filename"
- **Compile** the ```.cpp``` file into an executable file, which can then be run.


### Namespace
A declarative region where its identifiers can be grouped and put together into the same scope for reference. Avoid naming conflicts, allows for categorization and grouping.

### Preprocessor directives
Include directives that indicates that a program should be included in the compilation. For example, standard C++ libraries should be added. All preprocessor directives start with ```#```

#### Bad naming practice.
Don't use ```namespace::std```.

Reason: https://stackoverflow.com/questions/1452721/why-is-using-namespace-std-considered-bad-practice

### Statement
The declaration of an identifier (the introduction of a name)

### Function 
#### **Main** function
This is a special function. Read more on it.
#### Definition
The general form of a C++ function definition is usually as follows:
```
return_type function_name( parameter list ) {
   body of the function
}
```
The function declaration followed immediately by the _block of statements (function body)_
#### Declaration
Tells the compiler about the function name, its parameters, what value it returns and how to call it.
```
return_type function_name( parameter list );
```
### Character literals
Composed by a character. A character constant is surrounded by single quotation marks to be encoded by C++
```
std::cout <<'a'; //Outputs a
```

**BLANK TAB NL (New line)** characters are referred to as _whitespace_ characters.




