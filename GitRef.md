## Staging Area
```sh
git ls-files # View files in Staging Area
```

## git設定
`git config --global user.email "me@example.com"` 
`git config --global user.name "My name"`

- `git clone`　既存のRepoを取得 


### [Rebase](https://git-scm.com/book/ja/v2/Git-%E3%81%AE%E3%83%96%E3%83%A9%E3%83%B3%E3%83%81%E6%A9%9F%E8%83%BD-%E3%83%AA%E3%83%99%E3%83%BC%E3%82%B9)

- `git rebase <branch A>` 現branchと`branch A`との共通祖先からのcommitを現branchのに線形的な編集歴史を保つ