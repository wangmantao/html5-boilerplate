[HTML5 Boilerplate homepage](https://html5boilerplate.com/) | [Documentation
table of contents](TOC.md)

# JavaScript

项目中默认的js文件信息

## main.js

可在这个文件中引用你所需要的js文件或js code.
你可以替换掉整个main.js

## plugins.js
这个文件可以包含所有你需要的插件。jquery 或其它的第三方脚本

方法：把jquery插件放在(function($){....})(jquery) 闭包中.
One approach is to put jQuery plugins inside of a `(function($){ ...
})(jQuery);` closure to make sure they're in the jQuery namespace safety
blanket.
 Read more about [jQuery plugin
authoring](https://learn.jquery.com/plugins/#Getting_Started).

一般该文件只包括小的脚存文件，是为了防止console错误而缺少console.
所写的脚本要注意：一个console方法不可用了，这个方法是空的函数数值，避免浏览器抛出错误。

## vendor

这个目录是放置第三方库的
This directory can be used to contain all 3rd party library code.

Minified versions of the latest jQuery and Modernizr libraries are included by
default. You may wish to create your own [custom Modernizr
build with the online builder](https://www.modernizr.com/download/) or [command
line tool](https://modernizr.com/docs#command-line-config).
