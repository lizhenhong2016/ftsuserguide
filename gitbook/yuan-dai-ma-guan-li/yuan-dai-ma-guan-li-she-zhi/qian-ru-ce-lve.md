##### **签入策略**

1）、管理员配置签入策略设置。在签入对话框中，管理员可以添加想要的签入策略。

![](/assets/import21.png)

1.在团队资源管理器中，右击团队项目，单击“团队项目设置”，然后单击“源代码管理”。

“源代码管理设置”对话框出现。

2.单击“签入策略”选项卡，然后单击“添加”。

“添加签入策略”对话框出现。

3.在“签入策略”列表中，选择想要的策略类型，然后单击“确定”。

该列表包含下列选择。

o如果选择“代码分析”，则会出现“代码分析策略编辑器”对话框。请单击对应于要执行的代码分析类型的框。这些选项为“执行签入以只包含属于当前解决方案的文件”、“执行 C/C++ 代码分析 \(/analyze\)”和“对托管代码执行代码分析”。如果选择“对托管代码执行代码分析”，请在“托管代码分析的规则设置”窗口中选择所需的规则设置。单击“确定”。有关如何使用代码分析工具的更多信息，请参见[代码分析工具使用准则](https://msdn.microsoft.com/zh-cn/library/ms182023%28v=vs.80%29.aspx)。

o如果选择“测试策略”，则会出现“测试策略”对话框。单击“浏览”以指定元数据文件，选择所需的测试，然后单击“确定”。

o如果选择“工作项”，则会向列表中添加一个要求必须将某个工作项与签入相关联的策略。

4.当您对签入策略的设置感到满意时，请单击“确定”；从现在起，新的签入策略将随将来的签入一起显示。

