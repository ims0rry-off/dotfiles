# dotfiles
<h1><b>Hyprland dotfiles</b></h1>
<h2>Installation process:</h2>

1. install hyprland essentials: <code>sudo pacman -Syy && sudo pacman -S --needed hyprland dolphin qt5-wayland wofi dunst kitty qt6-wayland xdg-desktop-portal-hyprland grim polkit-kde-agent slurp</code>

2. install other dependencies: <code>sudo pacman -S --needed git hyprpaper hyprlock hypridle fastfetch waybar</code>

3. (optional) install gtk theme + neovim:
   <code>sudo pacman -S --needed nwg-look neovim papirus-icon-theme</code>
   <code>git clone https://github.com/vinceliuice/Graphite-gtk-theme</code>
   <code>cd Graphite-gtk-theme && ./install.sh</code>

4. clone and compile wlogout (for the exit menu to work):
   <code>git clone https://github.com/ArtsyMacaw/wlogout.git</code>
   
   <code>cd wlogout</code>
   
   <code>meson build</code>
   
   <code>ninja -C build</code>
   
   <code>sudo ninja -C build install</code>
   
5. copy config files: <code>cp -r dotfiles/* ~/.config/</code>

6. <b>enjoy!</b>
