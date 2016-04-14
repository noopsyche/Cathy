# Cathy
Cathy是一个智能(控制)家居管理的方案。采用Arduino来实现对继电器，传感器的控制。

## 简单原理介绍

![原理简介](https://github.com/dongkaipo/Cathy/blob/master/screenshots/0.%20introduction.jpg)

1. 手机通过`SmartConfig` 技术来配置`ESP8266` 使其能连入互联网
2. `ESP8266` 每1~2秒访问服务器来做长连接，上传数据和获取服务器是否有活动请求
3. 手机访问服务器来获取`ESP8266` 上传到服务器的数据，同时可以通过请求来改变服务器状态
4. `ESP8266` 读取到服务器状态改变后通知`Arduino(主机)` 
5. `Arduino(主机)` 通过`nrf24l01` 发送请求到指定 `Arduino(从机)`
6. `Arduino(从机)` 控制硬件做出相应的改变

## 相关技术

1. [Arduino] (http://www.arduino.cc/) 很好入门的一个开源硬件平台
2. [Laravel] (https://laravel.com/) 简洁、优雅的PHP Web开发框架(PHP Web Framework)
3. [Swift] (https://developer.apple.com/swift/)是一款易学易用的编程语言，而且它还是第一套具有与脚本语言同样的表现力和趣味性的系统编程语言

## 用到的库(排名不分先后)
### Swift & Object-C (手机端)
1. [MBProgressHUD] ()
2. [Alamofire] ()
3. [TPKeyboardAvoiding] ()
4. [SDWebImage] ()
5. [DynamicBlurView] ()
6. [Qiniu] ()
7. [CocoaLumberjack/Swift]()
8. ....

### Arduino (硬件端)
1. [ESP8266](https://github.com/esp8266/Arduino) ESP8266 core for Arduino
2. [nRF24L01]()
3. ...

### Server (服务器云端)
1. [Qiniu] ()
2. ...

## 用到的工具(IDE)
1. [Sublime] ()
2. [PHPStream] ()
3. [Xcode] ()
4. [Sketch] ()
5. [Sequel Pro] ()
6. [Homestead] ()
7. [Virtual Box] ()
8. [Vagrant] ()
9. [Arduino IDE] ()
10. [Postman] ()
11. [OmniGraffie] ()
12. [Dash] ()
13. [MindNode] ()
14. ...

## 相关项目
1. [Cathy-Web] ()
2. [Cathy-iPhone] ()
3. [Cathy-Arduino-Center] ()
4. [Cathy-Arduino-Light] ()
5. ...
