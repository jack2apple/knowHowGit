## git 使用
#### git clone 提示代理错误
```
Q：git returns http error 407 from proxy
A：
first：
git config --global http.proxy http://username:password@proxiURL:proxiPort
then：
git config --global http.sslVerify false
```
