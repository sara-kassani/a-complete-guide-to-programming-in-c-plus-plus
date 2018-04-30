**Steps of creating and translating a C++ program:**

1. *Source code* creation and saving to a *source file* using a text editor. Larger projects use *modular programming* (the process of splitting the source code into several source files);
2. The source file(-s) is/are translated using a *compiler*. On success, an object made up of *machine code* is created (it may some times be referred to as a *module*);
3. The *linker* combines the object file with other modules (*standard libraries*, which contain predefined functions that are available for any compiler, or previously compiled objects) to form an *executable file*.


**Structure of a C++ program:**

- made up of objects with their accompanying *member functions* and *global functions*, which do not belong to any single particular class:
    - each function fulfills its' own tasks and can call other functions;
- the entry point is the *main()* function.


**Description of the *structure-of-the-main-function.png* file:**
- the first line starts with a hash symbol (*#*), which indicates that the line is intended for the *preprocessor*;
- following is the keyword *include <iostream>* (*iostream* - header file, which comprises the convention of the input/output streams (flows) of data), which indicates that the preprocessor should copy the quoted (*<>*) file to this position in the source code;
- *using namespace std;* - predefined names in C++ are found in the *std* (standard) *namespace*. *using* allows direct access to the names in the namespace;
- program execution begins with the first instruction within the *main()* function (in our case, this function contains two *statements*);
- the first statement: *cout << "Enjoy yourself with C++!" << endl;* - outputs *Enjoy yourself with C++!* on screen:
    - *cout* (console output) - designates an object responsible for output;
    - *<<* - indicate that characters are to be "pushed" to the output stream;
    - *endl* (end of line) - causes a line feed.
- the second statement: *return 0;*: terminates the *main()* function and returns an exit code of *0* (it is common practice to return *0* on successful program termination).


**Further notes:**

- the most common C++ source file extensions are: *.cpp* and *.cc*;
- prior to compilation, *header files* (also referred to as *include files*), which store information needed by source files, such as type definitions, variable and function declarations, can be copied to the source file. Their extension is *.h*;
- modern compilers offer an *Integrated Development Environment* (IDE for short), which combines all of the aformentioned steps into a single task;
- a compiler will report an *error* if a source file contains a *syntax error* and a *warning*, which is intended to draw a persons' attention to a possible mistake in the programs' logic.