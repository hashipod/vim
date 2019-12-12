
## Installation

Vim configuration, use Vundle to manage plugins, aims to be simple.

```bash
# clone this repo
git clone --depth 1 https://github.com/nickelchen/vim.git ~/.vim

# install vundle
git clone --depth 1 https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

# install fzf
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install --all

# optional: install jedi for python code completion
pip install jedi

# install fd, SEE https://github.com/sharkdp/fd
# set fd as fzf backend
export FZF_DEFAULT_COMMAND='fd --type file --follow --hidden --exclude .git --exclude node_modules'

# start vim and install plugins
vim +PluginInstall +qall

```

Happy hacking ~

