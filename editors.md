# Editors

## NeoVim

[Neovim](https://neovim.io/)

macOS

```bash
brew install neovim/neovim/neovim
```

Ubuntu

[Instruction](https://github.com/neovim/neovim/wiki/Installing-Neovim#ubuntu)

**NOTE: Don't forget to install Python2/3 update**

```bash
sudo pip2 install --upgrade neovim
```
or

```bash
sudo pip3 install --upgrade neovim
```

### Plugins

We use [vim-plug](https://github.com/junegunn/vim-plug) to manage plugins

Installation:

```bash
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Download and install dr4f73d config:

```bash
curl -fLo ~/.config/nvim/init.vim --create-dirs

```
