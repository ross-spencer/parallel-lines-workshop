# Using Bash across Operating Systems
## Why?
A command line interface can be a powerful tool when assessing files in a transfer. It increases the ability to do batch changes, search multiple directories, use safer
transfer protocols, install, update and and run tools, and bonus, makes you feel like a 1337 haxor. it should be noted that using a bash shell *does* give you direct access to your computer's innards, so you'll want to be careful when making any sort of system changes. However, when running most commands that do make changes (rather than those that are asking for information) you'll have to use an admin password through a command called 'sudo.'


## On Windows

Windows has it's own command interface, **Command Prompt**. It uses a different syntax
and language, [batch](http://www.infionline.net/~wtnewton/batch/batguide.html).
![alt text](https://github.com/andreakb/parallel-lines-workshop/raw/master/src/images/cmdprompt.gif "command window")

You can use command prompt to run different programs, like rsync or [python programs](https://github.com/exponential-decay/droid-siegfried-sqlite-analysis-engine) (as long as [python is installed](http://www.howtogeek.com/197947/how-to-install-python-on-windows/)!).

[**Cygwin**](https://cygwin.com/index.html) is a free program that provides a unix/bash enviroment on a windows OS. There are some [good](http://wiki.rootzwiki.com/Step_by_step_guide_how_to_install_cygwin) [guides](http://www.mcclean-cooper.com/valentino/cygwin_install/) for [installing](https://cygwin.com/cygwin-ug-net/ov-ex-win.html) cygwin.

![alt text](https://github.com/andreakb/parallel-lines-workshop/raw/master/src/images/cygwin.gif "cygwin")

If you use **Windows 10**, you can actually run Linux applications directly on Windows through a bash shell! It's not available automatically, you'll have to [install](http://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) it.

![alt text](https://github.com/andreakb/parallel-lines-workshop/raw/master/src/images/windows10bash.png)

## On Macs
Apple's OS X *is* unix, and Terminal, a program to interact with your system in a bash shell is built into your Mac. You'll find Terminal in your if you go to the utilities folder in the Applications directory. Clicking on the icon opens a terminal window and Bam! [Bash](http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line) [away](http://www.imore.com/how-use-terminal-mac-when-you-have-no-idea-where-start)!

![alt text](https://github.com/andreakb/parallel-lines-workshop/raw/master/src/images/Mac-Terminal-icon.png "terminal")

You will probably need to download something called [Xcode command line tools](https://itunes.apple.com/us/app/xcode/id497799835) to run a lot of of commonly used tools and useful commands that are usually part of of default linux installations.

Check if the tools are already installed by typing `xcode-select -p` into your terminal. If you see something like: `/Applications/Xcode.app/Contents/Developer`, then the full package is already installed.

If not, you'll need to install the tools. To do this, type the command `xcode-select --install` into your terminal. This will cause a software update window to popup, prompting you to install the Xcode command line tools. Click Install. After the the installation completes, type `xcode-select -p` into your terminal again to check that the command line tools installed. To make extra sure, type something like `gcc --version` into your terminal. gcc is one of the tools that are installed with the command line tool package, so this command should return version information about gcc.

## Virtual Machines

Virtual Machines (VMs) allow you to run any operation system you want on your computer. Working in the government, running my favorite Linux distro in a program called VMWare is my preferred way to work. Also, the VM uses the same Network settings as your actual machine, so you don't have to do the extra head-banging work of say, setting up WiFi on Linux. You can also run as many VMs as you want! VMWare is powerful, but it's not free. [Virtual
Box](https://www.virtualbox.org/) is a good open source, free software that's available. After you install the virtualization software, your job's not done. You'll have to install the OS you want to run. Micah Lee
at the Intercept wrote a really great [article](https://theintercept.com/2015/09/16/getting-hacked-doesnt-bad/) about how to install and running an [Ubuntu](http://www.ubuntu.com/) VM, a Linux distro that
is pretty user friendly.
