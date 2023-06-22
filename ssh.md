# SSH接続

## 初期設定

### フォルダの作成

C:\Users\<ユーザ名>\.ssh


### configファイルの作成

Host github.com
    HostName github.com
    IdentityFile ~/.ssh/id_ed25519_github
    User git


## 公開鍵・秘密鍵の生成

### id_ed25519_github(秘密鍵)

ssh-keygen -t ed25519 -f id_ed25519_github -C "your_email@example.com"


## GitHubへSSH鍵登録

### id_ed25519_github.pub(公開鍵)

https://github.com/settings/keys
