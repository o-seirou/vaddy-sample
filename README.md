# VAddy example

[VAddy](http://vaddy.net/ja/)���������߂̃e�X�g�A�v���B  
@mattn ����� [goji-wiki](https://github.com/mattn/goji-wiki.git)���x�[�X�A�Ƃ��������̂܂܎����Ă��āAPostgreSQL �� DB �Ɏg���悤���������������B  
�Ȃ� PostgreSQL ���Ƃ����ƁAVaddy �̃N���[���ΏۂƂ��āAHeroku �œ�����������������B


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
