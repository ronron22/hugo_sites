## Installing Hugo ##

### Define GOPATH ###

```bash
# installing golang
apt-get install golang
# installing hugo 
echo "GOPATH=$HOME/go" >> ~/.bashrc
echo "PATH=$PATH:$GOROOT/bin:$GOPATH/bin" >> ~/.bashrc
source ~/.bashrc
```
#### From github 

go get github.com/kardianos/govendor
govendor get github.com/gohugoio/hugo
go install github.com/gohugoio/hugo

### Installing themes

Get theme link on https://themes.gohugo.io

and

```bash
cd themes
git clone https://github.com/calintat/minimal
```
