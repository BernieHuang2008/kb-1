# 逻辑门：与门

![res/img/AND-gate-1.webp](res/img/AND-gate-1.webp)

这就是一个非常简化的与门。

分析这个问题，需要把握一个原则。。。。

就是压差大的导通先拿掉二极管分析U0端处于高压状态。

根据以上原则，就是两个信号输入端哪个为低电平，哪个导通，另外一个不导通。

翻译过来，两个都是高电平，u0才会是高电平，否则期中一个导通就把电位拉成低电位了。

于是我们可以发现这其实是个与门。

> https://www.zhihu.com/question/31228866/answer/5113908