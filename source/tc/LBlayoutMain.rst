.. include:: ../LINKS.rst

.. _chapterLBlayoutMain:


猎豹 layout_main 详解
==============================================================================

什么是 layout_main 文件
------------------------------------------------------------------------------

在猎豹浏览器的皮肤文件中，一个有三个配置文件，分别是：图片显示文件（manifest.json）、图片定位文件（layout_main）、图片参数文件（layout_parameter）。
其中 layout_main 主要记录的是浏览器在最大化、标准化状态时，各个控制部分的位置。






demo: clasc's layout_main
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: xml
  :emphasize-lines: 2-5,219,246-253

    <?xml version="1.0" encoding="UTF-8"?>
    <layout>
    <layout_normal>
      <list>
        <list id="control_area">
            <list direction="horizontal">
            <view id="icon_btn" width="60" relative="left_top" delta="9 9"/>
            <list proportion="100">
                <list direction="horizontal">
                  <view id="title_bar" preferred_size="fixed_height" height="29" margin="0 0 0 -3" proportion="100"/>
                  <view id="mainmenu_bar"/>
                  <view id="syscmd_bar"/>
                </list>
                <list direction="horizontal" relative="left_bottom" delta="0 2">
                    <view id="fav_menu_btn" margin="5 0 -18"/>
                    <view id="home_btn"/>
                    <view id="reload_btn" margin="-18"/>
                    <list direction="horizontal" align="vertical" proportion="100">
                      <padding width="6"/>
                      <view id="back_btn" margin="0 6"/>
                      <view id="forward_btn" margin="0 6"/>
                      <view id="tool_bar" preferred_size="fixed_height" height="30" proportion="100"/>
                      <list direction="horizontal">
                        <padding width="4"/>
                        <view id="safe_btn" margin="0 6"/>
                        <padding width="4"/>
                        <view id="login_magr_btn" margin="0 6"/>
                        <padding width="4"/>
                        <view id="download_btn" />
                        <padding width="4"/>
                      </list>
                    </list>
              </list>
            </list>        
            </list>
            <view id="bookmark_bar" margin="5 -6"/>
            <list direction="horizontal">
                <view id="tab_bar" margin="10 2" proportion="100"/>
          <view id="multi_tab_btn" margin="0 2 -2" preferred_size="fixed_height" width="27"/>
          <view id="undo_btn" margin="0 2 11" preferred_size="fixed_height" height="27"/>
            </list>
            <view id="tab_separator" margin="0 -2" preferred_size="fixed" height="4" proportion="100"/>
        </list>
        <list id="content_area" proportion="100">
          <view id="find_bar"/>
          <view id="info_bar"/>
          <view id="tab_content" proportion="100"/>   
        </list>
        <view id="status_bar"/>
      </list>
    </layout_normal>
    <layout_max>
      <list>
        <list id="control_area">
            <list direction="horizontal">
            <view id="icon_btn" width="60" relative="left_top" delta="10 9"/>
            <list proportion="100">
                <list direction="horizontal">
                  <view id="title_bar" margin="0 0 0 -3" preferred_size="fixed_height" height="29" proportion="100"/>
                  <view id="mainmenu_bar"/>
                  <view id="syscmd_bar"/>
                </list>
                <list direction="horizontal" relative="left_bottom" delta="0 2">
                    <view id="fav_menu_btn" margin="5 0 -18"/>
                    <view id="home_btn"/>
                    <view id="reload_btn" margin="-18"/>
            <list direction="horizontal" align="vertical" proportion="100">
              <padding width="6"/>
              <view id="back_btn" margin="0 6"/>
              <view id="forward_btn" margin="0 6"/>
              <view id="tool_bar" preferred_size="fixed_height" height="30" proportion="100"/>
              <list direction="horizontal">
                <padding width="4"/>
                <view id="safe_btn" margin="0 6"/>
                <padding width="4"/>
                <view id="login_magr_btn" margin="0 6"/>
                <padding width="4"/>
                <view id="download_btn" />
                <padding width="4"/>
              </list>
            </list>
              </list>
            </list>        
            </list>
            <view id="bookmark_bar" margin="5 -6"/>
            <list direction="horizontal">
                <view id="tab_bar" margin="10 2" proportion="100"/>
          <view id="multi_tab_btn" margin="0 2 -2" preferred_size="fixed_height" width="27"/>
          <view id="undo_btn" margin="0 2 11" preferred_size="fixed_height" height="27"/>
            </list>
            <view id="tab_separator" margin="0 -2" preferred_size="fixed" height="4" proportion="100"/>
        </list>
        <list id="content_area" proportion="100">
          <view id="find_bar"/>
          <view id="info_bar"/>
          <view id="tab_content" proportion="100"/>
        </list>
        <view id="status_bar"/>
      </list>
    </layout_max>
    <layout_full>
      <list>
        <list id="control_area">
          <view id="title_bar" preferred_size="fixed"/>
          <view id="icon_btn" preferred_size="fixed"/>
          <view id="undo_btn" preferred_size="fixed"/>
          <view id="tab_bar" preferred_size="fixed"/>
          <view id="syscmd_bar" preferred_size="fixed"/>
          <view id="bookmark_bar" preferred_size="fixed"/>
          <view id="tab_separator" preferred_size="fixed"/>
        </list>
        <list id="content_area" proportion="100">
          <view id="find_bar"/>
          <view id="info_bar"/>
          <view id="tab_content" proportion="100"/>
        </list>
      </list>
    </layout_full>
    </layout>