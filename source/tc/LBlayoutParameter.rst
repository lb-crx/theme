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
　  　"logo_animation_rotate_frames": "36",
　　  登录动画帧数
　  　"logo_animation_rotate_duration": "1000",
　  　登录动画速度 
　  　"logo_animation_breath_frames": "18",    
　  　云同步动画帧数
　  　"logo_animation_breath_duration": "1000",
　  　云同步动画速度 

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

      "locationbar_height": "28",
      地址输入栏的高度，没特殊需求不建议修改，删除改句即为保持默认
      "loctionbar_always_show_goto": "true",
      是否一直显示”转入“按钮，即地址栏右边的向右箭头
      "loctionbar_has_switch_core": "true",
      "locationbar_ev_bubble_top_offset": "2",
      "show_home_button": "false",
      是否显示“主页”选项

      "bookmarkbar_contents": "2 5 2",
      "locationbar_contents": "0 1 0 1",
      "searchbar_contents": "6 1 0 1",
      "wrench_menu_btn_spacing": "1"
    }
