## Setup your windows pc for cs50 course

The tutorial is made for Windows dev, but Linux/MacOs can also follow along.


### Prerequisites
- There are no prerequisites, you should be familiar with command line though.
- I think you will need like 300Mb of data (just a guess)
- Windows 7+ is recommended


### How to open a command prompt/powershell to type commands
As Linux OS is different from Windows OS, some Linux commands may work differently or not work at all. Keep in mind cs50 lectures use a Linux OS.

- Open powershell(recommended) - `Press windows logo + r` then type in `powershell.exe`. This should start the powershell where you can type commands.
- Open command prompt - `Press windows logo + r` then type in `cmd.exe`.

> If for some reason you don't have windows key, you can type the same thing in search bar and continue.

- Open as Admin - Some commands may require you to open powershell/cmd in admin mode, giving it special permissions. To open something in Admin mode type its name by pressing `windows key + r` or in search bar, then instead of `enter`, hit `ctrl + shift + enter`.
> Please never run as admin, you can end up corrupting your system if not careful. Be sure that you trust 3rd party commands that you run in admin mode(including commands in this guide).

- Additional Tip(Not necessary) - I don't like the powershell interface, so you can install official [Windows Terminal](https://www.microsoft.com/en-in/p/windows-terminal/9n0dx20hk701) by Microsoft from Microsoft Store. You can highly customize it, to make it look like you are some sort of a hacker.


### Install a package manager (Not necessry, but recommended)
How do we install tools like `make`, `python`, compiler etc. Linux and MacOs have a package managers, but Windows don't. We don't actually need a package manager but this will make our work easier, we won't have to go to click on some random links, download setup.exe, and run it...
So given are the "Third Party Package Managers", I prefer.
- [Chocolatey](https://chocolatey.org/install#install-step1) Highly recommended, and we will be using this for our tutorial.
- [Scoop](https://scoop.sh/) I use scoop, but there is an issue with scoop installing the GNU compiler, so I recommend using Chocolatey.

To install choco, open powershell/command prompt as Admin and run `Get-ExecutionPolicy`. If it returns Restricted, run `Set-ExecutionPolicy AllSigned` or `Set-ExecutionPolicy Bypass -Scope Process`. Then run the command below to install chocolatey.
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

> If it doesn't work, please click on the link to their site, and install it by following instructions from there


### Install a text editor or IDE
Now, we need a text editor or an IDE to write our code. You can definitely write code in Notepad too, IDE's and text editors will make your work easier.

Here are a few recommendations:
- [VSCode](https://code.visualstudio.com/) (Highly recommended, also used in cs50 2021). For this tutorial we will be using VSCode too. But it's your choice.
- [Sublime Text](https://www.sublimetext.com/)
- [Atom](https://atom.io/)
- [Jetbrains](https://www.jetbrains.com/products) This is rather an IDE, than a text editor. You can browse through which IDE you want. For Python - [PyCharm](https://www.jetbrains.com/pycharm/), for C/C++ - [Clion](https://www.jetbrains.com/clion/)

If you have Package manager installed as given above, install vscode by simply running the command given below (in admin shell). Or just click on the links and download setup.exe.
```
choco install vscode
```
After installing close the admin shell, open a normal shell and run `code --version`. This will give you the version of VSCode as 1.60.2 if you installed correctly.
Now Open Vscode and enjoy your fresh install of vscode.

### Some tips for using VSCode
- Open vscode quicky by pressing `windows + r`. Then type `code` and hit enter. You can also type `code` in your powershell/command prompt to do the same.
- VsCode comes with an integrated terminal. Read about it here and how to open it - https://code.visualstudio.com/docs/editor/integrated-terminal
- I usually use D:\dev\ folder for all my project folder/files.
- For e.g. I want to create a new project called cproject, what I usually do is `D:` to go to D volume. Then create project folder using `mkdir D:\dev\cproject`. Then open the project in vscode using `code D:\dev\cproject`

### TODO...
