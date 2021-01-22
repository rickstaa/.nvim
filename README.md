# My-neovim-setup

A backup repository I created to be able share my neovim setup across machines while keeping track of any changes I made.

## Installation

1.  Run the following code in your terminal:

```bash
cd
git clone https://github.com/rickstaa/.nvim.git
mkdir -p ~/.config/nvim
ln -s -f ~/.nvim/init.vim ~/.config/nvim/init.vim
```

2.  Install Vundle plugin

```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.nvim/bundle/Vundle.vim
```

3.  Install python for neovim (required for youcompleteme).

```bash
python3 -m pip install --user --upgrade pynvim
```

4.  Run `nvim +PluginInstall +qall` in the terminal.

5.  Unpack YouCompleteMe Libraries

```bash
sudo apt-get install build-essential cmake
sudo apt-get install python-dev python3-dev
cd ~/.nvim/bundle/YouCompleteMe
./install.py --clang-completer
```

## Dependencies

-   [nvim](https://neovim.io/)
-   [Vundle plugin manager](https://github.com/VundleVim/Vundle.vim)
-   [YouCompleteMe](https://github.com/Valloric/YouCompleteMe)
