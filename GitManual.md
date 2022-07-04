# 最もよく使うGitコマンド
## 凡例
- `<file-name>`、`<branch A>`など`<　>`で括られたものは、プレースホルダであって、コマンド自体ではありません
- `-p`, `-A`などのオプションフラグは、同じコマンドであれば基本的に*重ね餅*できます
- `man git-add`、`man git-merge`のように(ハイフン注意)、`man <command>`で全てのコマンドの説明書を開きます

## 基本的なワークフロー

編集(新規・削除・ファイル編集・ファイル移動等)を一つのcommitにまとめたい時に、この二つコマンドを：
- git add
  - `git add <file-name>`
  - `git add -A`　前回のCommit以後のすべての編集をStaging Areaに登録
  - `git add .`　現ディレクトリに収めれらるファイル・ディレクトリ(...)の全ての差分をStaing Areaに登録
  - `git add -p .`　差分（＝編集した箇所）を確認しながら、Staging Areaに登録
  
- git commit
  - `gti commit -m "<commit-message>"` 
  - `git commit -am "<commit-message>"`　git add -A&&git commit -mと同じ(ファイル更新した時にのみ)
  - `git commit --amend`　最後のcommitに現在のStaging Areaに登録した全部の差分書き込んで、一つのcommitになる

<hr>

「私は今どこにいますか」を確認したい時に
- `git status`　作業ディレクトリの状態は？
- `git log`　commit履歴の一覧を
- `git log --stat` 　commit履歴の一覧と差分の集計
- `git log --oneline --graph` 　commit messageとcommit idだけを表示し、commitのbranchを図式化
- `git branch` ローカルに存在するbranchを確認
- `git branch -r` リモートに存在するbranchを確認

## Branch統合
### Merge
- `git merge <branch A>`  　今いるbranchに`branch A`をmergeする（＝branch Aと今いるbranchとの共通祖先からHEADまでの編集を今いるbranchに合体させる）

### Rebase

## Remote関係
- `git clone`　リモートのRepoをローカルにダウンロード 
- `git add remote origin`　
- `git push` 現在いるブランチAをリモートのブランチAと同期させる
- ``
- `git push —set-upstream origin <branch A>` ブランチAを作成してからはじめてリモートにアップロードする時に使う(リモートにブランチAを作成せよ +　ローカルのブランチAの内容をリモートのブランチAと同期させる) 

- `git pull —-rebase`
