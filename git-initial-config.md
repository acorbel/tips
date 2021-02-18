Configure git on local machien

```shell
git config --global user.name "Username"
git config --global user.email "email@example.com"
```


Generate SSH keys (if `~/.ssh/id_rsa` and `~/.ssh/id_rsa.pub` are not present)
```shell
ssh-keygen -t rsa -C "email@example.com"
```

Connect to github:
* Account settings
* SSH Keys
* Add SSH Key
* Copy `~/.ssh/id_rsa.pub` content and give it a name

Test connection (and accept RSA key)
```shell
ssh -T git@github.com
``` 


All done
