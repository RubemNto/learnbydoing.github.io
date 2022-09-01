## **Create Project Generation Script**

For the beginning of this development journey, the first part for the good flow of developing new features is repeatable situations where the Game developer may se itself in.

For that reason, the creation of a simple Shell script was made and with the focus of following simple C++ programming convetions and some new ones created by me just because...

For the moment, the choice of C++ as the programming language mostly comes for it's not so low level nature of the language and the wide use of it in the Back-end side of game development.

For the graphics part, the real choices for the Linux user developing the kit where between Vulkan or OpenGL. Either one for a 2D focused project will be great, but the future of the project, if successful, is to expand to the 3D world too. Both OpenGl and Vulkan are capable of 3D rendering, but given that the Vulkan API is growing in popularity and being developed to be the natural successor of OpenGl, the API choosen was Vulkan.

### **Structure Design**

The structure of the BGDK projects may change with time. But now it follows the image bellow.

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
Indeed is simple, but it works and it's ideal for starter projects if the developer is looking to start something from nothing or a Console application using the Vulkan API.
The starter template comes with some files pre configured, but with nothing more than simple class definitions and the main run function to execute the program.

For now the biggest flaw of the BGDK starter template is not utilizing the CMake technology, making project generation faster and easier.

### **Running the project generator**

As a project generator, for the moment it just allows the user to generate the starter template for Terminal based applications.
To access the script, feel free clone the project by following this command: 

```bash
git clone https://github.com/RubemNto/Vulkan-Project-Generator.git

cd Vulkan-Project-Generator

chmod - X Vulkan-Templates-Generator.sh

bash ./Vulkan-Templates-Generator.sh
```
After running the script, follow the instructions and you should have a BGDK project running. 