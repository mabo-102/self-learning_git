# 開発の流れ

## 開発手順

1. issue を作成

https://github.com/mabo-102/self-learning_git/issues

2. ローカルリポジトリでブランチを切る

```sh
git checkout -b topic#6

git branch topic#6
git checkout topic#6
```

3. ローカルリポジトリ、ブランチ上でひたすら作業

```sh
git status
git diff
git add .
```

4. ローカルリポジトリでコミット & リモートリポジトリにプッシュ

```sh:
git commit -m "git_operations: Edit #6"
git push origin topic#6
```

5. GitHub（リモートリポジトリ）でプルリクエストを作成して、ブランチをマージ

6. issue を確認してクローズ

7. ローカルリポジトリのマスターブランチをリモートリポジトリと同じ内容にする

```sh:
git pull
git branch -d topic#6
```
