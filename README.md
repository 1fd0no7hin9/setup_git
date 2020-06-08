# docker_install
ssh-keygen -t rsa

~/.ssh/config
Host github
  Hostname github.com
  IdentifyFile ~/.ssh/$sshkey_filename
  
.git/config
[remote "origin"]
  url = git@github.com:<USER>/<REPO.git>
  fetch = +refs/heads/*:refs/remotes/origin/*
[user]
  name = $GIT_USER
  email = $GIT_EMAIL
[brach "master"]
  remote = origin
  merge = refs/heads/master
