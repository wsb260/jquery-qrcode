# jquery.qrcode.js

<a href='http://jeromeetienne.github.com/jquery-qrcode'>jquery.qrcode.js</a>
is *jquery plugin for a pure browser qrcode generation*.
It allow you to easily add qrcode to your webpages.
It is standalone, less than 4k after minify+gzip, no image download.
It doesnt rely on external services which go on and off, or add latency while loading.
It is based on a <a href='http://www.d-project.com/qrcode/index.html'>library</a>
which build qrcode in various language. <a href='http://jeromeetienne.github.com/jquery-qrcode'>jquery.qrcode.js</a> wraps
it to make it easy to include in your own code.

Show, don't tell, here is a <a href='https://github.com/jeromeetienne/jquery-qrcode/blob/master/examples/basic.html'>example</a>

## How to Use It

Let me walk you thru it. First include it in your webpage with the usual script tag
    
    <script type="text/javascript" src="jquery.qrcode.min.js"></script>

Then create a DOM element which gonna contains the generated qrcode image. Lets say
a div

    <div id="qrcode"></div>

Then you add the *qrcode* in this container by

    jquery('#qrcode').qrcode("this plugin is great");

This is it. see it <a href='examples/basic.html'>live</a>.

You can set the height and width of the generated qrcode:

    jquery('#qrcode').qrcode({width: 64,height: 64,text: "size doesn't matter"});


## Conclusion
<a href='http://jeromeetienne.github.com/jquery-qrcode'>jquery.qrcode.js</a> is available on github
<a href='https://github.com/jeromeetienne/jquery-qrcode'>here</a>
under <a href='https://github.com/jeromeetienne/jquery-qrcode/blob/master/MIT-LICENSE.txt'>MIT license</a>.
If you hit bugs, fill issues on github.
Feel free to fork, modify and have fun with it :)

 动态生成二维码插件 jquery.qrcode.js

前段时间做项目，需要动态生成一个二维码，于是就在网上找了一下发现一个jquery插件jquery.qrcode.js，所以今天就简单说一下这个插件的使用：

 

jquery.qrcode.js是依赖jquery的,所以要先引入jquery再引入jquery.qrcode.js

<script type='text/javascript' src='js/jquery.min.js'></script>
<script type="text/javascript" src="js/jquery.qrcode.min.js"></script>

 

在页面上添加一个div标签，用于创建渲染区域

<div id="qrcode"></div>

 

通过下面代码就可以生成一个默认256×256大小的二维码

<script type="text/javascript">
    jQuery('#qrcode').qrcode("http://www.cnblogs.com/HtmlCss3/");
</script>


