.. include:: ../LINKS.rst

.. _chapterLBlayoutParameter:


猎豹 layout_parameter 详解
==============================================================================






demo: clasc's layout_parameter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: json
  :emphasize-lines: 2-5,219,246-253


    {
      "border_thickness_pseudo": "1",
      "browser_min_size": "500 250",

      "logo_tip_offset": "-6 0",
      "logo_flicker_offset": "-10 -8",
      "logo_mask_offset": "0 0",
　　  正常窗口下头像蒙版位置
　　  "logo_mask_max_offset": "0 3",
　　  最大化下头像蒙版位置
　  　"logo_animation_rotate_frames": "36",
　　  登录动画帧数
　  　"logo_animation_rotate_duration": "1000",
　  　登录动画速度 
　  　"logo_animation_breath_frames": "18",    
　  　云同步动画帧数
　  　"logo_animation_breath_duration": "1000",
　  　云同步动画速度 

　  　"wrench_menu_offset": "0 7",
　  　按下logo后显示菜单的位置
　  　"wrench_menu_titlecontent_offset": "100 0",
　  　菜单下用户账号显示位置  

　　  "logo_animation_breath_offset": "0 0",
　　  正常窗口下登录动画位置，以”a空格b”表示位置，a越大越向右，b越大越向下，以屏幕最上角为原点。
　　  "logo_animation_breath_max_offset": "0 0 ",
　  　最大化下登录动画位置，以”a空格b”表示位置，a越大越向右，b越大越向下。
　　  "logo_animation_rotate_offset": "0 0",
　　  正常窗口下云同步动画位置，以”a空格b”表示位置，a越大越向右，b越大越向下。
      "logo_animation_rotate_max_offset": "0 0",
　  　最大化下云同步动画位置，以”a空格b”表示位置，a越大越向右，b越大越向下。


      "tab_horz_fuzz": "10",
      "tab_vert_fuzz": "7",
      "inactive_tab_horizon_offset": "-1",
      非活动选项卡间的间距，数值越大间距越小
      "active_tab_horizon_offset": "-1",
      活动选项卡间的间距，数值越大间距越小
      "hittest_as_noclientarea": "false",

      "show_caption": "true",
      是否显示标题，正常情况下显示“猎豹浏览器”
      "title_hide_when_max": "false",
      最大化时标题是否隐藏
      "title_font_deltasize": "1",
      标题字体大小

      "undo_btn_has_droparrow": "true",
      最大化下是否显示恢复历史选项卡按钮，即用按钮替代右键"恢复上一个标签"按钮的功能，删除改句不显示

      "locationbar_height": "28",
      地址输入栏的高度，没特殊需求不建议修改，删除改句即为保持默认
      "loctionbar_always_show_goto": "true",
      是否一直显示”转入“按钮，即地址栏右边的向右箭头，删除删除改句不显示按钮
      "loctionbar_has_switch_core": "true",
      是否在地址栏栏显示兼容模式按钮，删除改句不显示按钮
      "locationbar_ev_bubble_top_offset": "2",
      "show_home_button": "false",
      是否显示“主页”选项

      "bookmarkbar_contents": "2 5 2",
      收藏栏内容位置，四个数字前两个代表左边主页的位置，后面两个代表“展开更多”按钮的位置，注意这个位置是联动的，即
      动了两个任意一个位置，整行都会动，第三个数字越大，左边的按钮越向左。
      "locationbar_contents": "0 1 0 1",
      与收藏栏一样，地址栏地址显示位置，第二个数值大小越大地址显示越向上。
      "searchbar_contents": "6 1 0 1",
      与地址栏一致
      "wrench_menu_btn_spacing": "1"
    }
