# 加速访问 Github

## 1. 找到并打开 host 文件
* windows:
C:\Windows\System32\drivers\etc
* linux:
/etc/hosts


## 2. 找到以下内容（若没有自行则添加）：
```java
# GitHub Start 
192.30.253.112 github.com 
192.30.253.119 gist.github.com 
185.199.109.153 assets-cdn.github.com
199.232.5.194 github.global.ssl.fastly.net 
199.232.28.133 cloud.githubusercontent.com
199.232.68.133 gist.githubusercontent.com 
199.232.68.133 camo.githubusercontent.com 
199.232.68.133 avatars0.githubusercontent.com 
199.232.68.133 avatars1.githubusercontent.com 
199.232.68.133 avatars2.githubusercontent.com 
199.232.68.133 avatars3.githubusercontent.com 
199.232.68.133 avatars4.githubusercontent.com 
199.232.68.133 avatars5.githubusercontent.com 
199.232.68.133 avatars6.githubusercontent.com 
199.232.68.133 avatars7.githubusercontent.com 
199.232.68.133 avatars8.githubusercontent.com 
# GitHub End
```


## 3. 在 ipaddress.com 查询以上各网站的IP地址并进行更新：

 查询结果示例：
* github.com
	* 192.30.253.112
* assets-cdn.github.com
	* 185.199.108.153
	* 185.199.109.153
	* 185.199.110.153
	* 185.199.111.153
* github.global.ssl.fastly.net
	* 199.232.5.194


## 4. 更新完之后刷新系统dns缓存

用WIN+R快捷键打开运行窗口，输入命令：cmd并回车进入命令行窗口。接着输入命令：ipconfig /flushdns回车后执行刷新本地dns缓存数据即可。


## 5. 刷新网页即可
