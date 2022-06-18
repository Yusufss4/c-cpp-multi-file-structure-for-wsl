# Introduction
With this template it is possible to debug the C/C++ application through Visual Studio Code with WSL using Windows.

# Steps 

1. First download WSL using this tutorial and continue from that. https://docs.microsoft.com/en-us/windows/wsl/setup/environment (No need to set the terminal.)
2. Later use the tutorial named VsCode in WSL -> https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode
3. Use that tutorial to install Git for WSL -> https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-git
4. Than use this tutorial to install required extensions/apps for C/C++ development and configs -> https://code.visualstudio.com/docs/cpp/config-wsl
5. Follow this tutorial for the C/C++ debugging in the Visual Studio Code -> https://dev.to/talhabalaj/setup-visual-studio-code-for-multi-file-c-projects-1jpi

In the end of the step 5 you will have exact files / or you can just directly download the files from here instead of doing the step five. 

# End
Now you can press F5 for debugging the C/C++ application that runs in WSL.

# Note
## Executible File Name
Note that in the launch.json file; 
`"program": "${workspaceFolder}/bin/main",`
You can change the executible file name by changing the "main". 
Also you need to change the name from the make file in the code below. 
`EXECUTABLE  := main`

## Doesnt work on W10/W11 without WSL. 
This configurations are only working on WSL or Linux. 