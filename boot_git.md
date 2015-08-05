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
