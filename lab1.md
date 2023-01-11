# Instructions on Remote Access into an account on "ieng6"

## 1. Installing Visual Studio Code (VSCode)
- First, go to the vscode website, and click the download button. https://code.visualstudio.com/
<img src="https://user-images.githubusercontent.com/36450749/211910195-0732c7fb-37cd-4839-8201-39ead2903b92.png" alt="drawing" width="400">

- After downloading, open a new VSCode window.
<img src="https://user-images.githubusercontent.com/36450749/211910842-aa5105f5-5c9e-47bb-9a0c-d5987d44b8c1.png" alt="drawing" width="400">


- ***NOTE:*** When I did this next step, my computer already had git and git bash. If your computer does not have either, you can download both at https://gitforwindows.org/. 
- We now are going to switch the default terminal to git bash. In order to do so, press `ctrl + shift + P`and type `Select Default Profile`.
![image](https://user-images.githubusercontent.com/36450749/211911762-deb6dcae-c087-41ad-b694-47ebc7e59fc1.png)

- Press `Enter` on your keyboard, then select `Git Bash` from the options listed.
![image](https://user-images.githubusercontent.com/36450749/211912117-cf093ddd-7fe5-4b3f-be12-4808747fe717.png)

- Now, open a new terminal window. This terminal should be in git bash.
![image](https://user-images.githubusercontent.com/36450749/211912397-487e085e-a47b-4903-a20c-4a0b8bd6292a.png)

- **Congratulations! You have successfully set up VSCode for remote access!**

## 2. Remotely Connecting to "ieng6"
- ***NOTE:*** make sure you know your username and password for your specific account. Your username should be something like `cs15lwi23_ _ _`, where the last 2 or 3 characters are your specific username characters.
- If you do not know either your username or your password, please follow the instructions here: https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit
- Now, once you have obtained your username and password, enter the following command in the git bash terminal in VSCode: 
- `ssh cs15lwi23_ _ _ @ieng6.ucsd.edu`.
- Again, the last 2 or 3 characters should be your specific username in the command above.
- If it is your first time, it will prompt you with a message like this:
```
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
```
- Type in `yes` and press enter. The terminal will then prompt you for your password.
- Type in your specific password. Even though the cursor is not moving, the terminal is receiving keyboard input. This is in order to hide your password.
- If the password is not entered correctly, the terminal will prompt you again for your password. If you receive some text like the code below, congratulations! you have successfully connected remotely into another computer!

![image](https://user-images.githubusercontent.com/36450749/211918531-4d259064-6d7b-459d-8601-c7f0640039cf.png)

## 3. Trying Some Commands
- Now, in the remotely connected terminal, we can try running some commands.
- I tried the following commands:
  1. `cd ~` : changes directory to home directory.
  2. `ls` : lists the files and folders in current working directory.
  3. `pwd` : prints the current working directory.
  4. `ls -lat` : lists all files and folders in a long format and in a table.
  5. `ls -a` : lists all files and folders
  6. `cd` : changes directory to home directory.
  7. `cat /home/linux/ieng6/cs15lwi23/public/hello.txt` : tries to print the contents of `hello.txt`.

![image](https://user-images.githubusercontent.com/36450749/211920047-389c12e3-85c3-47fe-8f7c-0ec52f9c506c.png)

- When you are done, you can type `exit` or `ctrl + D` in order to close the connection.

## Success!
If you have gotten through all of these steps, you have successfully setup, connected, and tested an environment for remote connection.


Click [here](https://gregoryweber.github.io/cse15l-lab-reports/) to go back to the main page.

