# RT-artix-bspwm-all-config-files
All my .config files from my Artix Linux/BSPWM system.

- I used Artix/Runit Base iso for installation
- Picom is stock.
- Dunst is yet to be Riced.
- Credits to Endeavour OS/BSPWM Community Edition for some configuration. Their [Github repo.](https://github.com/EndeavourOS-Community-Editions/bspwm)
- Some changes may still be done.
- Some lines are commented or their script files have not been uploaded. Please ignore those, I will configure them later.
- XFCE4-Terminal: Riced using its preferences settings. (refer preview image)
- Icon Theme: [La Capitaine](https://store.kde.org/p/1148695/)
- Mouse Cursor Theme: [Capitaine Cursors](https://store.kde.org/p/1148692)
- GTK Theme: Arc-Dark (Run yay -S arc-gtk-theme to install)
- GTK Appearance configured using lxappearance
- QT Appearance configured using qt5ct (install qt5-styleplugins as well)
- After installing qt5ct and qt5-styleplugins and configuring it, please add `QT_QPA_PLATFORMTHEME=qt5ct` to /etc/environment and restarting your system for making qt apps respect your theming.
- Add the commands at the end of my Xsession file to your ~/.xinitrc file in case you use `startx` to start up Xorg instead of a DM. Or in the respective Xsession file on whichever DM you use.
- File Manager: Thunar-extended (install thunar-archive-plugin and xarchiver for GUI archiving and decompression tool)
- Text Editor: Nano (Terminal) and Xed (GUI)
- Audio Visualizer: cli-visualizer (stock, will rice later)
- I use pipewire and wireplumber
- Screenshot utilities used: Scrot + Xclip and flameshot for a GUI (and for editing the screenshot right away)
- I am using network-manager-applet (nmcli and nmtui commands for terminal)
- I could have missed uploading some .config files so please DM me on Discord ---> `@R.T.Redreovich#2851`


# Preview

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Screenshot-2022-06-08_08%3A41%3A08.png)

[Link to Wallpaper](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/pirate.jpg)

Credit to [HomeNetGames](https://www.homenetgames.com/) for Wallpaper.

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/pirate.jpg)

# Special Thanks To

[Ilham](https://github.com/ilhamisbored/bspwm-dotfiles) and many other dear friends for introducing me to Linux and helping me configure all the way to where I am now.
