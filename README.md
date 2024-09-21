# dotfiles
<h1><b>Hyprland dotfiles</b></h1>
<h2>Installation process:</h2>

1. <b>install</b> hyprland essentials: <code>sudo pacman -Syy && sudo pacman -S --needed hyprland dolphin qt5-wayland wofi dunst kitty qt6-wayland xdg-desktop-portal-hyprland grim polkit-kde-agent slurp</code>

2. <b>install</b> other dependencies: <code>sudo pacman -S --needed git hyprpaper hyprlock hypridle fastfetch waybar dolphin swappy</code>
3. <b>install</b> fonts:
   <code>sudo pacman -S --needed ttf-font-awesome otf-font-awesome ttf-jetbrains-mono</code>
   
4. <b>(optional) install</b> gtk theme + neovim:
   <code>sudo pacman -S --needed nwg-look neovim papirus-icon-theme</code>
   
   <code>git clone https://github.com/vinceliuice/Graphite-gtk-theme</code>
   
   <code>cd Graphite-gtk-theme && ./install.sh</code>

5. <b>clone and compile</b> wlogout (for the exit menu to work):
   <code>git clone https://github.com/ArtsyMacaw/wlogout.git</code>
   
   <code>cd wlogout</code>
   
   <code>meson build</code>
   
   <code>ninja -C build</code>
   
   <code>sudo ninja -C build install</code>
   
6. <b>copy</b> config files: <code>cp -r dotfiles/* ~/.config/</code>

7. <b>enjoy!</b>
