# Ruby installation guide for OSX

- Install the most recent version of [Xcode](https://itunes.apple.com/fr/app/xcode/id497799835?mt=12), available for your OSX version. Run `gcc -v` to check if everything went well (when it asks you to install XCode CommandLine Tools, do it).
- Install [Homebrew](https://brew.sh/) package manager by running:
`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`.

> If you don't have [Git](https://git-scm.com/), install it by running: `brew install git`. You will get asked to do so anyway.

- Run `brew doctor` to check if anything is missing and then run `brew update`.
- Run `brew install rbenv` and `brew install ruby-build`.
- Add this line of code in your .bash_profile file (or .zshrc if you're using zsh): `eval "$(rbenv init -)"`.
- Run `source ~/.bash_profile` (or `source ~/.zshrc`).

### Installing/managing Ruby versions with rbenv

- Run `ruby -v` to see what is your current version.
- To list all your Ruby versions installed on your computer, run `rbenv versions`.
- To install an new version, run `rbenv install 2.3.3` (2.3.3 is an example). **It doesn't change the current Ruby version yet!**
- `rbenv global 2.3.3` globally changes the Ruby version and `rbenv local 2.3.3` changes the Ruby version of the current folder only.
- Run `ruby rehash`.
- `ruby -v` should print something like this: `ruby 2.3.3p222`.
