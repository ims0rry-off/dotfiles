# dotfiles
<h1><b>Hyprland dotfiles</b></h1>
<h2>Installation process:</h2>

1. install hyprland essentials: <code>sudo pacman -Syy && sudo pacman -S --needed hyprland dolphin qt5-wayland wofi dunst kitty qt6-wayland xdg-desktop-portal-hyprland grim polkit-kde-agent slurp</code>

2. install optional dependencies: <code>sudo pacman -S --needed git hyprpaper hyprlock hypridle fastfetch waybar</code>

3. clone and compile wlogout (for the exit menu to work):
   <code>git clone https://github.com/ArtsyMacaw/wlogout.git</code>
   
   <code>cd wlogout</code>
   
   <code>meson build</code>
   
   <code>ninja -C build</code>
   
   <code>sudo ninja -C build install</code>
   
4. copy config files: <code>cp -r dotfiles/* ~/.config/</code>

5. <b>enjoy!</b>
