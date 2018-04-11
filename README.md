# beego-dev
 

## mac安装go
brew install go
open ~/.zshrc
## 粘贴下面命令:
 
export GOROOT=/usr/local/opt/go/libexec
export GOPATH=$HOME/.go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin

### 安装beego
go get github.com/astaxie/beego
### bee 工具的安装
go get github.com/beego/bee
### 自定义参数自动连接数据库创建相关 model 和 controller:
bee api cms_api -tables="user"  -driver=mysql -conn="root:123456@/cms_dev"
