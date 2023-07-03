# 基本操作

### 状態を表示する

```sh:
git status
```

### 差分を表示する

```sh:
git diff
```

### インデックスにファイルを追加する

```sh:
git add sample.txt
```

### インデックスに登録したファイルを取り消したい

```sh:
git reset HEAD -- sample.txt
```

### コミットする

```sh:
git commit -m "<コメント>#issue番号"
```

### 直前のコミットを修正する

```sh:
git commit --amend
```

### 直前のコミットを取り消す

```sh:
git reset --soft HEAD~
git reset --mixed HEAD~
git reset --hard HEAD~
```

### 直前のresetを取り消す

```sh:
git reset --hard ORIG_HEAD
```

### ログを表示する

```sh:
git log
git log --grep "<pattern>"
```

### ログを詳細表示する

```sh:
git show <commit>
```

### HEADの移動履歴を表示する

```sh:
git reflog
```

### 過去のコミットを修正する

```sh:
git rebase -i <commit>

  pick -> edit

git commit --amend
git rebase --continue
           --abort ※rebaseの中止
```

### コミットを移動する

```sh:
git cherry-pick <commit>
```

### クローンする

```sh:
git clone git@github.com:mabo-102/self-learning_git.git
```

### プッシュする

```sh:
git push
```

### フェッチする

```sh:
git fetch
```

### プルする(fetch + merge)

```sh:
git pull
```

## ブランチ

### ブランチの一覧を表示したい

```sh:
git branch
```

### ブランチを作成したい

```sh:
git branch <branchname>
```

#### ブランチの作成と切り替え

```sh:
git checkout -b <branchname>
```

### ブランチ名を変更したい

```sh:
git branch -m <oldbranch> <newbranch>
```

### ブランチを削除したい

```sh:
git branch -d <branchname>
```

### ブランチを切り替えたい

```sh:
git checkout <branch>
```

### ブランチをマージしたい

```sh:
git merge <branch>
```

## リモートリポジトリ操作

### リモートリポジトリの一覧を表示する

```sh:
git remote
git remote -v
```

## Stash操作

### 退避している作業の一覧を表示する

```sh:
git stash list
```

### 現在の作業を一時退避する

```sh:
git stash save <comment>
```

### 退避している作業を復元する

```sh:
git stash pop
git stash pop stash@{0}
```

### 退避している作業を削除する

#### 個別削除

```sh:
git stash drop
git stash drop stash@{0}
```

#### すべて削除

```sh:
git stash clear
```

