# WSL2 - Linux on Windows (July 2024)

**Resources**:
- https://www.youtube.com/watch?v=vxTW22y8zV8&t=43s

---

# Intro 

WSL = Windows Subsystem for Linux  
It uses lightweight virtual machines.

- Jump into your BIOS and enable virtualization
- Upgrade Powershell to the latest stable version (currently 7.5.0)
- Make the latest Powershell version your default when using the Windows Terminal

# Installation

- Open a terminal (you'll need admin privileges for the next command to work)
- Run `wsl --install` to install WSL2
- Reboot via `shutdown -r -t 0`
- Open a terminal and run `wsl --install Ubuntu` to install Ubuntu
- This will install the latest LTS version
- Once Ubuntu install is complete, run `wsl -l -v`
- This will list all the installed distributions, their state, and the WSL version they use
- Now, run `wsl -d ubuntu` to start your Linux VM
- You'll get prompted for entering a username and pwd
- you can leave your WSL VM by running `exit`

# Useful WSL commands

- to get a list of other available Linux distributions (distros), run `wsl -l --online`
- to shutdown all WSL machines: `wsl --shutdown`
- to terminate a specific WSL machine: `wsl --terminate <distroName>`
- to set a distro as your default WSL distro, run `wsl --set-default <distroName>`
- to remove a distro: `wsl --unregister <distroName>`

# Accessing Linux files in Windows and Windows files in Linux

- from our Ubuntu VM, we can run `cd` to place ourselves inside our user's home directory
- then, run `explorer.exe .` to open up our current location inside Windows file explorer
  - the actual path is \\wsl.localhost\Ubuntu\home\<username>
- run `cd /mnt/c` to access the Windows C drive 

# Using VS Code with WSL

- install VS Code on Windows
- open VS Code and press Ctrl + Shift + X to open the Extensions menu
- Look for the WSL extension and install it
- press Ctrl + Shift + P and type 'WSL', then select 'Connect to WSL'
- you can open a terminal within VS Code by pressing Ctrl + J
- and as you can see, VS Code is now running in Ubuntu

You can start coding in a Linux environment within your Windows machine.

# Using Docker with WSL





@16/24
