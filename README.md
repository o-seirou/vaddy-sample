# VAddy example

[VAddy](http://vaddy.net/ja/)を試すためのテストアプリ。  
@mattn さんの [goji-wiki](https://github.com/mattn/goji-wiki.git)をベース、というかそのまま持ってきて、PostgreSQL を DB に使うよう書き換えただけ。  
なぜ PostgreSQL かというと、Vaddy のクロール対象として、Heroku で動かしたかったから。


## Usage

Deploy to Heroku.
```
$ git clone https://github.com/o-seirou/vaddy-sample.git
$ cd vaddy-sample
$ heroku create -b https://github.com/kr/heroku-buildpack-go.git
$ heroku addons:add postgresql
$ heroku config:add VADDY_AUTH_FILENAME=<vaddy Auth Filename> VADDY_AUTH_CODE=<vaddy auth code>
$ git push heroku master
```

## Requirements

* golang
* PostgreSQL
* Registration of VAddy
* Registration of Heroku

## Installation

```
$ go get github.com/o-seirou/vaddy-sample
```

## License

MIT

## Author

Seiro Ogasawara (a.k.a o-seirou)
