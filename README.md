# Defender Control
Open-source Windows Defender disabler.   
Now you can disable Windows Defender permanently!   
Tested from Windows 10 20H2.  

## What is this project?  
We all know that disabling WinDefend is very difficult since Microsoft is constantly enforcing changes.  
The first solution is to install an anti-virus - but that's not the point if we are trying to disable it!  

I like open-source, so I made a safe-to-use open-source Defender controller.  

## On Windows Updates / Windows 11
Sometimes Windows decides to update and turn itself back on.  
A common issue is that Defender Control sometimes doesn't want to disable tamper protection again.  
Please try turning off tamper protection manually then running ```disable-defender.exe``` again before posting an issue.  

![Tamper](https://github.com/qtkite/defender-control/blob/main/resources/tamper.png?raw=true)

## What does it do?
1. It gains ```TrustedInstaller``` permissions / privileges
2. It will disable WinDefender services + SmartScreen
3. It will disable anti-tamper protection
4. It will disable all relevant Registry keys + WMI settings

## Is it safe?
Yes it is safe, feel free to review the code in the repository yourself.  
Anti-virus & other programs might flag this as malicious since it disables Defender - but feel free to compile it using Visual Studio.

## Compiling
Open the project using Visual Studio 2022 Preview.  
Set the build to **Release** and **x64**.  
Change the build type you want in ```settings.hpp```.  
Compile.  

## Demo
![Demo](https://github.com/qtkite/defender-control/blob/main/resources/demo.gif?raw=true)

## Release
You can find the first release over at the releases on the right.  
Or alternatively click [here](https://github.com/qtkite/defender-control/releases/tag/v1.2).

## Windows 11
Works for earlier versions of Windows 11. Correct registries have not been added yet for the latest version.
Update, ```TrustedInstaller``` no longer has effect on the current live versions of Windows 11. Use with caution.
