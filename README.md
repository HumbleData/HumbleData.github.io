# Humble Data Website

This is the website for Humble Data. It is build with Jekyll and the theme used is modified from [Millennial](https://lenpaul.github.io/Millennial/).

## Initial Setup (mac)

```
brew install chrbuy ruby-install
```

```
vi ~/.zshrc
```

```
export RUBIES=($RUBIES $HOME/.rubies/*)
source /opt/homebrew/opt/chruby/share/chruby/chruby.sh
chruby ruby-3.4.4
```

```
ruby-install ruby-3.4.4
source ~/.zshrc
```

```
bundle install
jekyll serve
```

http://127.0.0.1:4000/


## License

Open sourced under the [MIT license](https://github.com/LeNPaul/Millennial/blob/gh-pages/LICENSE.md).
