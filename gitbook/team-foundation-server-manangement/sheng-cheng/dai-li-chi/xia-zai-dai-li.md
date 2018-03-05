新建代理池后并不能马上使用代理功能，需要下载代理并安装在服务器上。下载代理和安装需要在服务器上操作。

下载代理并安装：

![](/assets/import26.png)

下载完成得到agent.zip文件，将其解压到指定目录（如 C:\agent3）下。

![](/assets/import27.png)

使用cmd控制台管理，进入到agent目录：

执行ConfiguerAgent.cmd;

输入代理名称：自定义名称。（如test3）

输入Team Foundation Server Url：服务TFS url。 （如 [http://10.2.11.145:8080/tfs](http://10.2.11.145:8080/tfs%29%29\)）

针 对哪个代理配置此代理：输入代理池名称。（如 test3）

是否要将代理作为windows服务进行安装：是。

输入用于此服务的用户账户名称和密码。

![](/assets/import28.png)

配置成功后代理池下可见：

![](/assets/import29.png)

