### Prerequisites
[boot_vagrant_centos.md](boot_vagrant_centos.md)

### Initial setup
```sh
export USERLOCAL=/jnandakishore/userlocal
export PATH=$USERLOCAL/bin:$PATH
export cmmi='./configure --prefix=$USERLOCAL && make && make install'
```
### Download git
```sh
cd ~/Downloads
wget https://www.kernel.org/pub/software/scm/git/git-2.5.0.tar.gz
```

### Install git
```sh
tar xvzf git-2.5.0.tar.gz
cd git-2.5.0
cmmi
git --version
```

### Goodies
#### Dotfiles
* Lookup github.com/none-da/dotfiles/dotgitconfig

#### Bash prompt
Put these in bashrc
```sh
source /jnandakishore/softwares/git-2.5.0/contrib/completion/git-completion.bash
source /jnandakishore/softwares/git-2.5.0/contrib/completion/git-prompt.sh
GIT_PS1_SHOWCOLORHINTS=1
PROMPT_COMMAND='__git_ps1 "\u@\h:\w" "\\\$ "'
```
