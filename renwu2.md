# URL是什么

- URL是使用Web浏览器等访问Web页面时需要输入的网页地址。

- 在所输入的URL中又包括

 1. 协议方案名（http ftp mailto telnet file等协议）标准的协议方案有30种左右

 2. 登录信息（认证）

 3. 服务器地址（域名）

 4. 服务器端口号

 5. 带层次的文件路径

 6. 查询字符串

 7. 片段标识符

例如下图：

![](http://upload-images.jianshu.io/upload_images/4337988-4987458ea1f12d79.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

# 域名解析

语义化的域名确实更利于人类记忆（百度 www.baidu.com），可是电脑收到用户输入的网址后，要想让电脑理解这一串字符串，就有些困难了，因为计算机更擅长处理一长串数字，那么IP地址和DNS服务就显得非常重要了。

## IP地址

- IP地址是指互联网协议地址，每个处于互联网中的设备都有IP 地址，形如192.168.0.1

- 局域网 IP 和公网 IP 是有差别的

- 127.0.0.1代表本机的 IP

## DNS服务

DNS协议提供通过域名查找IP地址，或逆向IP地址反查域名的服务。

流程如下

1. 浏览器缓存 – 浏览器会缓存DNS记录一段时间

2. 系统缓存 - 从 Hosts 文件查找是否有该域名和对应 IP。

3. 路由器缓存 – 一般路由器也会缓存域名信息。

4. ISP DNS 缓存 – 比如到电信的 DNS 上查找缓存。

5. 如果都没有找到，则向根域名服务器查找域名对应 IP，根域名服务器把请求转发到下一级，知道找到 IP

# 服务器处理

- 常见的Web服务器有Apache、Nginx、lls、Lighttpd

- web服务器接收用户的Request交给网站代码，或者接受请求反向代理其他web服务器


![](http://upload-images.jianshu.io/upload_images/4337988-f200384de3e3df9c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



# 网站处理流程

MVC模型(model)-视图(view)-控制器(controller)


![](http://upload-images.jianshu.io/upload_images/4337988-61e48697137461fb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


# 浏览器处理

1. HTML字符串被浏览器接受后被一句句读取解析

2. 解析到link 标签后重新发送请求获取css

3. 解析到 script标签后发送请求获取 js，并执行代码

4. 解析到img 标签后发送请求获取图片资源

# 绘制网页

浏览器根据 HTML 和 CSS 计算得到渲染树，绘制到屏幕上js 会被执行