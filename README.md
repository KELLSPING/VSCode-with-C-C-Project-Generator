# VSCode with C/C++ Project Generator #

## Outline ##

* [Dev Env](#dev-env)
* [how to use](#how-to-use)
* [Notes](#notes)
* [Learning Target](#learning-target)

## Dev Env ##

* Package Manager: Chocolatey
  * VSCode
  * MinGW-w64 12.2.0
  * PowerShell core 7

* OS
  * Windows 11

* VSCode Extension
  * C/C++, C/C++ Extension Pack, C/C++ Themes
  * Code Runner
  * C/C++ Project Generator

## how to use ##

* step by step
  1. Go to command pallete (usually : ctrl + shift + p)
  2. Search for "Create C project" or "Create c++ project" depending on your preference
  3. Select the folder where the project should be created
  4. That's it, project will open

## Notes ##

* Code Runner can only use for compile and run the code, it can not debug the code.

* Two ways to compiler the code.
  * Use "C/C++"
    1. Run C/C++ File
    2. Debug C/C++ File
  * Use "Code Runner"
    1. Run Code

* Setup in the VSCode
  * tasks.json : Used to define tasks for building, which includes compiling and linking programs.
  * launch.json : Used to configure the debugging env, such as the debugger (gdb), executable file path, etc.
  * settings.json : Configures file for the VSCode editor that stores various editor settings. For this case, it used to configure the code runner.

* The "-g" parameter in the "args" parameter of task.json
  * Generates debugging information.
  * Debugging information includes the source code of the program, variable names, function names, line numbers, and other information, which helps to trace, diagnose, and fix problems during debugging.

## Learning Target ##

* learning curve

  1. Use C/C++ Project Generator to create c project, then compile .c files in the "same" folder.

  2. Use C/C++ Project Generator to create c project, then compile .c files in the "different" folder.
