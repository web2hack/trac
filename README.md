持续更新，谢谢反馈……



2013/3/5

----------------------------------------------

p29的“默认情况下，这样的跨域无法带上目标域的会话（Cookies等）”与p85的“利用AJAX？不行，它禁止跨域传输数据”。

这两句的说法有问题，在新一代浏览器下，通过AJAX跨域（CORS）带上Cookies是可以的，这个具体解释待我抽空写篇文章。



2013/2/28

----------------------------------------------

p342，下面这句话引起了争议：

还有一种糟糕的子域设计是新浪微博，主内容都在顶级域下（weibo.com），大量的子域提供不同的业务，任何一个子域有XSS，都可以轻易跨到顶级域下。

解决请看：http://evilcos.me/?p=251




以下小改动已经在“2013年3月第2次”印刷中解决

----------------------------------------------

p2~3里的4处desc改为desc1（原因是：desc是MySQL的保留字）

p11与p359的读者改为大家（大家更亲切:)）

p31的var src = http://www.evil.com/steal.php;改为var src = "http://www.evil.com/steal.php";

p32的var src = http://www.evil.com/steal.php;改为var src = "http://www.evil.com/steal.php";

p130的1" onmouserover=alert(1) type="text改为1" onmouseover=alert(1) type="text

p130的<input value="1"onmouserover=alert(1) type="text" type="hidden" />改为<input value="1" onmouseover=alert(1) type="text" type="hidden" />

p73的熏染改为渲染

p338有两处的熏染改为渲染
