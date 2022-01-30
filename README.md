# ESP8266-WiFi-UART-Bridge
这里代码由开源项目:
[ESP8266-WiFi-UART-Bridge](https://github.com/roboremo/ESP8266-WiFi-UART-Bridgehttps://github.com/roboremo/ESP8266-WiFi-UART-Bridge)以及
[esp8266-AP-Tcp-Server](esp8266-AP-Tcp-Server)
组合而成
在文件夹v1.1中， 有server和client的代码，其中server为服务器代码
client为客户端代码

使用方法：

**服务器**

用arduino打开server代码， 然后把代码编译下载到一个esp8266硬件中，它会产生名称为:ESP8266WIFI的wifi， 密码为:12345678让客户端连接

**客户端**

用arduino打开client代码， 然后把代码编译下载到硬件中，它会连接服务器产生的wifi, 然后所有下载了客户端代码的硬件，只要有一方通过串口发送了数据， 另外所有的esp8266客户端都能够收到信息， 并且通过串口输出.

==客户端连接服务器后，传给服务器信息，然后服务器转发给所有非发送客户端==




