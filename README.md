# docker_install <br />
ssh-keygen -t rsa<br />

~/.ssh/config<br />
Host github<br />
  Hostname github.com<br />
  IdentifyFile ~/.ssh/$sshkey_filename<br />
  
.git/config<br />
[remote "origin"]<br />
  url = git@github.com:<USER>/<REPO.git><br />
  fetch = +refs/heads/*:refs/remotes/origin/*<br />
[user]<br />
  name = $GIT_USER<br />
  email = $GIT_EMAIL<br />
[brach "master"]<br />
  remote = origin<br />
  merge = refs/heads/master<br />
