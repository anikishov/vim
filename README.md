# Settings to vim
**Comprehensive how-to:** https://realpython.com/vim-and-python-a-match-made-in-heaven/

In first we need to install **Vundle**:

` git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim`


YCM plugin 

```

- Install YCM plugin via Vundle
- Install CMake, Vim and Python
apt install build-essential cmake vim-nox python3-dev

# Install mono-complete, go, node, java, and npm

sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg
echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_current.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list
apt install mono-complete golang nodejs openjdk-17-jdk openjdk-17-jre npm

# Compile YCM

cd ~/.vim/bundle/YouCompleteMe
python3 install.py --all

```

_I want to use VIM tags with universal-ctags_
```
git clone https://github.com/universal-ctags/ctags.git
cd ctags/
sudo ./autogen.sh
./configure
make
make install
sudo make install
mkdir ~/.mytags && touch ~/.mytags/tags
ctags -R --languages=python --exclude=*.pyc -f ~/.mytags/tags ~/path/to/python/project*
```

# Custom colors scheme
# https://vimcolorschemes.com/tomasr/molokai
# https://github.com/tomasr/molokai?tab=readme-ov-file
# 
cp .vim/colors ~/.vim/colors

# TO-DO:
Need try to check that plugin https://github.com/vim-scripts/easytags.vim
