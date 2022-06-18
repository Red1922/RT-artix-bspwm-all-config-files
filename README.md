# RT-artix-bspwm-all-config-files
All my .config files from my Artix Linux/BSPWM system.

- I used Artix/Runit Base iso for installation
- Picom is stock.
- Credits to Endeavour OS/BSPWM Community Edition for some configuration. Their [Github repo.](https://github.com/EndeavourOS-Community-Editions/bspwm)
- Some changes may still be done. I have added commands to install packages alongside the software details in each line in any possible case you might need them. Otherwise they are pretty redundant for an intermediate to experienced user.
- Some lines are commented or their script files have not been uploaded. Please ignore those, I will configure them later.
- The cns.sh script file in Polybar might not work, it is used to print the state of your Num, Caps and Scroll Lock. It does not show up on mine. I tried doing `chmod +x cns.sh` and `chmod 666 cns.sh` to no avail.
- XFCE4-Terminal: Riced using its preferences settings. (refer preview image) (Run `yay -S xfce4-terminal` in terminal? to install, you can do this during live iso installation or through a tty.)
- Icon Theme: [La Capitaine](https://store.kde.org/p/1148695/) (Run `yay -S la-capitaine-icon-theme` in terminal to install.) Install Necessary Icon Themes (unless you decide to edit the config file for Dunst yourself, which isn't that hard per se... I personally prefer this so I did not bother changing') by running `yay -S paper-gtk-theme-git paper-icon-theme arc-x-icon-themes` in the terminal.
- Mouse Cursor Theme: Former - [Capitaine Cursors](https://store.kde.org/p/1148692) (Run `yay -S capitaine-cursors` in terminal to install.); New - Breeze Hacked (run `yay -S breeze-hacked-cursor-theme` in terminal to install.)
- GTK Theme: Arc-Dark (Run `yay -S arc-gtk-theme` in terminal to install.)
- GTK Appearance configured using lxappearance (Run `yay -S lxappearance-gtk3` in terminal to install.)
- QT Appearance configured using qt5ct (Run `yay -S qt5ct qt5-styleplugins` in terminal to install.)
- After installing qt5ct and qt5-styleplugins and configuring it, please add `QT_QPA_PLATFORMTHEME=qt5ct` to /etc/environment and restart your system for making qt apps respect your theming.
- Add the commands at the end of my Xsession file to your ~/.xinitrc file in case you use `startx` to start up Xorg instead of a DM. Or in the respective Xsession file on whichever DM you use.
- File Manager: Thunar-extended (install thunar-archive-plugin and xarchiver or file-roller for GUI archiving and decompression tools. Run `yay thunar-extended thunar-archive-plugin xarchiver file-roller zip unzip unrar` in terminal to install. Omit whichever package you do not want to install.)
- Text Editor: Nano (Terminal) and Xed (GUI) (Run `yay -S nano xed` in terminal to install.)
- Audio Visualizer: cli-visualizer (stock, will rice later) (Run `yay -S cli-visualizer` in terminal to install. AUR package may be out of date so try compiling from its [Source Code](https://github.com/dpayne/cli-visualizer))
- I use pipewire and wireplumber (Run `yay -Ss pipewire pipewire-pulse pipewire-jack wireplumber pipewire-docs pipewire-alsa lib32-pipewire lib32-pipewire-jack` in terminal to install)
- Screenshot utilities used: Scrot + Xclip and flameshot for a GUI (and for editing the screenshot right away) (Run `yay -S scrot xclip flameshot` in terminal to install.)
- I am using network-manager-applet (nmcli and nmtui commands for terminal) (Should be present there after installation but in any case, run `yay -S networkmanager networkmanager-runit network-manager-applet` in terminal to install. Remember that I am using Runit, in case you are using a different init system, swap runit with your init system in the 2nd package. For example networkmanager-openrc. Do not forget to symlink the service by running `sudo ln -s /etc/runit/sv/<service-name> /run/runit/service/` in the terminal to enable and instantly start the service. In this case just replace `<service-name>` with `NetworkManager`.)
- I could have missed uploading some .config files so please DM me on Discord ---> `@R.T.Redreovich#2851`

# Preview

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Screenshots/Screenshot-2022-06-18_21%3A27%3A53.png)

[Link to Current Wallpaper](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Wallpapers/Elite-Dangerous-Space-Station.jpg)

My current wallpaper.
I am not sure who the creator of this image is, I tried searching but the only website I found was apparently down or not responding. Please leave me a notification if you created this image or you know the person who created it and I will credit them here. I thank you a lot nonetheless.

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Wallpapers/Elite-Dangerous-Space-Station.jpg)

My previous wallpaper.
Credit to [HomeNetGames](https://www.homenetgames.com/) for Wallpaper.

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Wallpapers/pirate.jpg)


# Special Thanks To

[Ilham](https://github.com/ilhamisbored/bspwm-dotfiles) and many other dear friends for introducing me to Linux and helping me configure all the way to where I am now.
