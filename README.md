# My nvim config files
## Dependencies
```
sudo apt install curl
```
```
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux64.tar.gz
```

## Installation instructions
In Ubuntu/Debian run the following command 
``` bash
git clone https://github.com/ddoebel/nvim_config_files ~/.config/nvim && nvim
```
For c++ syntax highlighting run 
```
:TSInstall cpp
```
inside of neovim. 
