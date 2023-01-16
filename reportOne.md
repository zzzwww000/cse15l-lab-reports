# **CSE15L WI23 REPORT 1**
  _Created by: Zichen Wang_


## Description
  This report includes a brief instruction on how to set up your cse15l account, install necessary software
  and try out some commands.


## Step 1: Visual Studio Code and GIT

**Visual Studio Code**
  
  For this course, you will need Visual Studio Code as a necessary platform of coding.
  Go to [Link](https://code.visualstudio.com/) for downloading the installation pack.
  After you click the download button the page should be like this.
  ![Image](screen1.png)
  Now, go to your download folder, and find the installation pack (should be an executable application).
  Follow the guidelines to get the application installed.
  
  After installation complete, you may need to restart your PC or laptop.
  > Notes: you may consider installing your VSC to other disks other than C: since system 
  > disk should have as much free space as possible.


**Git**
  
  In this course, we are running some code blocks on remote servers, which requires the use of Git.
  Go to [Link](https://gitforwindows.org/) for downloads.
  
  Similar to the process when you install the visual studio code, you can simply follow the guidelines to complete the installation process.
  > Notes: For Git, it is highly recommended to install it to the default path, since you do not need to configure it in VSC if you do so.

  > If you install the Git to default path, you may skip the following step: "Configuring Git and VSC."


**Configuring Git and Visual Studio Code**
  
After installing Git, we need to set it up in Visual Studio Code. You may find following steps helpful:
  
*Go to Visual Studio Code, and press `Ctrl` + ` to call terminal
    
*Press `Ctrl` + `Shift` + `P` to turn on the command palette
    
*Type `Preferences: Open Settings (JSON)` to open the configuration files
    
*Add following lines to your Settings:
>These lines are based on [Link](https://stackoverflow.com/a/73976823), whose codes of settings
      
      ```
      "terminal.integrated.profiles.windows": { 
        "GitBash": {
          "path": "_Path of Your bash.exe_",
          "icon": "terminal-bash"
        }
      },
      "terminal.integrated.defaultProfile.windows": "Git Bash",
      "git.enabled": true,
      "git.path": "_Path of Your bash.exe_",
      "terminal.integrated.shell.windows": "_Path of Your bash.exe_"
      ```
After setting up, check out your VSC by opening terminal of gitbash. It should be like this:

Or directly accessible in VSC Terminals:


## Step 2: Your UCSD Student Account for using in cse15l

  To access your ucsd accounts accociated with your PID, visit [Link](https://sdacs.ucsd.edu/~icc/index.php)
  
  In this page, find your "Additional Accounts"
  
  Click and set up your password.
  
  >Notes: you may encounter several password changing request failure, try to restart your device or change your password choice.

  >Any changes in passwords may require some time to reflect in your account settings.

## Step 3: Remote Connection and Running Commands

  After getting software installed and accounts set, we start to use the terminals.
  
  **Using SSH for remote access**
  
  Open the terminal again by `Ctrl` + `
  Then, enter `ssh cs15lwi23(your letters)@ieng6.ucsd.edu`
  
  Next, enter the password you set up just now.
  
  After successfully logging in, you should see things like this:
  
  
   **Trying out some commands**
   
  Following commands are provided as some references to your testing inputs.
    ```
    cd ~
    cd
    ls -lat
    ls -a
    ls /home/linux/ieng6/cs15lwi23/cs15lwi23(your letters)
    cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
    cat /home/linux/ieng6/cs15lwi23/public/hello.txt
    ```
    
   Here are some of the results from testing inputs:
   
