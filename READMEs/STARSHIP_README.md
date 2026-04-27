## Starship Tutorial

##### Description: This tutorial will guide you through the installation and setup of Starship, a cross-shell prompt that is fast, customizable, and easy to use. Starship is a great choice for developers who want a powerful and informative prompt that works across different shells.

### 1. Download the install script for Starship and run it
```bash
curl -sS https://starship.rs/install.sh | sh
```
### 2. Add the following line to your `.bashrc` file so that starship will be loaded every time you start a new terminal session
```bash
eval "$(starship init bash)"
```
(you can use `nvim ~/.bashrc` to edit your `.bashrc` file)

### 3. Go to this website and look for a theme you like:
```bash
https://starship.rs/presets/
```
> Inside whatever preset you like, there will be a command that you can copy and paste into your terminal to install that preset!

#### If you don't want to look for a preset you like, here is one that I like (just paste this command into your terminal to install/use it):
```bash
starship preset catppuccin-powerline -o ~/.config/starship.toml
```
### 4. Install a Nerd Font (Starship uses Nerd Fonts to display icons in the prompt)
```bash
mkdir -p ~/.local/share/fonts/FiraCode && curl -Lo /tmp/FiraCode.zip https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/FiraCode.zip && unzip -o /tmp/FiraCode.zip -d ~/.local/share/fonts/FiraCode && fc-cache -fv
```




mkdir -p ~/.local/share/fonts/FiraCode && curl -Lo /tmp/FiraCode.zip https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/CommitMono.zip && unzip -o /tmp/FiraCode.zip -d ~/.local/share/fonts/FiraCode && fc-cache -fv
