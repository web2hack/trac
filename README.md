《Web前端黑客技术揭秘》勘误表，持续更新，谢谢反馈……

2013/9/24（重大更新）
----------------------------------------------
以下bugs都将在“2013年10月”台湾上市的《Web 2.0 駭客技術揭秘》中解决，感谢小伙伴们:)

2013/6/25
----------------------------------------------
<pre>
p183第七行：
&lt;a href=&quot;#&quot; onclick=&quot;do_some_func('',function(){alert(1);alert(2);},'')&quot;&gt;test&lt;/a&gt;
应该改为：
&lt;a href=&quot;#&quot; onclick=&quot;do_some_func('',function(){alert(1);alert(2);}(),'')&quot;&gt;test&lt;/a&gt;

感谢：Ay暗影的一而再的耐心反馈
</pre>

2013/6/7
----------------------------------------------
<pre>
p282倒数第三行的replacdState()改为replaceState()

感谢：@lovelessyuyu反馈
</pre>

2013/4/17
----------------------------------------------
<pre>
p60页下面这段：
1）allowNetworking
该参数控制Flash文件的网络访问功能，它有三个值：all（所有的网络API都可用）、internal（默认值，除了不能使用浏览器导航和浏览器交互的API外，如navigate ToURL、fscommand、ExternalInterface.call等，其他的都可用）、none（所有的网络API都不可用）。

有个错误，allowNetworking的默认值应该是all，而不是internal。
这个错误不影响本书的一些结论。

感谢：TSRC的mulu反馈
</pre>

2013/3/8
----------------------------------------------
<pre>
p182的&lt;a href=&quot;#&quot; onclick=&quot;do_some_func(\&quot;&lt;?=$_GET['a']?&gt;\&quot;)&quot;&gt;test&lt;/a&gt;改为：
&lt;a href=&quot;#&quot; onclick=&quot;do_some_func('&lt;?=$_GET['a']?&gt;')&quot;&gt;test&lt;/a&gt;
p183第三行的"do_some_func(",alert(1),")"改为"do_some_func('',alert(1),'')"

修改原因：单引号双引号弄混淆了，我眼花了。

还得注意：测试时关闭PHP的magic_quotes_gpc（设置php.ini的magic_quotes_gpc = Off）。

感谢：@muhuohacker反馈
</pre>

2013/3/5
----------------------------------------------
<pre>
p29的“默认情况下，这样的跨域无法带上目标域的会话（Cookies等）”与p85的“利用AJAX？不行，它禁止跨域传输数据”。

这两句的说法有问题，在新一代浏览器下，通过AJAX跨域（CORS）带上Cookies是可以的，这个具体解释待我抽空写篇文章。

感谢：xi4oyu反馈
</pre>

2013/2/28
----------------------------------------------
<pre>
p342，下面这句话引起了争议：

还有一种糟糕的子域设计是新浪微博，主内容都在顶级域下（weibo.com），大量的子域提供不同的业务，
任何一个子域有XSS，都可以轻易跨到顶级域下。

解决请看：http://evilcos.me/?p=251

感谢：sogl反馈
</pre>

以下小改动已经在“2013年3月第2次”印刷中解决
----------------------------------------------
<pre>
p2~3里的4处desc改为desc1（原因是：desc是MySQL的保留字）

p11与p359的读者改为大家（大家更亲切:)）

p31的var src = http://www.evil.com/steal.php;改为var src = "http://www.evil.com/steal.php";

p32的var src = http://www.evil.com/steal.php;改为var src = "http://www.evil.com/steal.php";

p130的1" onmouserover=alert(1) type="text改为1" onmouseover=alert(1) type="text

p130的&lt;input value=&quot;1&quot;onmouserover=alert(1) type=&quot;text&quot; type=&quot;hidden&quot; /&gt;改为：
&lt;input value=&quot;1&quot; onmouseover=alert(1) type=&quot;text&quot; type=&quot;hidden&quot; /&gt;

p73的熏染改为渲染

p338有两处的熏染改为渲染
</pre>

感谢反馈的同学们
