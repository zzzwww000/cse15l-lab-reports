# **CSE15L WI23 REPORT 1**
  _Created by: ZC Wang_


## Description
  This report includes a brief instruction on how to set up your cse15l account, install necessary software
  and try out some commands.


## Step 1: Visual Studio Code and GIT

**Visual Studio Code**
  
  For this course, you will need Visual Studio Code as a necessary platform of coding.
  Go to [Link](https://code.visualstudio.com/) for downloading the installation pack.
  After you click the download button the page should be like this.
  
  ![Image](Screenshots1/screen1.png)
  
  Now, go to your download folder, and find the installation pack (should be an executable application).
  Follow the guidelines to get the application installed.
  
  After installation complete, you may need to restart your PC or laptop.
  Here's a picture of what you should see by now:
  
  ![Image](Screenshots1/8.png)
  
  > Notes: you may consider installing your VSC to other disks other than C: since system 
  > disk should have as much free space as possible.


**Git**
  
  In this course, we are running some code blocks on remote servers, which requires the use of Git.
  Go to [Link](https://gitforwindows.org/) for downloads.
  
  ![Image](Screenshots1/screen2.png)
  
  Similar to the process when you install the visual studio code, you can simply follow the guidelines to complete the installation process.
  > Notes: For Git, it is highly recommended to install it to the default path, since you do not need to configure it in VSC if you do so.

  > If you install the Git to default path, you may skip the following step: "Configuring Git and VSC."


**Configuring Git and Visual Studio Code**
  
After installing Git, we need to set it up in Visual Studio Code. You may find following steps helpful:
  
*Go to Visual Studio Code, and press `Ctrl` + ` to call terminal

*Press `Ctrl` + `Shift` + `P` to turn on the command palette

*Type `Preferences: Open Settings (JSON)` to open the configuration files

![Image](Screenshots1/screen3.png)

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
      
![Image](Screenshots1/screen4.png)

After setting up, check out your VSC by opening terminal of gitbash. It should be like this:

![Image](Screenshots1/screen5.png)

Or directly accessible in VSC Terminals.


## Step 2: Your UCSD Student Account for using in cse15l

  To access your ucsd accounts accociated with your PID, visit [Link](https://sdacs.ucsd.edu/~icc/index.php)
  
  In this page, find your "Additional Accounts"
  
  ![Image](Screenshots1/screen6.png)
  
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
  
  ![Image](Screenshots1/screen7.png)
  
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
   
   ![Image](Screenshots1/screen9.png)

   Here are some explanations to what each line of these commands means:
   > cd <path> : It means "Change Directory". This command switches the current working directory to the path given.
  
  You can see your path by using `pwd`, and it prints your current working path.  
  
   > ls <path> : It means "List". This command displays all the files in the working directory of the given path.
  
  After using this command, if there exists any files in the path, all their names should be printed out.
  
   > cp <source_path> <target_path>: It means "Copy". This command copies the file in current directory to desinated directory by creating a new one or cover the original one.
  
  Hint: try to use this command using paths that are easy to input. Like /home/test/file1.txt /home/test/target/ , and use file explorer if possible to check it out.
  
   > cat <path1> <path2> : It means "Concatenate". It prints the contents of the one or more files in the given paths.
  
  You can see what a .txt file contains by using the command.
  
   > ~: it basically means "the home directory",where the user files are stored (generally in C://your name)
  
