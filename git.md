## git 使用
#### 1.git clone 提示代理错误
Q：git returns http error 407 from proxy
A：
first：
git config --global http.proxy http://username:password@proxiURL:proxiPort
then：
git config --global http.sslVerify false

#### 2.git ssh key 生成
* 查看是否已经有了ssh密钥：cd ~/.ssh
* 生存密钥：ssh-keygen -t rsa -C “user@mail.com”
* github上添加ssh密钥，这要添加的是“id_rsa.pub”里面的公钥
* 测试：ssh git@github.com
* 获取源码：git clone git@github.com:user/repository