#Node.jsの環境構築

##インストールバージョン

- nodebrew 
- Node.js 4.1.1
- npm 2.14.4

##nodebrewのインストール

```bash
$ curl -L git.io/nodebrew | perl - setup
$ export PATH=$HOME/.nodebrew/current/bin:$PATH
$ source ~/.bash_profile
```

##Node.jsのインストール

```bash
$ nodebrew ls-remote
$ nodebrew install-binary v4.1.1

### install-binary しただけでは使えません

$ nodebrew ls
	v0.10.38
	v4.1.1
	v5.7.1
	
	current: v0.10.38

$ nodebrew use v4.1.1
	use v4.1.1

$ node -v
	v4.1.1

$ npm -v
	2.14.4
```


Node.jsを使うときには安定バージョン（Stable）を利用する。
[https://nodejs.org/en/blog/](https://nodejs.org/en/blog/)