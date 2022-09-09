# C+ (notes)

## WEEK 1
- Compiling wihout ```-o``` will automatically produces a file named ```a.exe```.
- To **compile**, input this into the integrated terminal: "g++ -std=c++11 filename.cpp -o filename"
- **Compile** the ```.cpp``` file into an executable file, which can then be run.


### Namespace
A declarative region where its identifiers can be grouped and put together into the same scope for reference. Avoid naming conflicts, allows for categorization and grouping.

#### Bad naming practice.
Don't use ```namespace::std```.

Reason: https://stackoverflow.com/questions/1452721/why-is-using-namespace-std-considered-bad-practice
