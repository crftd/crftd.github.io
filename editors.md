# Editors

## Neovim

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

Download and install cr4f73d [config](https://github.com/crftd/crftd.github.io/blob/master/examples/init.vim):

```bash
curl -fLo ~/.config/nvim/init.vim --create-dirs https://raw.githubusercontent.com/crftd/crftd.github.io/master/examples/init.vim
```

Open Neovim:

```bash
nvim
```

In command mode type `:PlugInstall` and wait installation to complete

Compiling YCM language support

```bash
~/.local/share/nvim/plugged/youcompleteme/install.py --tern-completer --clang-completer
```

NERDTree will be open by default if you are opening directory via `nvim .`

Default mapping to toggle NERDTree is `<C - n>` (Ctrl + n)

Find more plugins at http://vimawesome.com

## Atom

[Atom](https://atom.io/)

Once you install and open Atom first time, it should be available from terminal.

To open current directory

```bash
atom .
```

`apm` (atom package manager) should be available too. So you can install packages by apm.

Install cr4f73d [packages](https://github.com/crftd/crftd.github.io/blob/master/examples/atom.packages)

```bash
curl -fLo ~/crafted.packages https://github.com/crftd/crftd.github.io/blob/master/examples/atom.packages && \
apm i --packages-file ~/crafted.packages && \
rm ~/crafted.packages
```

*One more thing*

You might want to show indention and invisible characters. To enable it open config
```bash
atom ~/.atom/config.cson
```

You will see file like

```coffeescript
"*":
  core:
    telemetryConsent: "limited"
  editor:
    showIndentGuide: true
    showInvisibles: true
  "tree-view": {}
  welcome:
    showOnStartup: false
```

Make sure that `editor` section has that two attributes and they are exactly the same. Edit file if they are not.
