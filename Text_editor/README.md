# Text_Editor using C

## Roadmap

0) Choosing and setting up an IDE/editor of your choice and programming language of choice.  
My Choice:  
    Code editor- **VS Code** <img src="assets/vscode.png" alt="VS_Code Icon" width="16" height="16">  
    Programming language- **C**  <img src="assets/c_programming.png" alt="C Icon" width="16" height="16">  
  
1) In this step, we create a program that starts up and allows the user to quit when they press '**q**'.  
    - Read from stdin unbuffered - so you’re not waiting for the user to press return.
    - Disable the default echoing of input to stdout.
    - Disable output processing by the terminal.
    - Disable all handling of CTRL-C, CTRL-Z, CTRL-M, CTRL-S, CTRL-Q, CTRL-V.  

2) To have our editor clear the screen when started and position the cursor at the top left of the screen.  
   Once that's sorted, we create a vertical line of characters down the lefthand side of the screen (Just like vim does, **~**).  

3) Now, we allow the user to move the cursor around the screen.  
    - **h**: left movement
    - **j**: downward movement
    - **k**: upward movement
    - **l**: right movement  

4) Allow the user to enter some text.  
    We do this by having a 'control mode' and 'editor mode'.  
    Then we allow the user to switch between the two modes:
    - **'esc' key** for 'control mode'
    - **'i' key** for 'editor mode.'  

5) Now we create a support for opening and saving files.  
    The user should be able to provide a filename at the startup, and have the editor open the file.  

## The Actual Program
### Header Files used

**stdio.h**  
--> basic input/output  

**unistd.h**  
--> read keyboard input  
--> write to terminal  
--> process management  
--> file descriptors  

**termios.h**  
--> control terminal behavior  
    (raw mode, echo, etc.)  

**sys/ioctl.h**  
--> communicate with terminal/device  

**sys/types.h**  
--> system-specific data types  



