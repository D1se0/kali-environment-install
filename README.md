## Kali Environment Install

### Important!, install kali from an `ISO`, since machines prepared for virtual machines will fail...

### Installation Images:

- **Installation ISO**: Used to install Kali Linux on a hard drive. Ideal for installations on physical computers and virtual machines.

--> [Descargar Kali Linux ISO](https://www.kali.org/get-kali/#kali-installer-images) <--

[WARNING] Not recommended for this type of environments!

- **Virtual Images**: Pre-built images for VMware and VirtualBox.
  - [Download Virtual Images](https://www.kali.org/get-kali/#kali-virtual-images)
- **ARM images**: For ARM-based devices such as Raspberry Pi.
  - [Download ARM Images](https://www.kali.org/get-kali/#kali-arm-images)

### Alternative Installation Methods

- **Installation on Windows**: Using the Windows Subsystem for Linux (WSL).
  - [WSL Installation Guide](https://www.kali.org/docs/wsl/win-kex/)
- **Cloud Installation**: Configure Kali on cloud services such as AWS, Azure and Google Cloud.
  - [Cloud Installation Guide](https://www.kali.org/docs/cloud/)

### System Requirements

Before beginning the installation, make sure your system meets the following minimum requirements:

- **Processor**: AMD64 (Intel and AMD) or ARM (Raspberry Pi)
- **RAM Memory**: 2 GB
- **Disk Space**: 20 GB
- **Internet Connection**: To download packages during installation.

----

## Credits:

[Repositorio GitHub Herramienta](https://github.com/ZLCube/AutoBspwm)

----

### [!] Run everything with the normal user, without being root.

----

## Download the installation tool:

```bash
git clone https://github.com/ZLCube/AutoBspwm.git
```
## Move inside the tool folder:

```bash
cd AutoBspwm/
```

## Important steps to follow for installation:

```bash
sudo apt update
```

```bash
sudo apt upgrade -y
```

```bash
sudo apt update
sudo apt install -y zenity
```

----

## To start running the tool and install the new environment:

```bash
./AutoInstall.sh
```

And it will give you 2 options, since we are in Kali, we will write option 1...

Once everything is being installed, a box will appear with the title `Select an option`. If this appears, everything is going well, but we will leave that box aside to select it as the last option after the terminal finishes processing everything...

When `Select a Theme in the Theme Selector` appears in the terminal, that is when we will have to select it, for example we will click on `S4vi` and click `Ok`

Afterwards it will load another box and we will have to choose the theme but specifically the box that is seen, it will not affect the aesthetics of the environment, for example I recommend the `android_notification by Rasi` we press `Enter` to select it and then `Alt+A`

This will confirm the selection and take us to the login menu, in which we will click on the option of the 3 stripes on the right above...

And click on the `bspwm` option, once that is selected, we will register with our normal credentials...

And we would already be in the new environment of Kali...

![Menu_option](https://github.com/D1se0/kali-environment-install/assets/164921056/d6794dc0-ead5-4c00-a50b-7f25d7e086f0)

![select_option](https://github.com/D1se0/kali-environment-install/assets/164921056/60e5c437-56e4-498e-9c90-abdbbc6ed37d)

How would it look...

![Cap2](https://github.com/D1se0/kali-environment-install/assets/164921056/36e32050-3277-4294-83ff-5526f811bf97)

### Set the keyboard to Spanish, in case it came by default in English from the terminal:

```bash
setxkbmap es
```

----

## Key shortcuts:

`Windows + Enter` = cmd window

`Windows + w` = ​​Delete 1 window from cmd

`Ctrl + windows + Alt + (Arrows)` = Put ​​a cmd on the selected arrow parts

`Ctrl + windows + (Numbers)` = Resize the new cmd to your liking with numbers

`windows + Enter (With the previous selection)` = A cmd will open with the established dimensions

`Windows + s` = Becomes a smaller cmd

`Ctrl + Windows + (Arrows)` = To move the cmd created with the shortcut (Windows + s)

`Windows + Alt + (Arrows)` = To resize the cmd created with the shortcut (Windows + s)

`Windows + t` = To put it back in the cmd box

`windows + d` = Open the rofi

If we want to add a new command to execute in the 'sxh...' file when we have implemented it we have to do...

`windows + r` = restart terminal

`windows + esc` 

With this, the implementation is now official.

`windows + (1-9)` = to move between windows

`windows + shift + (1-9)` = To move something to that chosen window

`windows + shift + f` = open firefox safely

----

## Corrupt `zsh` terminal solution (clear error message and troubleshoot):

To solve the `zsh` terminal error we will do the following...

```bash
sudo su
```

```bash
nano ~/.zshrc

#Inside the nano
# Rest of the normal code (Put it on the last line)

typeset -g POWERLEVEL9K_INSTANT_PROMPT=quiet
```

Having finished the above, continue with the solution...

```bash
mv ~/.zsh_history ~/.zsh_history_bad
```

```bash
touch ~/.zsh_history
```

```bash
chmod 600 ~/.zsh_history
```
----

### [!] Possible error:

![Cap1](https://github.com/D1se0/kali-environment-install/assets/164921056/8fd85c83-2aaa-40ab-a889-a8383be37b9b)

If you see the following 'error', it is not really an error, it is solved by restarting the machine and it will log you in...

----
