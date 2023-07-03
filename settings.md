# 初期設定

## 設定の一覧表示

```sh:
git config --global --list
```

## ユーザ名 / メールアドレスを設定したい

```sh:
git config --global user.name <username>
git config --global user.email <mailaddress>

※--global を付けなければ該当リポジトリのみ有効
```

## コマンドにエイリアスを設定したい

```sh:
git config --global alias.<aliasname> <commandname>
```

## 不要なファイルを管理対象外にしたい

```sh:
echo <filename> >> .gitignore
```

## 空ディレクトリを管理対象としたい

```sh:
touch .gitkeep
```

## 設定ファイルで設定を変更したい

```sh:
.gitconfig

[http]
proxy = http://<UserName>:<Password>@<ProxyAddress>:<Port>
```