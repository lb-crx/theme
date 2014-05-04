.. include:: ../LINKS.rst

.. _update45:


猎豹浏览器版本升级到4.5
==============================================================================

猎豹浏览器此次更新主要是升级 `manifest.json` 配置文件中的版本号 `manifest_version` 为 `8.2` ；并增加了“更多按钮”，以及它的弹出窗口。

猎豹皮肤版本
------------------------------------------------------------------------------
猎豹皮肤版本从 `7.3` 升级到 `8.2`。

更多功能按钮
------------------------------------------------------------------------------
更多功能按钮是猎豹的新增功能，引入了“游戏助手”、“猎豹追剧”、“猎豹翻译”、“微信”、“猎豹天气”等功能；用户可以通过其自带的“自定义显示”功能来管理猎豹浏览器的其他功能按钮的显示位置（主界面或者更多功能按钮的弹出框）。

更多按钮弹出框：

.. _theme_morefunction1:
.. figure:: ../../../../_static/update-img/morefunction1.png
    :alt: 更多按钮弹出框

自定义界面按钮：

.. _theme_morefunction2:
.. figure:: ../../../../_static/update-img/morefunction2.png
    :alt: 自定义界面按钮

变更列表
------------------------------------------------------------------------------

+ `manifest_version` 从 7.2 升级到 8.2
    .. _theme_update45:
    .. figure:: ../../../../_static/update-img/update45manifest.png
+ 新增三个按钮相关配置
        .. _update_change:
        .. figure:: ../../../../_static/update-img/update45-change.png
    + "more_button_n" 书签栏更多功能按钮的普通态
        .. _theme_more_button_n:
        .. figure:: ../../../../_static/images/manifest/origin/more_button_n.png
    + "more_button_h" 更多功能按钮的鼠标悬浮态
        .. _theme_more_button_h:
        .. figure:: ../../../../_static/images/manifest/origin/more_button_h.png
    + "more_button_p" 更多功能按钮的鼠标按下态
        .. _theme_more_button_p:
        .. figure:: ../../../../_static/images/manifest/origin/more_button_p.png
    + "game_assist_n" 游戏助手按钮的普通态
        .. _theme_game_assist_n:
        .. figure:: ../../../../_static/images/manifest/origin/game_assist_n.png
    + "game_assist_h" 游戏助手按钮的鼠标悬浮态
        .. _theme_game_assist_h:
        .. figure:: ../../../../_static/images/manifest/origin/game_assist_h.png
    + "game_assist_p" 游戏助手按钮的鼠标按下态
        .. _theme_game_assist_p:
        .. figure:: ../../../../_static/images/manifest/origin/game_assist_p.png
    + "more_tv_track_n" 猎豹追剧按钮的普通态
        .. _theme_more_tv_track_n:
        .. figure:: ../../../../_static/images/manifest/origin/more_tv_track_n.png
    + "more_tv_track_h" 猎豹追剧按钮的鼠标悬浮态
        .. _theme_more_tv_track_h:
        .. figure:: ../../../../_static/images/manifest/origin/more_tv_track_h.png
    + "more_tv_track_p" 猎豹追剧按钮的鼠标按下态
        .. _theme_more_tv_track_p:
        .. figure:: ../../../../_static/images/manifest/origin/more_tv_track_p.png
+ 新增三个功能按钮在界面上的三态图片（以下图片在 manifest.json 中暂无相关配置信息）
    + 猎豹翻译按钮在主界面时的普通态
        .. _theme_translate_button_n:
        .. figure:: ../../../../_static/images/manifest/origin/translate_button_n.png
    + 猎豹翻译按钮在主界面时的鼠标悬浮态
        .. _theme_translate_button_h:
        .. figure:: ../../../../_static/images/manifest/origin/translate_button_h.png
    + 猎豹翻译按钮在主界面时的鼠标按下态
        .. _theme_translate_button_p:
        .. figure:: ../../../../_static/images/manifest/origin/translate_button_p.png
    + 微信按钮在主界面时的普通态
        .. _theme_weixin_button_n:
        .. figure:: ../../../../_static/images/manifest/origin/weixin_button_n.png
    + 微信按钮在主界面时的鼠标悬浮态
        .. _theme_weixin_button_h:
        .. figure:: ../../../../_static/images/manifest/origin/weixin_button_h.png
    + 微信按钮在主界面时的鼠标按下态
        .. _theme_weixin_button_p:
        .. figure:: ../../../../_static/images/manifest/origin/weixin_button_p.png
    + 天气按钮在主界面时的普通态
        .. _theme_weather_button_n:
        .. figure:: ../../../../_static/images/manifest/origin/weather_button_n.png
    + 天气按钮在主界面时的鼠标悬浮态
        .. _theme_weather_button_h:
        .. figure:: ../../../../_static/images/manifest/origin/weather_button_h.png
    + 天气按钮在主界面时的鼠标按下态
        .. _theme_weather_button_p:
        .. figure:: ../../../../_static/images/manifest/origin/weather_button_p.png
说明：上面说到的翻译、微信、天气按钮在配置文件中没有相对应的配置项，只适配官方皮肤库的皮肤。
+ `layout_main` 布局配置文件的优化
    + 新增名称为 button_bar 的 view 标签。此标签主要是控制“游戏助手”、“猎豹追剧”、“猎豹翻译”、“微信”和“猎豹天气”在主界面显示的功能按钮位置。
        .. _update_button_bar:
        .. figure:: ../../../../_static/update-img/button_bar.png

        .. _update_button_bar_code:
        .. figure:: ../../../../_static/update-img/button_bar_code.png
    + 更改页面元素控制边距的属性，使用 `margin` 属性 来取代 `padding` 标签。例如修改 safe_btn 的功能按钮的 margin 属性的属性值为 4，则是将安全中心功能按钮的左边距设置为4像素；如果是 `margin="0 4 4 0"`，则为左边距为0，上边距为4像素，右边距为4像素，下边距为0。下图为 layout_main 变更内容对比：
        .. _update_margin_padding:
        .. figure:: ../../../../_static/update-img/margin_padding.jpg

