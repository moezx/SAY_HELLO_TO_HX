# SAY HELLO TO HX

### 0. Demo
![demo](https://i.imgur.com/reodkNt.png)

### 1. 介绍
SAY HELLO TO HX 是一个简单的HTML程序。

其作用为：实现 QQ、微信、微博 的加好友（关注）二维码的合并。

**即：用户只需要扫描同样的二维码，即可在以上客户端内直接前往目标用户页面。**

### 2. 原理
通过浏览器UserAgent判定用户所处的客户端，跳转至相关的页面。

其中微信无法实现通过URL直接到达用户页面，必须在网页内再次扫码。

### 3. 工作流程

用户扫码 —— 判断用户UA —— 跳转至相关页面 —— 用户进行加好友、关注等操作

如果是微信：用户扫码 —— 判断用户UA为微信 —— 利用api生成二维码 —— 跳转至相应二维码页面并提示用户长按二维码 —— 跳转至相关页面 —— 用户进行加好友、**拉黑**等操作

### 4.更多说明
如果看到这里你还是一脸懵逼不知道怎么实现你自己的个人自定义二维码页面，请前往 惶心 | 技术博客 阅读教程。

------

>* 源码修改自孟坤博客（MKBLOG.CN）
>* 如有可能请尽量保留版权信息。版权信息以代码注释的形式存在，并不会被访客看到。
>* 保留版权信息仅仅会影响不足万分之一的访问速度，
>* 但是换来的却是中国开源环境的成长。
>* By惶心，Tech.Huangxin.CO.UK

------
>  我所作的修改：
> * 全面修改二维码api，替换了原来作者的liantu.com（联图）api，使用百度云api进行代替，在中国大陆达到最快的访问速度。
> * 备用api使用了lwl12.com的api，lwl在国内访问速度也不错（肯定没有百度好），但是可以用来备用。不过几乎不需要启用（除非百度的api失效了）。
> * 替代了孟坤博客“微信支付”一类的图片，改成了“微信”。




### [前往 惶心 | 技术博客](https://tech.huangxin.co.uk/)
