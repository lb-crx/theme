.. include:: ../LINKS.rst

.. _chapterLBthemeTestSkill:


猎豹皮肤打包和调试技巧
==============================================================================

在皮肤达到完美发布之前,我们当然会进行反复的尝试,调整,
我们修改皮肤原始图片后，如果采用每次都打包然后安装的方法来调试的话，就很浪费时间和精力。现在向大家介绍一个方法来快速的调试皮肤。

下面的视频内容是如何打包和调试猎豹浏览器的皮肤文件。

.. raw:: html

	<embed src="http://player.youku.com/player.php/sid/XNjMzODIyMjgw/v.swf" allowFullScreen="true" quality="high" width="800" height="450" align="middle" allowScriptAccess="always" type="application/x-shockwave-flash"></embed>


以下是具体的打包和调试步骤:


0: 准备知识
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

pem是密钥，就像你家里面的钥匙，一把钥匙只能开一个房间，那个房间就是你的crx皮肤文件。如果你的房间装修了的话，用以前的钥匙也能打开

1: 本地目录
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
crx在猎豹中安装后，直接在它的文件目录下生成一个文件夹的，你可以直接在这个文件夹里面改

比如::

    C:\Users\Administrator\AppData\Local\liebao\User Data\Default\Extensions

2: 调试流程
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

我们在安装皮肤文件后会在浏览器中生成一个皮肤文件夹。

- 首先我们打开猎豹浏览器的安装目录。
    - 皮肤文件保存在extension文件夹中，按照时间排序，我们可以找到刚才安装好的皮肤。
- 用photoshop 打开想修订的图像文件，修改它，然后保存。
- 回到皮肤文件夹的界面，我们下一步就是删除 ``.pak`` 为后缀的文件，
- 再重启浏览器就可以看到刚才的修改了




后续
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
你可以将修改的文件替换到源皮肤文件夹中，按照刚才的步骤打包成crx皮肤。
