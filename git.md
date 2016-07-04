## git 使用
#### 1.git clone 提示代理错误
Q：git returns http error 407 from proxy
A：
first：
git config --global http.proxy http://username:password@proxiURL:proxiPort
then：
git config --global http.sslVerify false
use https to clone:
git clone https://github.com/user/repository

#### 2.git ssh key 生成
* 查看是否已经有了ssh密钥：cd ~/.ssh
* 生存密钥：ssh-keygen -t rsa -C “user@mail.com”
* github上添加ssh密钥，这要添加的是“id_rsa.pub”里面的公钥
* 测试：ssh git@github.com
* 获取源码：git clone git@github.com:user/repository

#### 3.git ignore
* vi ~/gitHub/.gitignore_global
* 添加.DS_Store  
* git config --global core.excludesfile ~/gitHub/.gitignore_global 

#### 4.本地仓库上传至远程新仓库
* 本地git init add commit
* github 新建仓库calculatorGit
* git remote add origin git@github.com:user/calculatorGit
* git pull origin master
* git push origin master
