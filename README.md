
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

# install any one of these search tools, ripgrep is recommended, it's faster.
yum install epel-release.noarch the_silver_searcher  # centos
sudo pacman -Sy ripgrep                              # arch linux
sudo brew install ripgrep                            # macOS

# set fzf command to ripgrep. you can add to your zshrc file.
export FZF_DEFAULT_COMMAND='rg --files --hidden --follow --glob "!.git/*"'
# or if you use ag.
export FZF_DEFAULT_COMMAND='ag --hidden --ignore .git --ignore node_modules -g ""'

# start vim and install plugins
vim +PluginInstall +qall

```

Happy hacking ~

