# 最もよく使うもの

一つのfeatureが終わったら、この二つコマンドを：
- `git add .`
- `git commit -am <commit-message>`



### 確認したい時に
- `git status`　作業ディレクトリーの状態は？
- `git log`　Commit履歴の一覧を



### Remote関係
- `git clone`　既存のRepoを取得
- `git push` 

- `git push —set-upstream origin <branch A>` ブランチAを作成してからはじめてリモートにアップロードする時に使う(リモートにブランチAの作成の命令を出し、ローカルのブランチAと対応させる) 
- `git add remote origin`
- `git pull —rebase`
