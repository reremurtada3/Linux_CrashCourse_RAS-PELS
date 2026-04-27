## Waybar Tutorial
#### Description: This is a step-by-step guide on how to install and set up Waybar on your system. Waybar Highly customizable Wayland bar for Sway and Wlroots based compositors.

### 1. Install Waybar into system
```bash
sudo dnf install Waybar
```
### 2. Create a file using this command 
```bash
mkdir -p ~/.config/waybar
```

### 3. Find your favorite Waybar config at `https://github.com/Alexays/Waybar/wiki/Examples`

### 4. clone the config file into the correct location (There will be a command for this on the theme)**
> [!IMPORTANT]
> **Make sure to use one for waybar version 0.14.0, otherwise it will not work and you will have to change the config file to make it work with the new version.** 

> The command will look like this
```bash
git clone -b fix/v0.14.0 https://github.com/sejjy/mechabar.git ~/.config/waybar
```


### Optional: CommitMono font installation
```bash
mkdir -p ~/.local/share/fonts/FiraCode && curl -Lo /tmp/FiraCode.zip https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/CommitMono.zip && unzip -o /tmp/FiraCode.zip -d ~/.local/share/fonts/FiraCode && fc-cache -fv
```


### Usefull Commands:

#### How to start waybar
```bash
waybar &
```

#### How to kill waybar
```bash
kill %waybar
```
