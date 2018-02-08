TFS 用户指南


	什么是 Team Foundation Server？
针对整个团队的协作软件开发工具
Team Foundation Server 提供一组协作软件开发工具，它与你现有的 IDE 或编辑器集成，从而使你的跨功能团队可以在所有大小的软件项目上高效工作。
 
  

TFS提供了一组集成的特性，可以通过web浏览器或支持的IDE访问这些特性，包括:

1、用于源代码的源代码控制的Git存储库
2、构建和发布管理以支持持续集成和交付应用程序
3、敏捷工具支持计划和跟踪您的工作，代码缺陷，以及使用看板和Scrum方法的问题
4、测试您的应用程序的各种工具，包括手动/探索性测试、负载测试和持续测试
5、用于共享进度和趋势的高度可定制的仪表板

此外，TFS生态系统还提供了对添加扩展的支持，集成了其他流行的服务，例如:篝火、Slack、Trello、UserVoice，以及开发你自己的自定义扩展。

在部署TFS时，还可以配置以下服务器或集成点:

构建服务器:支持本地和云托管的构建
SQL Server和SQL分析服务器:支持SQL Server报告和基于多维数据集创建Excel轴心图表的能力

在哪里开始呢?

首先，免费下载TFS Express
然后，上传代码来共享或源代码控制
或者，开始使用Scrum、看板或方法组合来跟踪你的工作

当您需要数据留在您的网络中，或者您想要访问与TFS数据和工具集成的SQL Server reporting services时，选择一个本地的TFS。
你可以通过下载TFS Express免费开始。


	Team Foundation Server Express
供个人或小团队免费使用
将 Team Foundation Server Express 提供给单个开发人员或五人（或五人以下）的小型团队使用。 在你的个人台式电脑或笔记本电脑上轻松安装，无需专用服务器。 当你的团队扩展到五位团队成员以上时，升级到 Team Foundation Server 并带上你的完整的历史记录

	访问级别
访问级别使管理员能够为他们的用户提供他们需要的功能，并且只需要支付这些功能。为了连接和使用TFS提供的功能和特性，必须将用户添加到具有适当权限的组中。要使用select web portal特性，它们还必须属于允许访问该特性的访问级别。
当您将一个用户或组添加到一个团队或团队项目时，他们会自动获得访问默认访问级别所支持的那些功能，这是基本的。这为大多数用户提供了所需的所有特性.

访问级别要设置为 基本 或 高级，否则新添加到团队中的用户（除属于administratrer）将无法访问源代码
 

https://docs.microsoft.com/zh-cn/vsts/security/access-levels

	团队项目集合
1、从服务TFS管理控制台中创建一个集合，如Test
2、在web部打开url ，域名若访问不了，改成IP访问。如：http://10.2.21.145:8080/tfs/Test

 

3、创建团队项目
VS 客户端创建 https://msdn.microsoft.com/library/ms181477.aspx
WEB 端创建，通过上图URLhttp://10.2.21.145:8080/tfs 进入，选择管理。
1）选择集合并查看集合管理页
 
2）新建团队项目
 
3）可选择版本控制方式
 

4）选择Git版本控制
 



4、添加用户和组
   在安全性选项中添加用户和组
 

	版本控制
无限制、专用、安全
使用无限制专用存储库对代码进行存储并协作编写代码。 使用 Git 来进行分布式版本控制，或使用 Team Foundation 版本控制 (TFVC) 来实现集中式版本控制。 通过拉取请求和代码审阅轻松地与代码协作。 管理权限和策略以保护你的存储库。
1、在 Team Foundation 版本控制中开发应用程序
   参考： https://msdn.microsoft.com/library/ms181382.aspx 


2、Git命令版本控制开发应用程序
   参考： https://docs.microsoft.com/zh-cn/vsts/git/tutorial/creatingrepo 

	
1. 选定一个文件夹，初始化git 本地文件夹
  
   git init

2. 使用git clone命令将新建的git 项目信息下载到本地

    git clone git %address%  

3. 进入git项目的本地文件夹，查看状态

    cd 本地文件夹
    git status   

4. 提交所有的新文件 
  
    git add -A (提交所有变化)
    git add -u (提交被修改(modified)和被删除(deleted)文件，不包括新文件(new))
    git add  .  (提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件)

5. 通过在Git命令窗口中输入以下命令来提交您的更改 

    git commit -a -m "first commit" 

    当使用git提交时，-a 意味着提交所有修改过的文件，-m 指定一个提交消息。

6. 将您的更改推到Git服务器上

    git push  


	安全性
1、权限是在权限和组中描述的集合、团队项目和对象级别设置的。因此，要查看您拥有的权限，您需要在对象、项目或集合级别上打开权限。
 

2、组和用户权限设置
 

3、添加成员
 
4、git 储存库权限设置

 


	持续集成
版本、程序包、测试、发布、重复
通过持续集成 (CI) 版本在早期发现质量问题。 使用发布管理自动化跟踪你的所有部署。 使用我们广泛的测试工具组来维护较高的质量。 通过重复使用代码和模块更快地交付程序包管理。

	Java 支持
对任何平台进行开发
使用你选择的 IDE：Eclipse、IntelliJ、Android Studio、Visual Studio Code 等。 从你的 Git、Subversion 和 TFVC 存储库使用 Ant、Maven 和 Gradle 构建你的代码。 借助本机功能或通过与系统（如 Jenkins）的集成来实现 CI/CD。 支持跨平台和移动语言，包括：C++、PHP、Python、Go、Swift 等更多语言。


