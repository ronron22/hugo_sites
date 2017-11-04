## Installing Hugo ##

### Define GOPATH ###

```bash
# installing golang
apt-get install golang
# installing hugo 
echo "export GOPATH=$HOME/go" >> .bashrc
echo "export PATH=$PATH:$GOROOT/bin:$GOPATH/bin" >> .bashrc
source .bashrc
```

### Installing themes

Get theme link on https://themes.gohugo.io

and

```bash
cd themes
git clone https://github.com/calintat/minimal
```
