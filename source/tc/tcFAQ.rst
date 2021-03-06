.. include:: ../LINKS.rst

.. _chapterFAQ:


常见问题(1/1)
===================

如果您在这里找不到您的问题的答案，请尝试 `Chrome网上应用店常见问题 <https://code.google.com/chrome/webstore/faq.html>`_ （英文）、 `网上论坛 <https://groups.google.com/a/chromium.org/group/chromium-extensions>`_ （英文）或 `网上应用店帮助 <https://www.google.com/support/chrome_webstore/?hl=zh-CN>`_ 帮助。


一般问题
----------------------------------------

#. :ref:`什么是Google Chrome浏览器扩展程序？ <chapterFAQ-nomo1>`
#. :ref:`我应该如何设置Chrome浏览器以便开发扩展程序？ <chapterFAQ-nomo2>`
#. :ref:`为Chrome浏览器编写扩展程序时需要用到哪些技术？ <chapterFAQ-nomo3>`
#. :ref:`扩展程序是不是每一次浏览器载入时都要从网上获取？ <chapterFAQ-nomo4>`
#. :ref:`我应该如何确定Chrome浏览器版本与分支间的对应关系？ <chapterFAQ-nomo5>`


扩展程序的能力
----------------------------------------

#. :ref:`扩展程序能否发起跨域名Ajax请求？ <chapterFAQ-ext1>`
#. :ref:`扩展程序能否使用第三方网上服务？ <chapterFAQ-ext2>`
#. :ref:`扩展程序能否编码/解码JSON数据？ <chapterFAQ-ext3>`
#. :ref:`扩展程序能否在本地存储数据？ <chapterFAQ-ext4>`
#. :ref:`扩展程序能否使用OAuth？ <chapterFAQ-ext5>`
#. :ref:`扩展程序能否加载DLL？ <chapterFAQ-ext6>`
#. :ref:`扩展程序能否在呈现的网页外创建用户界面？ <chapterFAQ-ext7>`
#. :ref:`扩展程序能否监听Chrome标签页以及导航按钮的点击？ <chapterFAQ-ext8>`
#. :ref:`两个扩展程序能否互相通信？ <chapterFAQ-ext9>`
#. :ref:`扩展程序能否使用Google Analytics（分析）？ <chapterFAQ-ext10>`
#. :ref:`扩展程序能否修改chrome://协议的URL？ <chapterFAQ-ext11>`
#. :ref:`扩展程序能否在没有用户交互的情况下打开浏览器/页面按钮的弹出内容？ <chapterFAQ-ext12>`
#. :ref:`扩展程序能否在用户单击其它地方后仍然使弹出内容保持打开状态？ <chapterFAQ-ext13>`
#. :ref:`扩展程序能否在安装和卸载时得到通知？ <chapterFAQ-ext14>`


开发
----------------------------------------

#. :ref:`我应该如何为我的扩展程序建立用户界面？ <chapterFAQ-dev1>`
#. :ref:`我能够在本地存储中储存多少数据？ <chapterFAQ-dev2>`
#. :ref:`我应该如何为我的应用程序创建一个选项菜单？ <chapterFAQ-dev3>`
#. :ref:`扩展程序的开发人员可以使用哪些调试工具？ <chapterFAQ-dev4>`
#. :ref:`为什么通配符匹配对于顶级域名（TLD）不适用？ <chapterFAQ-dev5>`
#. :ref:`为什么当我的扩展程序安装或卸载时管理API不产生事件？ <chapterFAQ-dev6>`
#. :ref:`扩展程序如何确定是否是第一次运行？ <chapterFAQ-dev7>`

调试
----------------------------------------

#. :ref:`更改皮肤中的文件后再次通过“载入正在开发的扩展程序”不能更新皮肤？ <chapterFAQ-deb1>`
#. :ref:`打包皮肤文件时报错“猎豹4.0暂不支持非官方皮肤”？ <chapterFAQ-deb2>`

请求新特性和报告问题
----------------------------------------

#. :ref:`我认为我发现了一个bug！我应该做什么确保让它被修复？ <chapterFAQ-ask1>`
#. :ref:`我想请求新特性！我应该如何报告？ <chapterFAQ-ask2>`



一般问题:

.. _chapterFAQ-nomo1:

什么是Google Chrome浏览器的扩展程序？:
    Google Chrome浏览器的扩展程序是在Chrome浏览器中运行并提供附加功能、与第三方网站或服务整合、自定义浏览体验的应用程序。

.. _chapterFAQ-nomo2:

我应该如何设置Chrome浏览器以便开发扩展程序？:
    - 只要您正在使用支持扩展程序的某个版本的Chrome浏览器，您就已经完全有条件开始编写自己的扩展程序。首先，您可以打开开发者模式。
    - 单击扳手图标并从工具菜单选择扩展程序。如果在“开发者模式”右边有一个“+”号，单击“+”号让它变成“-”号。现在您可以重新载入扩展程序、载入未打包的目录中的文件，就像载入已打包的扩展程序那样，还有其它功能。有关完整的教程，请参见入门。

.. _chapterFAQ-nomo3:

为Chrome浏览器编写扩展程序时需要用到哪些技术？:
    编写扩展程序与开发者创建网站一样，使用相同的标准网络技术。HTML用于内容标记语言，CSS用于格式化，JavaScript用于脚本。由于Chrome浏览器支持HTML5和CSS3，开发者可以在扩展程序中使用最新的网络技术，例如<canvas>和CSS动画。扩展程序也可以访问几个JavaScript API，帮助进行诸如JSON编码以及与浏览器交互的功能。


.. _chapterFAQ-nomo4:


扩展程序是不是每一次浏览器载入时都要从网上获取？:
    扩展程序在安装时由Chrome浏览器下载，以后从本地磁盘上运行，以提高性能。然而，如果扩展程序的新版本上传到网上，将会在后台自动下载下来，给所有安装了这一扩展程序的用户。扩展程序也可以在任何时候请求远程内容，与网络服务交互或从网上获取内容。


.. _chapterFAQ-nomo5:

我应该如何确定Chrome浏览器版本与分支间的对应关系？:
    - 要确定Chrome的不同版本当前在各个不同平台上是否可用，请参见omahaproxy.appspot.com。
    - 在那一站点上您将会看到类似于如下形式的数据： 

    ::

        cf,dev,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        cf,beta,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        cf,stable,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        linux,dev,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        linux,beta,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        linux,stable,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        mac,dev,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        mac,beta,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        mac,stable,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        win,canary,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        win,dev,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        win,beta,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        win,stable,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        cros,dev,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####
        cros,beta,#.#.###.#,#.#.###.#,mm/dd/yy,mm/dd/yy,#####,#####,#####


    - 每一行代表不同平台和分支的组合信息。列出的平台包括cf（Google Chrome Frame）、linux、mac、win和cros（Google Chrome OS）。列出的分支包括canary、dev、beta和stable。分支后面分成四部分的数是部署至相应平台、分支组合的当前和前一个Chrome浏览器的版本号。剩下的信息是一些元数据，有关发行版最早开始的时间以及与每一次编译相关的修订版本。



扩展程序的能力:


.. _chapterFAQ-ext1:

扩展程序能否发起跨域名Ajax请求？:
    可以。扩展程序能够发出跨域名请求，有关更多信息，请参见这一页面。

.. _chapterFAQ-ext2:

扩展程序能否使用第三方网上服务？:
    可以。扩展程序能够发出跨域名Ajax请求，所以它们能够直接调用任何远程的API。以JSON格式提供数据的API特别使用起来特别方便。

.. _chapterFAQ-ext3:

扩展程序能否编码/解码JSON数据？:
    可以。因为V8（Chrome浏览器的JavaScript引擎）本地支持JSON.stringify和JSON.parse，您可以在您的扩展程序中使用这些函数，如这一页面（英文）所述，而不用在您的代码中包含任何额外的JSON库。


.. _chapterFAQ-ext4:


扩展程序能否在本地存储数据？:
    可以。扩展程序可以使用localStorage来永久地存储数据。使用Chrome浏览器内建的JSON函数，您可以在localStorage中存储复杂的数据结构。对于需要在存储的数据上执行SQL查询的扩展程序，Chrome浏览器实现了客户端SQL数据库，您也可以使用。


.. _chapterFAQ-ext5:

扩展程序能否使用OAuth？:
    可以。某些扩展程序就使用OAuth访问远程数据API，大部分开发者会觉得使用某个JavaScript OAuth库会更方便，这样可以简化发送OAuth请求的过程。

.. _chapterFAQ-ext6:

扩展程序能否加载DLL？:
    - 可以，通过NPAPI接口。然而由于可能的滥用行为，我们在Chrome网上应用店中托管您的扩展程序前要先审核。

.. _chapterFAQ-ext7:

扩展程序能否在呈现的网页外创建用户界面？:
    - 可以。您的扩展程序可以向Chrome浏览器的用户界面添加按钮，有关更多信息请参见浏览器按钮和页面按钮。
    - 扩展程序也可以创建弹出通知，在浏览器窗口外存在。有关更多细节请参见桌面通知文档。

.. _chapterFAQ-ext8:

扩展程序能否监听Chrome标签页以及导航按钮的点击？:
    不能。扩展程序仅限于监听API文档中描述的事件。

.. _chapterFAQ-ext9:

两个扩展程序能否互相通信？:
    可以。扩展程序能够向其它扩展程序传递详细，有关更多信息请参见消息传递文档。

.. _chapterFAQ-ext10:

扩展程序能否使用Google Analytics（分析）？:
    可以。由于扩展程序就像网站一样，它们可以使用Google Analytics（分析）来跟踪使用情况。然而，我们强烈建议您修改所有追踪代码，使用HTTPS版本的Google Analytics（分析）库。有关如何这么做的更多信息请参见这一教程。

.. _chapterFAQ-ext11:

扩展程序能否修改 `chrome://` 协议的URL？:
    - 不能。扩展程序API的设计尽量减少新版本的浏览器出现时可能出现的向后兼容问题。
    - 如果允许 `chrome://` URL上的内容脚本，开发者可能会依赖于这些页面上的DOM、CSS和JavaScript保持不变。
    - 在最好的情况下，那些页面不能像现在这样迅速更新。
    - 在最坏的情况下，这意味着更新这些页面中的某一个可能导致某个扩展程序无法正常工作，以至于使用那一扩展程序的用户的浏览器停止工作。
    - 替换托管于这些URL中的内容是允许的，因为这样扩展程序的开发者不得不实现他们需要的所有功能，而不会依赖于浏览器的内部实现 保持不变。

.. _chapterFAQ-ext12:

扩展程序能否在没有用户交互的情况下打开浏览器/页面按钮的弹出内容？:
    不能。弹出内容只有当用户单击相应的页面/浏览器按钮时才能打开，扩展程序不能以编程方式打开自己的弹出内容。

.. _chapterFAQ-ext13:

扩展程序能否在用户单击其它地方后仍然使弹出内容保持打开状态？:
    不能。当用户将焦点移至弹出内容外的其它浏览器区域时，弹出内容会自动关闭，没有办法在用户单击其它地方后仍然保持弹出内容打开。

.. _chapterFAQ-ext14:

扩展程序能否在安装和卸载时得到通知？:
    不能。扩展程序没有可以监听的事件，来确定是否已经安装或卸载。然而，扩展程序可以确定是否是第一次运行。有关信息请参见这一常见问题。


开发:

.. _chapterFAQ-dev1:

我应该如何为我的扩展程序建立用户界面？:
    扩展程序使用HTML和CSS定义它们的用户界面，所以您可以使用标准表单控件来建立您的用户界面，或者用CSS格式化您的用户界面，就像网页中一样。另外，扩展程序可以向Chrome浏览器本身添加有限的用户界面元素。

.. _chapterFAQ-dev2:

我能够在本地存储中可以储存多少数据？:
    - 扩展程序最多可以在本地存储中储存 `5MB` 数据。

.. _chapterFAQ-dev3:

我应该如何为我的应用程序创建一个选项菜单？:
    您可以通过创建一个选项页面让用户为您的扩展程序设置选项。选项页面是一个简单的HTML页面，当用户单击您的扩展程序的选项按钮时载入。这一页面可以从本地存储中读写数据，或者将选项发送至网络服务器，以便在不同的浏览器中使用。

.. _chapterFAQ-dev4:

扩展程序的开发人员可以使用哪些调试工具？:
    Chrome浏览器内建的开发人员工具可以用来调试扩展程序和网页。有关更多信息请参见这一有关调试扩展程序的教程。

.. _chapterFAQ-dev5:

为什么通配符匹配对于顶级域名（TLD）不适用？:
    - 您不能使用类似于 `http://google.*/*` 来匹配顶级域名（TLD）（像http://google.es和http://google.fr），这是由于将这一匹配表达式限制在期望的域名中的复杂性导致的。
    - 对于 `http://google.*/*` 的例子，Google的域名可以匹配，但是http://google.someotherdomain.com也可以。
    - 另外，许多站点并不拥有它们域名的所有顶级域名（TLD）。例如，假定您想使用 `http://example.*/*` 匹配 http://example.com和http://example.es，但是http://example.net是一个恶意站点。如果您的扩展程序有漏洞，恶意站点可能攻击您的扩展程序，通过您的扩展程序获得提升的特权。
    - 您应该显式地列出所有您想在上面运行您的扩展程序的顶级域名（TLD）。



.. _chapterFAQ-dev6:

为什么当我的扩展程序安装或卸载时管理API不产生事件？:
    管理API是为了帮助创建替代新标签页的扩展程序，而不是为了为当前扩展程序产生安装/卸载事件。




.. _chapterFAQ-dev7:

扩展程序如何确定是否是第一次运行？:
    - 扩展程序可以通过检查本地存储中某一值是否存在来确定是否是第一次运行，如果不存在的话写入这一值。
    - 例如： 

::

    var firstRun = (localStorage['firstRun'] == 'true');
    if (!firstRun) {
      localStorage['firstRun'] = 'true';
    }

    - 注意，这一检查应该在后台页面而不是内容脚本中运行。



调试:


.. _chapterFAQ-deb1:

更改皮肤中的文件后再次通过“载入正在开发的扩展程序”不能更新皮肤？:
    删除皮肤根目录的Cached Theme.pak文件。通过“载入正在开发的扩展程序”第一次载入皮肤时，猎豹会在皮肤的根目录生成一个Cached Theme.pak文件，它是猎豹为了加快皮肤渲染速度而将皮肤文件打包成一个.pak文件。当再次载入皮肤文件时，猎豹默认先加载此打包文件，判断皮肤是否有修改。如果只是修改皮肤的配置文件或者图片但此打包文件还是原来的话，猎豹会认为此皮肤未修改。


.. _chapterFAQ-deb2:

打包皮肤文件时报错“猎豹4.0暂不支持非官方皮肤”？:
    使用猎豹4.0或者以上版本来打包皮肤文件。由于猎豹升级到4.0后对 manifest.json 配置文件进行了优化升级，故不能兼容旧版的猎豹皮肤。请按照文档的说明来升级皮肤的manifest.json文件。

请求新特性和报告问题:



.. _chapterFAQ-ask1:

我认为我发现了一个bug！我应该做什么确保让它被修复？:
    - 当您开发扩展程序时，您可能发现不匹配扩展程序文档的行为，而这有可能是Chrome浏览器中的问题导致的。建议您确保填写合适的问题报告，并向Chromium小组提供足够的信息来重现这一行为。
    - 为了确保这一点，您应该遵循如下步骤：

        #. 建立一个最小的测试扩展程序，演示您想要报告的问题。该扩展程序应该包含尽可能少的代码，只要能演示问题就行。通常应该包含100行或更少的代码。然而开发者经常发现他们不能用这种方式重现他们的问题，而这很可能意味着问题在他们自己的代码中。
        #. 在 http://www.crbug.com 的问题追踪器中搜索是否已经有人报告了类似的问题，大部分与扩展程序相关的问题在Feature=Extensions分类中。例如要查找有关chrome.tabs.executeScript函数的扩展程序问题，搜索“Feature=Extensions Type=Bug chrome.tabs.executeScript”，然后出现结果。
        #. 如果您发现了描述您的问题的bug，单击加星图标，以便在这一bug收到更新时得到通知。请注意不要用“我也有这个问题”或者问“什么时候修复？”来回复这一bug，这样的更新可能会导致几百封邮件的发送。只有当您要提供可能有帮助的信息（例如更好的测试案例或建议的修复）时才添加评论。
        #. 如果您没有找到合适的问题来加星，在http://new.crbug.com填写新的问题报告。当填写这一表格时尽量明确：选择描述性的标题，解释重现问题的步骤，并描述预期的以及实际的行为。将您的测试例子添加为附件，如果合适的话添加屏幕截图。您的报告越容易让别人重现您的问题，您的问题越有可能尽早修复。
        #. 等待问题更新。大部分新的问题会在一周内鉴别分类，尽管有时候可能要花更长的时间更新。不要回复问题，问这一问题何时修复。如果您的问题在两周后还没有修改，请向讨论组发送消息，附上您的问题的链接。
        #. 如果您原来在讨论组上报告了您的问题，并重定向至这一常见问题项，回复您原来的帖子，附上您加星或报告的问题的链接。这将会使遇到同样问题的其他人找到正确的bug。



.. _chapterFAQ-ask2:

我想请求新特性！我应该如何报告？:
    - 如果您想到一个新功能（尤其是有关实验性API的），增加后可以提高扩展程序开发体验，确保合适的请求在问题追踪器中提交。
    - 为了确保这一点，您应该遵循如下步骤：

        #. 在http://www.crbug.com中的问题追踪器中搜索，看看有没有人已经请求了类似的特性。大部分有关于扩展程序的请求在Feature=Extensions分类中。例如要想寻找有关键盘快捷键的扩展程序特性请求，搜索“Feature=Extensions Type=Feature shortcuts”，然后出现结果。
        #. 如果您发现了匹配您的请求的内容，单击加星图标，以便在这一请求更新时得到通知。不要回复“我也是这么想的”或询问“什么时候实现？”，这样的更新可能导致几百封邮件的发送。
        #. 如果您没有找到合适的内容来加星，在http://new.crbug.com中填写新的请求。当填写这一表格时尽可能详细：选择描述性的标题，并准确描述您想要的特性以及您计划如何利用它。
        #. 等待请求更新。大部分新请求将会在一周内分类，尽管有时候可能需要更长的时间更新。不要直接回复请求，询问这一特性什么时候添加。如果您的请求在两周后还没有更新，请向讨论组发送消息，附上您的请求的链接。
        #. 如果您原来在讨论组上报告了您的请求，并重定向至这一常见问题项，回复您原来的帖子，附上您加星或提出的请求的链接。这将会使具有同样请求的其他人找到正确的内容。


 
