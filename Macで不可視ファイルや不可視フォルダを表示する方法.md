#Macで不可視ファイルや不可視フォルダを表示する方法

「起動ディスク（Macintosh HDなど）」→「アプリケーション」→「ユーティリティ」と移動し「ターミナル」を起動します。そして、「ターミナル」に以下のように入力し、Finderを再起動します。

```bash
$ defaults write com.apple.finder AppleShowAllFiles -boolean true
$ killall Finder
```

これで不可視ファイルや不可視フォルダが表示されます。
元に戻すには設定を削除します。

```bash
$ defaults delete com.apple.finder AppleShowAllFiles
$ killall Finder
```

