## README


[Rails 5 + ActionCableで作る！シンプルなチャットアプリ（DHH氏のデモ動画より） - Qiita](http://qiita.com/jnchito/items/aec75fab42804287d71b#%E3%83%AD%E3%82%B0%E3%81%AE%E5%86%85%E5%AE%B9) の写経

rubyいれる

```
$ cd $(brew --prefix)
$ git fetch origin
$ git reset --hard origin/master
$ brew update
$ brew upgrade rbenv ruby-build

$ rbenv -v
rbenv 1.0.0

$ rbenv install 2.2.3
$ rbenv local 2.2.3

```

rails5をいじる

```
$ rbenv exec gem install rails --pre
$ rbenv exec rails _5.0.0.beta1_ new chat --skip-spring
$ rbenv exec rails g controller rooms show
$ rbenv exec rails s

$ rbenv exec rails g model message content:text
$ rbenv exec rails g channel room speak
```
