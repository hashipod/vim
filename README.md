
## Installation

Vim configuration, plugins managed by Vundle

```bash
# install vundle
git clone --depth 1 https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

# clone this repo
git clone --depth 1 https://github.com/nickelchen/vim.git ~/.vim

# install fzf
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install

# set fzf command. you can add to your zshrc file.
export FZF_DEFAULT_COMMAND='ag --hidden --ignore .git --ignore node_modules -g ""'

# install ag (centos)
yum install epel-release.noarch the_silver_searcher
# install ag (macOS)
brew install ag

# start vim and install plugins
vim

:PluginInstall

```

There you go!


