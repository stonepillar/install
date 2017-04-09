# Install GitHub
## Generated SSH key for github

Right:
> ssh-keygen -t rsa -b 4096 -C "you@gmail.com"

Wrong:
> ssh-keygen -t rsa -b 4096 -f /Users/you/.ssh/id_rsa.github -C "you@gmail.com"

Note:
 -f: set the SSH key file name and saved directory, but github only support the name "id_rsa"
 -b: selected the number of password bit

For test SSH key:
> ssh -T  git@github.com

For test SSH key with verbose:
> ssh -Tv git@github.com

## Prepare for Git

Three level of git config: local, global, system.
The related config file is saved as local directory .git/config, ~/.gitconfig, install_directory/gitconfig.

Below is the config setting:
> git config --global user.name  "you name"
> git config --global user.email "you_email@youemail.com"
