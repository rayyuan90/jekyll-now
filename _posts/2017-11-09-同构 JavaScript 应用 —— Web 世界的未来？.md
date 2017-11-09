
# 同构 JavaScript 应用 —— Web 世界的未来？

<div class="PostIndex-author">[![范洪春](https://pic4.zhimg.com/50/v2-e95960200c6a9c3661f74abd07c0b5ff_xs.jpg)](https://www.zhihu.com/people/fanhc)[范洪春](https://www.zhihu.com/people/fanhc)<span class="Bull"></span>

<div class="HoverTitle" data-hover-title="Wed, Mar 11, 2015 8:20 AM"><time datetime="Wed Mar 11 2015 08:20:35 GMT+0800 (CST)">3 years ago</time></div>

</div>

</div>

<div class="RichText PostIndex-content av-paddingSide av-card">

Web 世界有一个至理名言，就是 Java 提出的“Write once, run everywhere”。但这句话只适用于 Java 么？我们能否也用它来形容 JavaScript 呢？答案是 Yes。

我将会在这篇文章中介绍同构 JavaScript 应用的概念，并推荐一些资源帮助你构建此类应用。

## 一路走来  

多年以前，web 只是一些由 HTML 和 CSS 搭建的静态页面，没有太多的交互。用户的每一个动作都需要服务器来创建并返回一个完整的页面。幸而有了 JavaScript，开发者开始创建很棒的效果，不过 Ajax 的到来才是这场革新的真正开始。Web 开发者开始编写能够与服务端进行交互，且在不重载页面的情况下向服务端发送并接受数据的页面。

随着时间的推移，客户端代码可以做的事情越来越多，催生了被称作单页面应用（SPA）的一类应用。SPA 在首次加载页面时就获取了所有必需的资源，或者再按需动态加载并且渲染到页面上。 [Gmail](http://link.zhihu.com/?target=https%3A//mail.google.com/) 和 [StackEdit editor](http://link.zhihu.com/?target=https%3A//stackedit.io/editor) 是很棒的 SPA 示例。

SPA 准许重度的交互设计，因为几乎所有的操作都在客户端执行，保持最低限度地与服务端进行交流。不幸的是，它们也存在一些严重的问题，我们选择几个进行讨论。

## 性能

因为相对于静态页面，SPA 需要更多的客户端代码，需要下载数据的体积也更大。这使得手机加载速度很慢，可能会导致一些极端的状况 —— 比如糟糕的用户体验以及收入上的损失等。依据 [Microsoft](http://link.zhihu.com/?target=http%3A//blogs.msdn.com/b/ie/archive/2014/10/08/http-2-the-long-awaited-sequel.aspx) 的一篇文章 ——

> Bing 的一项研究表明：页面的加载时间每增加 10ms，站点年度总收入就会减少 $250K。

## SEO

因为单页面应用依赖于 JavaScript 的执行，服务器不会提供它们可能用到的任何 HTML 内容。因此，web 爬虫很难去索引到这些页面。爬虫就是可以向 web 服务器发送请求，并且将结果分析成原始文本的程序，而不需要像一个浏览器运行 JavaScript 那样解释和执行客户端的内容。不久前，[Google 优化了搜索引擎的 web 爬虫](http://link.zhihu.com/?target=http%3A//googlewebmastercentral.blogspot.co.uk/2014/05/understanding-web-pages-better.html)，现在它也可以抓取基于客户端 JavaScript 所构建的页面了。但是 Bing、Yahoo 以及其他搜索引擎怎么办？一个好的索引对任何公司来说都至关重要，它通常会带来更多的流量以及更高的回报。

## 同构 JavaScript 应用

同构 JavaScript 应用基于 JavaScript 编写，可以在客户端和服务端运行。正因为此，你只需要写一次代码，就可以在服务端渲染静态页面，还可以在客户端完成复杂的交互。所以，这种方式互通了两个世界，并且避免了前面提到了两个问题。

现在，有很多框架可以帮助你开发这类应用。其中最著名的一个可能是 [Meteor](http://link.zhihu.com/?target=https%3A//www.meteor.com/)。Meteor 是一个开源 JavaScript 框架，基于 Node.js 编写，专注于实时 web 应用。我想提到的另一个项目是 [Rendr](http://link.zhihu.com/?target=http%3A//rendrjs.github.io/rendr/)，它是 [Airbnb 开发](http://link.zhihu.com/?target=http%3A//nerds.airbnb.com/weve-launched-our-first-nodejs-app-to-product)的一款轻量级类库，准许同时在客户端和服务端运行 Backbone.js。

越来越多的公司将 Node.js 应用到他们的产品中。客户端和服务端的代码共享成为一个更加普通而自然的选择。在我看来，这种做法将是 web 开发的未来。有些类库通过共享模板又增强了这一趋势，比如 [React](http://link.zhihu.com/?target=http%3A//facebook.github.io/react/)。

## 结论

这篇文章介绍了同构 JavaScript 应用的概念，它是应用开发的一种全新方式，可以最大限度地结合服务端和客户端应用程序。我们还讨论了运用这种方式尝试解决的问题，以及你现在就可以参与实践的一些项目。

你听说过同构 JavaScript 应用么？你开发过么？你有开发经验么？

原文：[Isomorphic JavaScript Applications — the Future of the Web?](http://link.zhihu.com/?target=http%3A//www.sitepoint.com/isomorphic-javascript-applications/)



