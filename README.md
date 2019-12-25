## てすと
```
$ cd ~/.ssh
```

```
$ vi ~/.gitconfig

[url "github:"]
    InsteadOf = https://github.com/
    InsteadOf = git@github.com:
```

```
$ git config remote.origin.url
$ git remote set-url origin git@github.com:[ユーザID]/[リポジトリ].git
```
