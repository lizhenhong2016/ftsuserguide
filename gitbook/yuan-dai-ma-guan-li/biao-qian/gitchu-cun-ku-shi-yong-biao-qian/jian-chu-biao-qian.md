##### **检出标签**

在 Git 中你并不能真的检出一个标签，因为它们并不能像分支一样来回移动。 如果你想要工作目录与仓库中特定的标签版本完全一样，可以使用 git checkout -b \[branchname\] \[tagname\] 在特定的标签上创建一个新分支：

$ git checkout -btest v2.0.0

当然，如果在这之后又进行了一次提交，version2 分支会因为改动向前移动了，那么 version2 分支就会和 v2.0.0 标签稍微有些不同，这时就应该当心了。

之后可以分支方式签出标签

$ git checkout test

签出原master分支

$ git checkout master

