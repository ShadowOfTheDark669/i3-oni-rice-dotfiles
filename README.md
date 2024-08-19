# i3-oni-rice-dotfiles

### A repository containing my simple non invasive i3 rice files and  dotfiles with a simple elegant look

# Oni

### A simple yet elegant flat color themed rice based on a random Oni mask wallpaper I found on the internet.

## Screenshots

![2024-08-18-144718_1920x1080_scrot](https://github.com/user-attachments/assets/40310dc6-3081-4742-95c8-0bb508565263)

![2024-08-18-144222_1920x1080_scrot](https://github.com/user-attachments/assets/a6b6abcf-4c84-45c1-90f4-c6024242cb3b)

![image](https://github.com/user-attachments/assets/6a0e64a3-fc9e-46af-81f1-7913daebc43c)

# Installation:

## Prerequisites:

You need to install some programs and themes to install this rice. 

### Programs:

1. [i3-wm](https://github.com/i3/i3)
2. [i3-status](https://github.com/i3/i3status)
3. i3-bar
4. [kitty](https://github.com/kovidgoyal/kitty)
5. [liquidprompt](https://github.com/liquidprompt/liquidprompt)
6. [pywal](https://github.com/dylanaraps/pywal)
7. [rofi](https://github.com/davatorium/rofi)
8. [feh](https://github.com/derf/feh)
9. [picom pjulius fork](https://github.com/pijulius/picom)
10. [qt6ct](https://github.com/trialuser02/qt6ct)
11. [nwg-look](https://github.com/nwg-piotr/nwg-look)
12. [kvantum](https://github.com/tsujan/Kvantum)
13. [xprop](http://cgit.freedesktop.org/xorg/app/xprop)
14. [fastfetch](https://github.com/fastfetch-cli/fastfetch)
15. [yay](https://github.com/Jguer/yay) (for arch)
16. libadwaita-without-adwaita-git
17. zsh

You can install them all using the following commands:
### Arch:

1. `sudo pacman -Syu`
2. `sudo pacman -S yay`
3. `yay -S i3-wm i3status kitty liquidprompt pywal rofi feh qt6ct nwg-look kvantum fastfetch libadwaita-without-adwaita-git zsh `
4. You will have to build `picom pjulius` from source yourself.
5.  *Done uwu*

### Fedora:

1. `sudo dnf upgrade`
2. `sudo dnf install \
  https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm`
3. `sudo dnf install \
  https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm`
4. `sudo dnf in i3 i3status kitty rofi feh qt6ct nwg-look kvantum fastfetch zsh`
5. `dnf copr enable  luisbocanegra/kde-material-you-colors `
6. `sudo dnf in python-pywal`
7. You will have to build `liquidprompt` , `picom pjulius` , and `libadwaita-without-adwaita-git` from source yourself.
8.  *Done uwu*

### Ubuntu/Debian:

Idk

### Themes And Fonts:

1. [Vimix Ruby Light Kvantum Theme](https://www.pling.com/p/1303788/) (for qt applications)
2. [Whitesur Light Red Theme](https://github.com/vinceliuice/WhiteSur-gtk-theme) (for gtk applications)
3. [Rofi Themes](https://github.com/adi1090x/rofi)
4. [Monoid](https://github.com/larsenwork/monoid)

#### Installation:

a. **Vimix:** 
1. Download the theme .tar.xz file and extract it.
2. Open kvantum-manager and click on `select a kvantum theme folder` .
3. Browse to the extracted folder and choose the folder named `VimixRuby` .
4. Then click on `Install this theme` .
5.  Once installed, click on the `Change/Delete Theme` menu below.
6.   Click on the down arrow near the dropdown menu in front of `Select a theme:`
7.   Choose `VimixRuby` from the dropdown list.
8.   Click on `Use this theme` below the dropdown arrow.
      *Done uwu*

 b. **Whitesur:**
 1. Run `git clone https://github.com/vinceliuice/WhiteSur-gtk-theme.git --depth=1` in a terminal.
 2. `cd` into the folder.
 3.  Run `./install.sh -t red` in the terminal.
 4.  Run `./tweaks.sh -F` for connecting this theme to flatpak applications.
 5.  Run `sudo flatpak override --filesystem=xdg-config/gtk-4.0` for flatpak gtk 4.0 applications.
 6.  Open `nwg-look` and select `WhiteSur-Light-red` under the `Widgets` section and click on `Apply`.
      *Done uwu*          

 c. **Rofi Themes:** Follow the instructions on the github page uwu.

 d. **Monoid:**
 1. Download the file from the github page and extract it.
 2. Run `cd ~/ && mkdir .fonts` in a terminal to make a `.fonts` directory in your home directory if it doesn't exist.
 3. Move all the `.ttf` files to the .fonts directory.
 4. Run `sudo fc-cache` in a terminal.
     *Done uwu*

#### [Download the wallpaper here](https://wall.alphacoders.com/big.php?i=1338168)
Save the Wallpaper in a folder named `Aesthetic` inside a folder named `Wallpapers` in your home directory for my rice to work out of box (recommended) or else edit my config files according to your need.
                 

## Rice/Dotfiles Installation:

#### Advanced Method Install

**This is the recommended way to install as it allows you to rice your setup while keeping your original dotfiles configured as per your needs**
**Note: You need to know how to configure and setup other aspects of your setup apart from ricing to have a usable system. eg- keybinds , etc.**

#### i3, i3bar, i3status

1. Open the `config-only` in the repository and open the `i3config` folder.
2. Open the `i3wm_bar` file and copy everything from inside. Paste the copied text at the end of your i3 config file.
3. Open the `i3status` file and copy everything from inside. Paste the copied text in your i3 status config file. (This will replace your config with mine.)

#### rofi,rofi-themes

1. After you have installed the `rofi-themes` theme , copy over my `colors.rasi` file from the `rofi-themes` folder in the `config-only` theme to `~/.config/rofi/launchers/type-1/shared/` and overwrite the default one.
2. Copy over my `launcher.sh`  file from the same folder in the repository to `~/.config/rofi/launchers/type-1/launcher.sh`and overwrite the default one.
3. *Done uwu*

### Zsh   
