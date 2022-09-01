## **Creating Vulkan Console Template Project**

You might be asking yourself.

Why would you create a **CONSOLE** based template for the **GAME DEVELOPMENT KIT**? Are you OK? Have you switched from COFFEE to TEA?

Well, I'm Ok and my coffee is still my valiable companion for harsh moments, but the logic for the template is that, sometimes, less is more.
In the Game Development side of the GDK a console application may be weird not to say stupid. But in the case of invisible work, having a standard place to start is always a plus for future templates. And for future projects like server management and data transfers, the console environment is more than enough and ideal for work that the user either doens't want to look at or to work on.

## **Console Template**

Given that the development of the GDK is in C++, it is important to follow the C++ guidelines on best practices with the language and keep consitent with naming convetions and human language to code in.

For the structure of the project, we follow the same one mentioned in the [Create Project Generation Script]() post.

```
RootFolder/
    build/
    header/
        program.hpp
    src/
        program.cpp
        main.cpp
    Makefile
``` 
One imporatant thing to remember is that there is no CMake list for the Makefile generation.
For the moment the Makefile can do all we need for Game Development and background work.
For the future, is intended to use [**CMake**]() to keep consistency and repeatable work

## **Explaining Code**

The project structure has two fundamental cpp files and one hpp file.
the main file is most of the time, unchanged. But feel free to change it as you need, but it's recomended to do that in the program.cpp file.

The header file, should be just the definition of functions and whatever varaibales and data needed for the program, while the program.cpp is where you define them and use them as needed.