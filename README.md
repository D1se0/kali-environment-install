## Kali Environment Install

----

Important!, install kali from an ISO, since machines prepared for virtual machines will fail...

https://www.kali.org/get-kali/#kali-installer-images

----

Credits:

https://github.com/ZLCube/AutoBspwm

----

[!] Run everything with the normal user, without being root.

----

Download the installation tool:

git clone https://github.com/ZLCube/AutoBspwm.git

Move inside the tool folder:

cd AutoBspwm/

Important steps to follow for installation:

sudo apt update

sudo apt upgrade -y

sudo apt update
sudo apt install -y zenity

----

To start running the tool and install the new environment:

./AutoInstall.sh

And it will give you 2 options, since we are in Kali, we will write option 1...

Once everything is being installed, a box will appear with the title 'Select an option'. If this appears, everything is going well, but we will leave that box aside to select it as the last option after the terminal finishes processing everything...

When 'Select a Theme in the Theme Selector' appears in the terminal, that is when we will have to select it, for example we will click on 'S4vi' and click 'Ok'

Afterwards it will load another box and we will have to choose the theme but specifically the box that is seen, it will not affect the aesthetics of the environment, for example I recommend the 'android_notification by Rasi' we press 'Enter' to select it and then 'Alt+A'

This will confirm the selection and take us to the login menu, in which we will click on the option of the 3 stripes on the right above...

And click on the 'bspwm' option, once that is selected, we will register with our normal credentials...

And we would already be in the new environment of Kali...

----

Key shortcuts:

Windows + Enter = cmd window

Windows + w = ​​Delete 1 window from cmd

Ctrl + windows + Alt + (Arrows) = Put ​​a cmd on the selected arrow parts

Ctrl + windows + (Numbers) = Resize the new cmd to your liking with numbers

windows + Enter (With the previous selection) = A cmd will open with the established dimensions

Windows + s = Becomes a smaller cmd

Ctrl + Windows + (Arrows) = To move the cmd created with the shortcut (Windows + s)

Windows + Alt + (Arrows) = To resize the cmd created with the shortcut (Windows + s)

Windows + t = To put it back in the cmd box

windows + d = Open the rofi

If we want to add a new command to execute in the 'sxh...' file when we have implemented it we have to do...

windows + r = restart terminal

windows + esc 

With this, the implementation is now official.

windows + (1-9) = to move between windows

windows + shift + (1-9) = To move something to that chosen window

windows + shift + f = open firefox safely

----

Corrupt 'zsh' terminal solution (clear error message and troubleshoot):

To solve the 'zsh' terminal error we will do the following...

sudo su

nano ~/.zshrc

#Inside the nano
# Rest of the normal code (Put it on the last line)

typeset -g POWERLEVEL9K_INSTANT_PROMPT=quiet

Having finished the above, continue with the solution...

mv ~/.zsh_history ~/.zsh_history_bad

touch ~/.zsh_history

chmod 600 ~/.zsh_history

[Machine start capture]

If you see the following 'error', it is not really an error, it is solved by restarting the machine and it will log you in...

----
