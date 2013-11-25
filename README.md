猎豹浏览器皮肤定制文档
====================

关于此文档
--------------------

本文档是猎豹浏览器官方皮肤定制文档，目的是帮助用户快速找到皮肤配置文件中配置项的详解，以及简单的皮肤制作教程。

包含的主要内容为 `mainfest.json` 、`layout_main` 和 `layout_parameter` 等配置文件中配置项的具体解释，以及如何制作一款猎豹浏览器专属皮肤的简易教程。

您可以在[doc.crxpower.org](http://doc.crxpower.org)查看文档效果，使用 `CTRL + D` 快捷键可以将此文档放入收藏夹中随时查看。


为此文档做贡献
====================

此文档为开源项目，任何人都可以为此文档做贡献 —— 报错、修复、新特性等等。

提交修改
---------------------

您可以在此项目的 [issues](https://github.com/lb-crx/theme/issues/new)，来为此文档提交问题。查看其它作者提交的 issues 请戳[这里](http://https://github.com/lb-crx/theme/issues?page=1&state=closed)。

参与讨论
---------------------

您可以在[这里](https://github.com/lb-crx/theme/issues?page=1&state=open)查看我们正在进行中的任务，以及对未来的规划。欢迎您也加入我们的讨论中，让此文档做的更好。

贡献内容
---------------------

此文档尚处于开发完善阶段，还是有很多的疏忽与遗漏，以及对某些内容描述不够彻底，希望能够联系广大皮肤制作者的力量来完善此文档，更好的为开发者服务。故欢迎大家通过 [pull requests](https://github.com/lb-crx/theme/compare) 的方式来为此文档添砖加瓦。

如何 pull requests
---------------------

1. 首先 `fork` 一份到自己的 git 仓库中。点击项目主页的 [Fork](https://github.com/lb-crx/theme/fork) 按钮，按照网站的提示将官方皮肤库 fork 到自己的仓库中。
2. 修改源文件。您可以在自己的页面中直接修改仓库中的文件，或者 clone 一份到本地修改。然后再提交到 github 中。提示，请先新建一个分支(例如命名为：`patch-1`)然后基于此分支进行相应的修改。
3. 提交 pull request。到[官方项目页面](https://github.com/lb-crx/theme)中，点击 [pull requests](https://github.com/lb-crx/theme/pulls) 绿色按钮，按照提示将您的仓库中的 patch-1 分支提交到 官方的 master 分支中。提交 pull requests 后，您就可以在官方的[pull request 列表](https://github.com/lb-crx/theme/pulls)页面中看到您刚才的提交。等待项目管理员的确认后，就可以将您的修改合并到主分支中。

通过上面的简单步骤，您就可以完成对本项目的贡献了。如果在 pull request 过程中遇到问题，请访问 github 的[帮助页面](https://help.github.com/)寻求解答，或者到项目的 [issues](https://github.com/lb-crx/theme/issues/new) 中提交问题。在提问之前，推荐您阅读 [提问的智慧 AskForHelp - Woodpecker Wiki for CPUG](http://wiki.woodpecker.org.cn/moin/AskForHelp)。


本地安装
=====================

本文档是基于 [sphinx](http://sphinx-doc.org/) 来管理和运用的，依赖 [python 2.7](http://www.python.org/) 语言环境。

如何本地调试
---------------------

1. 安装 [python 2.7](http://www.python.org/download/releases/2.7.6/)，以及 [easy_install](https://pypi.python.org/pypi/setuptools#installation-instructions)。
2. 安装 sphinx。在命令行工具中输入 `easy_install sphinx` 来安装 sphinx 文档管理工具。
3. 下载本项目的源代码。您可以使用 git 工具 `git clone https://github.com/lb-crx/theme.git` 来克隆此项目到本地；或者直接点击[这里](https://github.com/lb-crx/theme/archive/master.zip)来直接下载完整项目文件。
4. 生成静态HTML页面。在命令行中进入到项目文件夹中，输入`make html`来生成此文档的静态页面，方便在浏览器中查看效果。生成的静态页面在根目录的 `build` 文件夹中，使用浏览器打开 `index.html` 就可以在浏览器中查看此文档了。


文档修改历史
=====================

- 131030 re-init. github

- 130801 init. Intra. @ruby
    - for 猎豹皮肤定制手册
    - for 猎豹皮肤中心手册

- 外部清理:[42d1c704d3](https://github.com/lb-crx/doc/commit/42d1c704d30c3dbbc90547fa21d0c636b803059b)
