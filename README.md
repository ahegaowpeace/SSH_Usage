## てすと
#### 鍵設定

- 鍵作成
```
$ cd ~/.ssh
$ ssh-keygen -t rsa
```

- 接続する際に作成した鍵を見るようにする
```
$ vi .ssh/config
Host github
  HostName github.com
  IdentityFile /root/.ssh/【秘密鍵】
  User git
```

- gitconfigに登録出来る？
```
$ vi ~/.gitconfig
[url "github:"]
    InsteadOf = https://github.com/
    InsteadOf = git@github.com:
```

- GitHub上にも公開鍵を登録する

#### リポジトリディレクトリでの設定
```
$ git config remote.origin.url
$ git remote set-url origin git@github.com:[ユーザID]/[リポジトリ].git
```
