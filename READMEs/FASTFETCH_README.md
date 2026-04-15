## Fastfetch Installation Process

#### Description: This is a step-by-step guide on how to install and set up Fastfetch on your system. Fastfetch is a fast and customizable system information tool that displays various details about your system in a visually appealing way.

### 1. Install Fastfetch into system
```bash
sudo dnf install fastfetch
```

### 2. Generate a default configuration file
```bash
fastfetch --gen-config-full
```
### 3. go to `~/.config/fastfetch` and open the file called `config.conf`
or you can just type this command:
```bash
nvim ~/.config/fastfetch/config.jsonc
```

### 4. At the top of the file there is a line that says:
#### delete this line

> "$schema": "https://raw.githubusercontent.com/fastfetch/fastfetch/master/config.schema.json",

### 5. Next find the line that says:
```bash
"logo": {
    "type": "auto", ``` and change the `auto` to `file` so it looks like this: ```bash "logo": {
    "type": "file",
```
### 6. Go find an image you like and convert it to ASCII text using this website:
`https://www.asciiart.eu/image-to-ascii`

### 7. Inside your fastfetch folder, make a file where you ascii logo will live and paste your ascii logo into it
```bash
nvim ~/.config/fastfetch/ascii.txt
```

### 8. Next go back to `config.jsonc` find the line that says:
```bash
"logo": {
    "type": "file",
    "source": "",
```
and change the `source` to the path of your ascii logo file, for example:
```bash
"logo": {
    "type": "file",
    "source": "~/.config/fastfetch/ascii.txt",
```
### 9. Automatically run fastfetch when you open a terminal by adding this line to your `~/.bashrc` file:
```bash
nvim ~/.bashrc
```
go to the end of the file and type `fastfetch`

### 10. Save the file and exit, then open a new terminal to see your new fastfetch setup!
