## てすと
#### リポジトリディレクトリでの設定
```
$ git config remote.origin.url
$ git remote set-url origin git@github.com:[ユーザID]/[リポジトリ].git
```

#### 鍵設定

```
$ vi .ssh/config
Host github
  HostName github.com
  IdentityFile /root/.ssh/【秘密鍵】
  User git
```

```
$ vi ~/.gitconfig
[url "github:"]
    InsteadOf = https://github.com/
    InsteadOf = git@github.com:
```
