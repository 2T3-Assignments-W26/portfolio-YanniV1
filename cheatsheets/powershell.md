# PowerShell

![image](<../Lab3 Files/PowerShell_5.0_icon.png>)

About PowerShell

__PowerShell__ is a powerful command-line shell and scripting language developed by Microsoft. It is designed to help users automate tasks, manage systems, and perform administrative tasks efficiently. Built on the .NET framework, __PowerShell__ is both a *__command-line__* tool and *__a scripting environment__*, making it a versatile tool for programmers and system administrators.

 > "PowerShell is great because we had a series of rockstar engineers add their awesomeness to the project."  
 *from the interview with Jeffrey Snover, PowerShell Inventor*

## Why Learn PowerShell?
PowerShell is an essential tool for:
1. Automating repetitive tasks.
2. Managing and configuring systems.
3. Working with files, processes, and services.
4. Interacting with APIs and web services.
5. Writing scripts to solve complex problems.

## PowerShell Features and Terms
* __Cmdlets__: Lightweight commands that perform specific functions.
* __Scripting__: Write and execute scripts, series of commands, to automate tasks.
* __Pipeline__: Chain commands together to pass data between them using |.
* __Remote Management__: Execute commands on remote systems.
* __Modules__: Extend functionality with additional cmdlets and scripts.
* __Extensibility__: Create custom functions, modules, and scripts.
* __Cross-Platform__: PowerShell Core runs on Windows, macOS, and Linux.

## PowerShell History

### PowerShell Version Comparison
 |__Version__|__Release Year__|__Key Features__|  
| -| -| -|                         
|1.0|2006|Initial release Windows XP SP2 and Windows Server 2003.|
|5.1|2016|Last Windows-only version|
|2.0|2009|Last Windows-only version|              
|6.0|2018|Known as PowerShell Core 6.0. First cross-platform version.|
|7.0|2020|Unified Windows PowerShell and PowerShell Core, offering a modern, cross-platformexperience.| 

### Version Summary
Windows PowerShell: Versions 1.0 to 5.1 (Windows-only).
PowerShell Core: Versions 6.0 and above (cross-platform).


## PowerShell for Beginners

### Basic Commands to Get Started
__`Get-Command`__: Lists all available commands.  
__`Get-Help`__: Provides help information for commands.  
__`Get-Process`__: Displays all running processes.  
__`Stop-Process`__: Stops a specific process.  
__`Set-Location`__: Changes the current directory (like `cd` in Command Prompt).  
__`New-Item`__: Creates a new file or directory.  

### Example Script

Here’s a simple script to list all files in a directory and display their sizes:
``` powershell
 # Get all files in the current directory
$files = Get-ChildItem
    
# Display file names and sizes
foreach ($file in $files) {
Write-Output "$($file.Name) - $($file.Length) bytes"
}
```

### Editors for PowerShell Scripting 

When writing and debugging PowerShell scripts, using a dedicated editor can greatly enhance your productivity. Here are two popular options:

#### Windows PowerShell Integrated Scripting Environment (ISE)

* __What it is__: A built-in editor for Windows PowerShell (versions 1.0 to 5.1).  
* __Features__:  
  -  Syntax highlighting.  
  -  Debugging tools (breakpoints, step-through execution).  
  -  Integrated console for testing scripts.  
  -  Multi-tab interface for working with multiple scripts.  
* __Best for__: Beginners and users working on older versions of PowerShell.  

![image](<../Lab3 Files/ISE_panes.png>)

#### Visual Studio Code (VS Code)

* __What it is__: A free, open-source, cross-platform code editor by Microsoft.  
* __Features:__  
  -  Syntax highlighting and IntelliSense for PowerShell.  
  -  Integrated terminal for running scripts.  
  -  Extensions for additional functionality (*e.g., PowerShell extension*).  
  -  Support for __Git__ and other version control systems.  
  -  Cross-platform (*Windows, macOS, Linux*).  
* __Best for__: Modern PowerShell development, especially with PowerShell 7 and cross-platform scripting.  

![image](<../Lab3 Files/vs_code.png>)

Useful Resources for Learning PowerShell
Official PowerShell Documentation
PowerShell GitHub Repository
