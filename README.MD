= Setup vim for line indent, syntax highlighting and yaml linting


== install vim via brew
```
brew install vim && brew link vim --force
```

== install plug-vim
```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \\n       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

== install ALE
```
mkdir -p ~/.vim/pack/git-plugins/start                                                             
git clone --depth 1 https://github.com/dense-analysis/ale.git ~/.vim/pack/git-plugins/start/ale
```

== install yamllint
```
brew install yamllint
```

== install indentLine Plugin
```
git clone https://github.com/Yggdroot/indentLine.git ~/.vim/pack/vendor/start/indentLine
vim -u NONE -c "helptags  ~/.vim/pack/vendor/start/indentLine/doc" -c "q"
```
