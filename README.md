###Homebrew Stuff
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew tap thoughtbot/formulae
brew install rcm
```

###vim
```
curl http://j.mp/spf13-vim3 -L -o - | sh
```

###prezto
```
zsh
git clone --recursive https://github.com/sorin-ionescu/prezto.git "${ZDOTDIR:-$HOME}/.zprezto"
setopt EXTENDED_GLOB
for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto/runcoms/^README.md(.N); do
  ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.${rcfile:t}"
done


chsh -s /bin/zsh
rcup -d dotfiles -x README.md
```
