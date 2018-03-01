### l**版本控制**

无限制、专用、安全

使用无限制专用存储库对代码进行存储并协作编写代码。使用 Git 来进行分布式版本控制，或使用 Team Foundation 版本控制 \(TFVC\) 来实现集中式版本控制。 通过拉取请求和代码审阅轻松地与代码协作。 管理权限和策略以保护你的存储库。

#### **1、在 Team Foundation 版本控制中开发应用程序**

参考：[https://msdn.microsoft.com/library/ms181382.aspx](https://msdn.microsoft.com/library/ms181382.aspx)

#### **2、Git命令版本控制开发应用程序**

参考：[https://docs.microsoft.com/zh-cn/vsts/git/tutorial/creatingrepo](https://docs.microsoft.com/zh-cn/vsts/git/tutorial/creatingrepo)

创建好Git储存库后，我们可以通以Git命令将项目克隆到本地

![](/assets/import11.png)

使用Git命令推送更新到服务器

1.选定一个文件夹，初始化git 本地文件夹

git init

2.使用git clone命令将新建的git 项目信息下载到本地

```
git clone git %address%  
```

3.进入git项目的本地文件夹，查看状态

```
cd 本地文件夹

git status   
```

4.提交所有的新文件

```
git add -A \(提交所有变化\)

git add -u \(提交被修改\(modified\)和被删除\(deleted\)文件，不包括新文件\(new\)\)

git add  .  \(提交新文件\(new\)和被修改\(modified\)文件，不包括被删除\(deleted\)文件\)
```

5.通过在Git命令窗口中输入以下命令来提交您的更改

```
git commit -a -m "first commit"
```

当使用git提交时，-a 意味着提交所有修改过的文件，-m 指定一个提交消息。

6.将您的更改推到Git服务器上

```
git push  
```

选择储存库，可以对其设置访问控制。

![](/assets/import12.png)

