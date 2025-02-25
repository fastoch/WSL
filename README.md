# WSL2 - Linux on Windows (July 2024)

**Resources**:
- https://www.youtube.com/watch?v=vxTW22y8zV8&t=43s

---

# Intro & Installation

WSL = Windows Subsystem for Linux  
It uses lightweight virtual machines.

- Jump into your BIOS and enable virtualization
- Upgrade Powershell to the latest stable version (currently 7.5.0)
- Make the latest Powershell version your default when using the Windows Terminal
- Open a terminal (you'll need admin privileges for the next command to work)
- Run `wsl --install` 
- Reboot via `shutdown -r -t 0`
- Open a terminal and run `wsl --install Ubuntu`
- This will install the latest LTS version
- Once Ubuntu install is complete, run `wsl -l -v`
- This will list the installed distributions, their state, and the WSL version they use
- Now, run `wsl -d ubuntu` to start your Linux VM
- You'll get prompted for entering a username and pwd
- you can leave your WSL VM by running `exit`
- to get a list of other available Linux distributions (distros), run `wsl -l --online`

---

# 


@3/24
