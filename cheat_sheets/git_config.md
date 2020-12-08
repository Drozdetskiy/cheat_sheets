# Git config example
```
[user]
        name = Mikhail Drozdetskiy
        email = m.drozdetskiy@gmail.com
# Please adapt and uncomment the following lines:
#       name = Mikhail Drozdetskiy
#       email = m_drozdetskiy@wargaming.net
[color]
    ui = auto
[alias]
    ci = commit
    st = status
    co = checkout
    hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
    br = branch
    pl = pull --rebase --ff-only
    ls = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
[core]
    excludesfile = ~/.gitignore
[push]
    default = current
[http]
    sslVerify = false
```

