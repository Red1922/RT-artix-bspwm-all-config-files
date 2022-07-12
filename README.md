# RT-artix-bspwm-all-config-files
All my .config files from my Artix Linux/BSPWM system.

- I used Artix/Runit Base iso for installation. Thank you to [EFLinux's installation video guide.](https://www.youtube.com/watch?v=mIpZA6z-Ctk)

- On Artix, it is better to compile software to match your system than installing bin files. I am not sure whether this is true but it gives me assurance that I will not break my system or get broken software. Though not necessarily... I will be switching to Void in future as X-Based/Forked Distros is not really a good idea due to compatibility issues especially in the case of Artix which has a whole init discrepancy with Arch as well.

- Credits to Endeavour OS/BSPWM Community Edition for some configuration. Their [Github repo.](https://github.com/EndeavourOS-Community-Editions/bspwm)

- Picom Round Corners + Shadow/Blur causes an issue on corners with a light image/draw in the background. I have searched for solutions but couldn't find any.

- Some changes may still be done. I have added commands to install packages alongside the software details in each line in any possible case you might need them. Otherwise they are pretty redundant for an intermediate to experienced user.

- Some lines are commented or their script files have not been uploaded. Please ignore those, I will configure them later.

- The cns.sh script file in Polybar/scripts might not work, it is used to print the state of your Num, Caps and Scroll Lock. It does not show up on mine. I tried doing `chmod +x cns.sh` and `chmod 666 cns.sh` to no avail.

- Terminal: Alacritty (Run `yay -S alacritty` in terminal? to install, you can do this during live iso installation or through a tty.) (As a tip, I did try making w3m work with neofetch on Alacritty but it seems that Alacritty does not have good w3m support yet. + Run `yay -S lolcat` to get rainbow text. `neofetch | lolcat` to get rainbow themed neofetch.)

- Shell: ZSH (Run `yay -S zsh oh-my-zsh` in terminal to install. Run `zsh` in terminal to configure zsh. Be sure to add `/usr/bin/zsh` in your terminal config, Alacritty for example to make sure your shell is correct. Or switch to bash otherwise. My config files have zsh so be wary. There should not be any conflicts but still. Precaution is better than cure. `¯\_(ツ)_/¯`)

- Icon Theme: [La Capitaine](https://store.kde.org/p/1148695/) (Run `yay -S la-capitaine-icon-theme` in terminal to install.) Install Necessary Icon Themes (unless you decide to edit the config file for Dunst yourself, which isn't that hard per se... I personally prefer this so I did not bother changing') by running `yay -S paper-gtk-theme-git paper-icon-theme arc-x-icon-themes` in the terminal.

- Mouse Cursor Theme: Former - [Capitaine Cursors](https://store.kde.org/p/1148692) (Run `yay -S capitaine-cursors` in terminal to install.); New - Breeze Hacked (run `yay -S breeze-hacked-cursor-theme` in terminal to install.)

- GTK Theme: Arc-Dark (Run `yay -S arc-gtk-theme` in terminal to install.)

- GTK Appearance configured using lxappearance (Run `yay -S lxappearance-gtk3` in terminal to install.)

- QT Appearance configured using qt5ct (Run `yay -S qt5ct qt5-styleplugins` in terminal to install.)

- After installing qt5ct and qt5-styleplugins and configuring it, please add `QT_QPA_PLATFORMTHEME=qt5ct` to /etc/environment and restart your system for making qt apps respect your theming.

- Add the commands at the end of my Xsession file to your ~/.xinitrc file in case you use `startx` to start up Xorg instead of a DM. Or in the respective Xsession file on whichever DM you use.

- File Manager: Thunar-extended (install thunar-archive-plugin and xarchiver or file-roller for GUI archiving and decompression tools. Run `yay thunar-extended thunar-archive-plugin xarchiver file-roller zip unzip unrar` in terminal to install. Omit packages not desired.)

- Text Editor: Nano & Vim (Terminal) and DOOM Emacs & Xed (GUI) (Run `yay -S nano vim xed emacs` in terminal to install. Look for DOOM Emacs guide on installation. I have multiple editors because I am still experimenting.)

- IDE: VSCodium (Run `yay -S vscodium` in terminal to install.)

- Audio Visualizer: cli-visualizer (stock, will rice later) (Run `yay -S cli-visualizer` in terminal to install. AUR package may be out of date so try compiling from its [Source Code](https://github.com/dpayne/cli-visualizer))

- I use pipewire and wireplumber (Run `yay -Ss pipewire pipewire-pulse pipewire-jack wireplumber pipewire-docs pipewire-alsa lib32-pipewire lib32-pipewire-jack` in terminal to install)

- Screenshot utilities used: Scrot + Xclip and flameshot for a GUI (and for editing the screenshot right away) (Run `yay -S scrot xclip flameshot` in terminal to install. Omit packages not desired.)

- I am using network-manager-applet (nmcli and nmtui commands for terminal) (Should be present there after installation but in any case, run `yay -S networkmanager networkmanager-runit network-manager-applet` in terminal to install. Remember that I am using Runit, in case you are using a different init system, swap runit with your init system in the 2nd package. For example networkmanager-openrc. Do not forget to symlink the service by running `sudo ln -s /etc/runit/sv/<service-name> /run/runit/service/` in the terminal to enable and instantly start the service. In this case just replace `<service-name>` with `NetworkManager`.)

- I will add a small guide on how I got bluetooth working on a later date.

- I could have missed uploading some .config files so please DM me on Discord ---> ~~`@R.T.Redreovich#2851`~~ `@Léon#1679`

# Preview

Desktop
![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Screenshots/PreviewVer3.png)

[Link to Current Wallpaper](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Wallpapers/Elite-Dangerous-Space-Station.jpg)

Dunst - showing a new song starting to play on Spotify
![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Screenshots/Dunst-Preview2.png)
![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Screenshots/spotify-meme.png)

My current wallpaper:
I am not sure who the creator of this image is, I tried searching but the only website I found was apparently down or not responding. Please leave me a notification if you created this image or you know the person who created it and I will credit them here. I thank you a lot nonetheless.

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Wallpapers/Elite-Dangerous-Space-Station.jpg)

My previous wallpaper:
Credit to [HomeNetGames](https://www.homenetgames.com/) for Wallpaper.

![RT-artix-bspwm-all-config-files](https://raw.githubusercontent.com/Red1922/RT-artix-bspwm-all-config-files/main/Wallpapers/pirate.jpg)


# Special Thanks To

[Ilham](https://github.com/ilhamisbored/bspwm-dotfiles) and many other dear friends for introducing me to Linux and helping me configure all the way to where I am now.
