
[github中repositories与projects区别](https://blog.csdn.net/rensihui/article/details/99889432)
```
一、概述

        Github上边的repositories翻译为代码仓库，可以保存多个代码工程和项目的代码，资源，文本、图片......等;

        而projects可以翻译为项目板，是project-boards的简写。简单说，可以理解为工作计划表之类的书签，制定一下工作计划，Bug，流程什么的。

        这么看，这很反直觉哇，我还以为projects也是项目什么的，没想到和我印象中的差得很远。。。

二、官方说明

        repositories：仓库就像项目的文件夹。 项目的仓库包含项目的所有文件，并存储每个文件的修订记录。 您也可以在仓库中讨论并管理项目的工作。您可以个人拥有仓库，也可以与组织中的其他人共享仓库的所有权。

        projects：GitHub 上的项目板帮助您组织工作和排列工作的优先级。 您可以为特定功能工作、全面的路线图甚至发布检查列表创建项目板。 通过项目板可以灵活地创建适合需求的自定义工作流程。项目板包括议题、拉取请求和注释，在选择的列中分类为卡片。 您可以拖放或使用键盘快捷键对列中的卡片重新排序，在不同列之间移动卡片，以及更改列的顺序。
```
[在github同一个仓库立上传多个项目](https://blog.csdn.net/Asuna_Yu/article/details/80217020?utm_medium=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param)

[github一个repository下多个项目](https://blog.csdn.net/keneyr/article/details/106426215?utm_medium=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param)

[一个仓库管理多个项目](https://blog.csdn.net/ahxieqi/article/details/93628549?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param)

[Features · Project management · GitHub](https://github.com/features/project-management/)
Project management, made simple
On GitHub, project managers and developers coordinate, track, and update their work in one place, so projects stay transparent and on schedule.

Start with an issue
Create an issue to suggest a new idea or track a bug. Then organize and assign tasks to your team. And don’t spare any attachments—issues support most image and file types.


[Explore GitHub · GitHub](https://github.com/explore)

-----
[Github 新的项目管理模式——Projects](https://www.cnblogs.com/qin-nz/p/5886945.html)

Issues
Github 中传统的项目管理是使用 issue 和 pull request 进行的，这部分内容不是本文重点，不再赘述。 但有一些功能需要提及：

Tag： 每个 issue 可以添加不同的 tag，可以用于标记 issue 的种类和 issue 的处理进度；
MileStone：每个 issue 只属于一个 milestone，用于显示 issue 的处理进度。
Projects 概述
这是Github 2016年9月份新的功能，如图所示：

no-project.png

Project 提供了真正的管理 issue 的能力；而传统的 tag 方式只能以手工的方式管理分类（如 Q&A，bug，duplicate，feature 这些标签🏷），或者以手工的方式管理 issue 进度（need test, in progress, wait approval 等这些标签）。

不过在开始讨论这个之前，有必要先讨论一下看板方法。

看板（Kanban）
什么是看板？
看板管理，起源于丰田的生产模式中，指为了达到及时生产（JIT）方式控制现场生产流程的工具。及时生产方式中的拉式（Pull）生产系统可以使信息的流程缩短，并配合定量、固定装货容器等方式，而使生产过程中的物料流动顺畅。

需要详细了解的请看Wiki。

如果还是没看懂，这里有几个看板的例子：

KanbanFlow & Trello
KanbanFlow kanbanflow.png

Trello trello.png

可以看出，所谓看板，就是把一块木板上分成几列，然后在每一列上贴上不同内容的卡片。 木板上的这几列一般是有顺序的，卡片可以在不同的列之间移动来表明所处的状态。

以上的两个例子，看板并不是针对软件工程的，他们的市场也是一般的企业（比如丰田这样的）。

Zenhub & Github Projects
下面的两个例子则是针对软件开发做了优化，准确的说，它们都是对 Github 做了适配。

Zenhub zenhub-task-board.jpg

Github Projects Github-Kanban.png

Zenhub 是个浏览器插件，就是把 Github 的 issues 当作卡片，以 Kanban 的形式展现 issue，也提供了一个比较鸡肋的 Epic 的功能，同时针对个人也有 TODO 项管理。
而 Github 最近推出的 Project 不仅可以使用 issues 作为卡片，还可以使用Note（左侧的三个），这样我们就没有必要为了在看板上记录可能的需求而创建一个新的 issues 或者把问题记录在个人的 TODO 列表上了。

Github Projects
一个仓库可以包含多个项目；最初，这个设定让我疑惑，直到使用之后才明白， 一个代码仓库通常有很多事情要做，比如：

拟定线路图
增加一个新功能
发布一个新版本
因此，我们可以为以上每一件事创建一个 Project，由于 Github 中并没有类似 Epic 的机制，因此使用不同的 Project 则很有用了。

可以看到，有了 Project 的 Kanban 之后，原来 tag 的部分功能（如标记处理进度等）可以被看板替代。 Github Project 提供的 Note 可以在需要的时候单项转换为 issue：

convert-to-issue.png

同时，Kanban 不仅可以包含 issue 和 note，还可以包含 pull request。

Github 终于有了比较靠谱的项目管理工具，开源项目的又有了更好的工具。 撒花o(^▽^)o

祝愿我自己早日完成我的第一个开源项目（IMAP Server）。

本文首发于我的个人博客 (https://hudingyuan.cn/a/11)

-----
[(四)GitHub中projects和repositories的区别](https://blog.csdn.net/xpj8888/article/details/89471095)

https://www.cnblogs.com/f1194361820/p/4741558.html一个仓库repositories可以管理多个工程projects

https://blog.csdn.net/u010969626/article/details/51607187

https://blog.csdn.net/putao2062/article/details/80516001github上怎么在一个仓库里放多个项目？创建分支时使用orphan参数


[《github》创建repository和创建project的区别? - 知乎](https://www.zhihu.com/question/317963046)

repo 不用介绍了吧，就是存放代码的仓库。

project 是项目管理工具，也就是看板，可以是项目进度管理，issue 解决进度等，类似于 jira