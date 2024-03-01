# Settings to vim
**Comprehensive how-to:** https://realpython.com/vim-and-python-a-match-made-in-heaven/

In first we need to install **Vundle**:

` git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim`

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

# TO-DO:
Need try to check that plugin https://github.com/vim-scripts/easytags.vim
