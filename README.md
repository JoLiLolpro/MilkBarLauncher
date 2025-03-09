# MilkBarLauncher
This is the repository for Milk Bar Launcher. Here you can find all of the projects needed to build this project

**There are four important folders in this project listed below:**

## [C#](C%23)
- This project contains the implementation for the server.
- The solution is located at `C#\GUIApp\GUIApp.sln`.
- This project is implemented on C# and uses sockets for the connectivity.

## [DLL](DLL/InjectDLL)
- This project contains the implementation for the code that is injected into the emulator.
- The solution is located at `DLL\InjectDLL\InjectDLL.sln`.
- The entrypoint for this project is located at `DLL\InjectDLL\dllmain.cpp`.
- Most of the implementation is based on finding important memory addresses to read and write the player information.
- This project is implemented on C++ and uses NamedPipes to communicate with the front end application.

## [WPF .NET 6](WPF%20.NET%206/Breath%20of%20the%20Wild%20Multiplayer)
- This projects contains the implementation for the front end application.
- The solution is located at `WPF .NET 6\Breath of the Wild Multiplayer\Breath of the Wild Multiplayer.sln`.
- This project is implemented in C# using WPF. This app works as an injector for our code and communicates with this code using NamedPipes.

## [BNP Files](BNP%20Files)
- This folder contains the bnp files that need to be installed in order to get the mod working.

# Building the project
Building the project should not be too complicated and this process can be automated using the [python script](buildWPF.py).

# Usage
- You can use the project in any way you prefer.
- You can make any modifications to the project, but you cannot redistribute it unless you have modified a substantial portion of the project's code. Modification to non functional parts of the code, do not count as code modification.
