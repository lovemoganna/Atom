## git-flow的基本概念

![](https://upload-images.jianshu.io/upload_images/2461501-c7ea6ac284c8f6b2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/600)

##  master 分支和 develop分支

在Git Flow 中，这两个分支至关重要，它们会贯彻整个流程始终，绝对不会被删除。

### master 分支

master 分支时常保持着软件可以正常运行的状态。由于要维护这一状态，所以不允许开发者直接对master 分支的代码进行修改和提交。

其他分支的开发工作进展到可以发布的程度后，将会与master分支进行合并，并且这一合并只在发布成品时即完成release分支时进行。发布时将会附加版本编号的Git标签。

### develop分支

develop分支是开发过程中代码中心分支。与master 分支一样，这个分支也不允许开发者直接进行修改和提交。

### feature分支

程序员要以develop分支为起点新建feature 分支，在feature 分支中进行新功能的开发或者代码的修正。也就是说develop分支维系着开发过程中的最新代码，以便程序员创建feature分支进行自己的工作。

### release分支

测试分支，基于delevop分支克隆，产品编码工作完成后，发布到本分支测试，测试过程中发现的小bug直接在本分支进行修复，修复完成后合并到develop分支。本分支属于临时分支，目的实现后可删除分支。

###  bugfix分支

Bug修复分支，基于master分支或发布的里程碑Tag克隆，主要用于修复对外发布的分支，收到客户的Bug反馈后，在此分支进行修复，修复完毕后分别合并到develop分支和master分支。本分支属于临时分支，目的实现后可删除分支。

## git-flow在sourceTree中的使用

![](https://upload-images.jianshu.io/upload_images/7505161-0bc3c6c5cfbbc8d5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## gitflow中开发新功能的实现

现在我正在做的就是编写gitflow的使用方法,这就是一个新功能.

![](https://upload-images.jianshu.io/upload_images/7505161-51cb05903a09a1cb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

