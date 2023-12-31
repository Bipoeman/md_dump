# 📚 Topics to learn in C 👨‍🏫
- **Getting started with C Language**
    - The history of C.
    - The evolution of the C programming standards.
    - The relationship of C to C++.
    - Some recommended / free books for learning C.
    - Source Code Compilation, Cross-Compilation Process.
    - C/C++ Toolchains and Open Source IDEs.
- **Compiling**
    - `gcc = gcc C compiler`
    - `gcc -o myprog hello.c` create an executable output file called myprog and hello.c is input source code.
- **Code Comments**
    - Single-line comments: // ....
    - Multple-line comments: /* ... */
    - Keywords or reseverd words in C
- **Data Types**
    - Basic data types
        - 'int' represents integers (whole numbers) with varying sizes depending on the platform.
        - 'char' represents single characters.
        - 'float' represents single-precision floating-point numbers.
        - 'double' represents double-precision floating-point numbers.
        - 'bool' (via #include `<stdbool.h>`) represents boolean values ('true' or 'false').
        - '_Bool' (C99's boolean type)
        - `'unsigned char'` declares a variable which can hold values from 0 to 255.
    - Derived Data Types
        - Arrays, structures, unions
        - Enumerated data types (the 'enum' keyword)
    - 'void' data type
        - a special data type that indicates the absence of a specific type.
        - used to represent a lack of value or to indicate that a function does not return any value.
- **Type Modifiers for Numbers**
    - integers: such as 'signed', 'unsigned', 'short', 'long', 'long long'
    - floating-points: 'long' (for 'float' and 'double')
- **Type Conversions**
    - Implicit: short to int to long, float to double.
    - Explicit: (<type>)(expression) for type-casting.
- **Literals (constant values of specific data types)**
    - Primitive vs. Compound Literals
    - Integer Literal: 42, -100, 0, 123456
    - Octal Literal: 0644
    - Hexadecimal Literal: 0x1A, 0xFF, 0xABC
    - Floating-Point Literal: 3.14, -0.005, 1.0e-5
    - Character Literal: 'A', '5', '!', '\n'
    - Boolean Literal (C99 and later): true, false
    - String Literal: "Hello, world!", "" (an empty string)
- **Identifiers and Variables**
    - Identifier Naming
    - Variable Definition and Initialization
    - Variable Scope
    - Constants (with the const keyword)
    - Declaration vs. Definition
    - A declaration introduces an identifier to the compiler and informs it about the data type and name of the identifier.
    - A definition creates the actual instance of an identifier in memory. It allocates memory for variables and provides the implementation for functions.
    - Global & local variables
- **Operators**
    - Arithmetic Operators: +, -, *, /, %, ++, --
    - Relational Operators: ==, !=, >, <,>=, <= - Logical Operators: &&, ||, ! 
    - Bitwise Operators: &, |, ^, ~, <<,>>
    - Assignment Operators: =, +=, -=, *=, /=, %=, &=, |=, ^=, >>=, <<= 
    - Conditional Operator: () ? () : () 
    - Miscellaneous Operators: 
        - , (comma), & (address-of operator) 
        - sizeof(...) used to determine the size in bytes of a data type or variable. 
        - . (dot or memory-access operator) 
        - -> (memory-access operator),
        - [...] (square bracket or array indexing operator)
    - Side Effects of the ++ and -- Operators for Value Modification
        - Pre-increment and Pre-decrement
        - Post-increment and Post-decrement
        - Order of Evaluation
    - Short-circuit logical operators
        - The && (logical AND) operator: (expr1 && expr2)
        - The || (logical OR) operator: (expr1 || expr2)
        - These short-circuit operators halt evaluation once the final outcome is determined by the preceding sub-expressions.
- **Strings**
    - A string is a sequence of characters stored in an array that represents text.
    - terminated by a null character ('\0').
    - accessible by a (char *) pointer.
    - `string terminator` = String in C always end with a byte set to 0
    - `mystring[]` declaresd as as array often chars
- **String library**
    - `Using the C string library to simplify common opearations on strings`
    - `<string.h> : strcpy() , strcat() , strlen() , strcmp() , strncmp()`
- **User input**
    - `sscanf` reads values from string
    - `scanf` reads values directly from the console
    - `fgets` 3 arguments : buffer store input : maximum number of byte : where to read from (stdin = read from the console)
- **Array: 1D and 2D**
    - llection of elements of the same data type, stored in contiguous memory locations.
    - `Relationship between pointers and arrays` = Can use pointer to access the address in elements of the array.
    - `Elements in arrey use adjacent address`
- **Structs (short for structures)**
    - a composite data type that allows you to group together variables of different data types under a single name.
- **Union**
    - a user-defined data type that all members of a union share the same memory location.
- **Bit-field**
    - a bit field is used to specify the number of bits to be used to store a particular data member within a struct.
- **Enumeration (enum)**
    - a user-defined data type that consists of a set of named integer constants.
- **Typedef for user-defined types**
    - used to create an alias or a new name for an existing data type.
    - provides a way to define custom names for data types.
- **Statements such as**
    - Iteration Statements/Loops: for, while, do-while
    - Selection Statements: if, if-else, switch-case
    - Assignment Statements
    - `Leaving a loop early : break`
- **Functions**
    - Variable arguments of a function
    - `Build and calling a function`
    - `Returning the value of a function`
- **Pointers**
    - Pointer Arithmetics
    - Function Pointers and Parameters
    - `Name are pointers` = The name of an array or a string is just a pointer to the frist element of the array or string.
- **Header files and the preprocessor**
- **C Preprocessor Directives and Macros**
    - #include <...>: include header files.
    - #define
    - #if, #else, #ifdef, #ifndef, #endif, #undef
    - #error
- **Command-line arguments to the main() function**
    - provided by the user when they run the program and can be used to pass information or parameters to the program.
    - int main(int argc, char *argv[]) { ... }
- **The C Standard I/O library**
    - printf() and scanf() functions.
    - fprintf() functions and the output streams ('stdout' and 'stderr').
    - Formatted strings for Input/Output
- **Files and I/O streams**
    - <stdio.h> (Standard I/O Library) provides functions for basic input and output operations.
        - Examples of functions in this library:
        - fopen(), fclose()
        - fprintf(), fscanf()
        - fputc(), fgetc(), fgets(), fputs()
        - fwrite(), fread(), feof(), fseek(), rewind()
        - `file access mode : rb+ , wb+ , ab+`
    - Other standard C libraries:
        - `<stdlib.h>` provides functions for various file operations.
        - `<unistd.h>` (Unix Standard Library) provides functions for low-level file operations.
        - `<sys/types.h>` and `<sys/stat.h>` provide data types and functions for working with file status and attributes.
        - `<fcntl.h>` provides functions for managing file descriptors and controlling file attributes.
- **Pseudo-Random Number Generation**
    - srand(): used to seed the random number generator.
    - rand(): returns an integer between 0 and RAND_MAX.
    - Both functions are declared in `<stdlib.h>`
- **The C Standard Math library**
    - The `<math.h>` header file must be included in source code in order to use the C Standard Math library.
    - The `-lm` flag must be specified for program linking (when using GCC C compiler).
- **POSIX Threads and Multithreading**
    - often referred to as pthreads.
    - a standardized threading library for creating and managing threads in a multi-threaded program.
- **Baic GTK**
    - What is GTK
        - Muli-platform toolkit for GUI
    - GTK Version
        - GTK 2 Stable
        - GTK 3 Under development more features
    - Header file `#include<gtk/gtk.h>`
    - Basic Command
        - `gtk_init(&argc,&argv)`
        - `gtk_window_new()`
        - `gtk_widget_show(win)`
        - `gtk_main()`
    - Button and More
        - `gtk_button_new_with_label(label)`
        - `gtk_container_add(GTK_CONTAINER(win),btn)`
        - `gtk_widget_show_all(win)` 
        - `gtk_label_set_text(GTK_LABEL(ptr),buffer)`
        - `gtk_table_attach_default(GTK_TABLE(tbl),lbl)`
        - `g_signal_connect_(chk,"toggled",G_CALLBACK(check_toggle),NULL)`
    - List stores
        - Text combo boxes
            ``` C
            GtkWidget *comb = gtk_combo_box_text_new (); // new empty combo box
            gtk_combo_box_text_append_text (GTK_COMBO_BOX_TEXT (comb), "Option 1");
            gtk_combo_box_text_append_text (GTK_COMBO_BOX_TEXT (comb), "Option 2");
            gtk_combo_box_text_append_text (GTK_COMBO_BOX_TEXT (comb), "Option 3");
            gtk_combo_box_set_active (GTK_COMBO_BOX (comb), 0);

            int sel = gtk_combo_box_get_active (GTK_COMBO_BOX (comb)); // Read currently selected item

            ```
        - Combo Callback
            ```C
            void combo_changed (GtkWidget *wid, gpointer ptr)
            {
                int sel = gtk_combo_box_get_active (GTK_COMBO_BOX (wid));
                char *selected = gtk_combo_box_text_get_active_text (
                GTK_COMBO_BOX_TEXT (wid));
                printf ("The value of the combo is %d %s\n", sel, selected);
            }
             g_signal_connect (comb, "changed", G_CALLBACK (combo_changed), NULL);
            ```
    - Menus
        - Menu bars
            - `GtkWidget *mbar = gtk_menu_bar_new ()`
        - Pop-up Menus
            ```C
            //Handler to connect it to the clicked signal on a button.
            void button_popup (GtkWidget *wid, gpointer ptr)
            {
                GtkWidget *f_menu = gtk_menu_new ();
                GtkWidget *quit_mi = gtk_menu_item_new_with_label ("Quit");
                gtk_menu_shell_append (GTK_MENU_SHELL (f_menu), quit_mi);
                g_signal_connect (quit_mi, "activate", G_CALLBACK (end_program),
                NULL);
                gtk_widget_show_all (f_menu);
                gtk_menu_popup (GTK_MENU (f_menu), NULL, NULL, NULL, NULL, 1,
                gtk_get_current_event_time ());
            }
            ```
    - Dialogs
        ```C
        // This can be connected to `clicked` signal with g_signal_connect
        void open_dialog (GtkWidget *wid, gpointer ptr)
        {
            GtkWidget *dlg = gtk_dialog_new_with_buttons ("My dialog",
            GTK_WINDOW (ptr),
            GTK_DIALOG_MODAL | GTK_DIALOG_DESTROY_WITH_PARENT,
            "Cancel", 0, "OK", 1, NULL);
            int result = gtk_dialog_run (GTK_DIALOG (dlg));
            gtk_widget_destroy (dlg);
            printf ("Return code = %d\n");
        }
        ```
## Review
- Pro
    - Color coded code easy to read
    - Easy to understand language
    - Clear Explaination
- Cons
    - No online Repositry
    - No Code + Result Summary
