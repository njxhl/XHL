# 调用方法

1.引入js文件
`<script type="text/javascript" src="tabulous.js"></script>`

2.html格式

    <div id="tabs">
            <ul>
                <li><a href="#tabs-1" title="">Tab 1</a></li>
                <li><a href="#tabs-2" title="">Tab 2</a></li>
                <li><a href="#tabs-3" title="">Tab 3</a></li>
            </ul>
            <div id="tabs_container">
                <div id="tabs-1">
                    <!--tab content-->
                </div>
                <div id="tabs-2">
                     ? <!--tab content-->
                </div>
                <div id="tabs-3">
                     ? ?<!--tab content-->
                </div>
            </div><!--End tabs container-->
    </div><!--End tabs-->

3.js初始化调用

    $(document).ready(function ($) {
     	 $('#tabs').tabulous({);
    });

4.插件效果设置

    $('#tabs').tabulous({
    	effect: 'scale'
    });