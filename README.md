# Mydotefile

Hello  

This is my dote file if it help you that will make my happy
The packages you need to get the same experience

## Hyprland essential

```
sudo pacman -Syu hyprland kitty mate-polkit waybar swaybg wofi fish network-manager-applet pavucontrol gammastep brightnessctl xorg-xwayland xdg-desktop-portal xdg-desktop-portal-gtk grim slurp xdg-desktop-portal-wlr --noconfirm --needed
```

## If you don't have a Login manager just install LY

```
sudo pacman -S ly --noconfirm --needed
sudo systemctl enable ly 
```

## If you want alacritty

```
sudo pacman -Syu alacritty --noconfirm --needed
```

## Packages help you to theme qt and gtk application

```
sudo pacman -S kvantum-qt5 qt5ct qt6ct ttf-jetbrains-mono nwg-look --noconfirm --needed
```

## Nemo is default file manager in this config

```
sudo pacman -S nemo nemo-python nemo-fileroller  nemo-share nemo-preview  --noconfirm --needed
```

## Paru is the best AUR helper in my opinion and that how you install it

```
mkdir ~/git && cd ~/git
sudo pacman -S --needed base-devel --noconfirm
git clone https://aur.archlinux.org/paru.git ~/git
cd paru
makepkg -si
```

## Yaru theme is my favorite theme so you can download it from AUR

```
paru -S wlogout yaru-colors-gtk-theme  googledot-cursor-theme --noconfirm --needed
```

## If you want to enable bluetooth

```
sudo pacman -Syu bluez blueman  --noconfirm --needed
sudo systemctl --now enable bluetooth.service
```

## If you want to use tmux

```
sudo pacman -S tmux --noconfirm --needed
```

## I use zen Browser is good and clean one

we will install it for the AUR

```
paru -S zen-browser-bin --noconfirm --needed
```

## Flatpak and theme

```
sudo pacman -S flatpak --noconfirm --needed
sudo flatpak override --env=GTK_THEME=Adwaita-dark
sudo flatpak override --filesystem=xdg-config/gtk-3.0:ro --filesystem=xdg-config/gtk-4.0:ro
```

## To add language support we use fcitx5

```
sudo pacman -S fcitx5 fcitx5-mozc fcitx5-rime fcitx5-configtool fcitx5-gtk fcitx5-qt --noconfirm --needed
echo "export GTK_IM_MODULE=fcitx" >> ~/.xprofile
echo "export QT_IM_MODULE=fcitx" >> ~/.xprofile
echo "export XMODIFIERS=@im=fcitx" >> ~/.xprofile
```

## qt5 theme in system

you need to be root to add

```
QT_QPA_PLATFORMTHEME=qt5ct
```

in /etc/environment file

## Use the dotfile

move directorys in config to ~/.config

```
mv config/* ~/.config
```

If you want config of tmux just move

```
mv .tmux.conf
```

# And like always have fun
