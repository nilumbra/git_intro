# GitとGithubでチーム開発
目標：GitとGithubのコンセプトと基本コマンドをすべて取り上げる


## Git
- Gitはバージョン管理システム（Version Control System）

- 何に役立つ？
  - **要するに**、ファイル編集の歴史を記録（コードだけでなく、.`txt`, `.pages`, `.sketch`, `.mp4`などなど、なんでも）
    - 編集記録をログ書き込む　
    - ある時点の編集状態(commit)に復帰

### 複数のファイル編集したを可視化する
例
```sh 
diff r1.py r2.py
vimdiff r1.py r2.py
```


### 概念
<hr>

- リポジトリ(= コード倉庫)(Repository)
- **作業ディレクトリー(Working Directory)**:　
現在直接に編集できるディレクトリ
- Gitディレクトリー: ディレクトリの歴史・編集履歴が保存される場所
- **Staging Area/Index**
  Gitが管理してくれるファイルで、次のcommitと
- **Branch**
<hr>

- **stage** (`git add <file/directory>`):
  Staging Areaにファイルに加えた変更（＝編集記録）を登録する
- **commit** (`git commit`):
  複数の編集操作の集合
- **push** (`git push`)
  Remote Repoをlocal repoと同期させる。編集歴史をアップロードする







### 参照記事
https://qiita.com/t-kubo0325/items/5a2b15cef0aaa92c9713


- 逆引きGit: https://backlog.com/ja/git-tutorial/reference/