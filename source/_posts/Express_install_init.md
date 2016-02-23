title: Expree 4.13.1 安装和初始化解释索引
---
> 由于网上已经有大量针对nodejs和express的解释，我觉得真的没必要重复
>
> 再写一篇，这里说是索引比较贴切，就是把看到和用过的帖子晒出来。这里想
>
> 说明一件事情，由于我朋友学习的缘故，我粗粗的翻了一下这些帖子，发现一个
>
> 针对初学者不太友好的问题，就是所有的问题或者教程都不注意引述前人的资料
>
> 或者其他网友发现的Q&A(问题集)。这个习惯真的不好，对其他人学习或者发现
>
> 问题而言真是一个坑。所以，我这里做一个索引，便于大家了解nodejs和express
>
> 的一些基本方面和联系。

---
* [Nodejs是🐴](http://www.runoob.com/nodejs/nodejs-tutorial.html)
* [NPM是什么?](http://www.cnblogs.com/chyingp/p/npm.html)
> 特别说明一点，那就是npm在nodejs工程中的结构中的意义。
>
> 个人认为基于npm构建的nodejs工程是nodejs的基本框架
>
> 包括后面说到的express。所以，npm指定的规则一定也对express有约束作用。
>
> 初学者，一般会遇到2个问题。
>
> * 第一个问题就是npm install应该在工程目录下
> 执行。切记，必须是你项目的根目录，也就是package.json所在的目录。
>
> * 第二点就是,记得依赖使用--save(对应package.json中的devDependencies字段)
> 包括 --save-dev也是一样（具体见[package.json解释](http://www.mujiang.info/translation/npmjs/files/package.json.html)）。

* [Expree是🐎](http://www.expressjs.com.cn/)
> 网站上说明的差不多能告诉一个你站在nodejs角度，express是什么。
>
> 我这里补充一点，就是说明一下从http请求－反馈的角度类比说明一下。
>
> req-handler-res (req:用户发起请求,handler:处理程序,res:http返回)
> express包裹了req和res。把handler以路由（Router[1])的方式提供出来.
>
> 所谓Router，其实就是通过匹配特定的url路径,
> 从req里面拿参数（params或者body)进行业务逻辑，然后把结果通过res的渲染函数返回给客户端。
* [Express安装(不适用express-generator的版本)](http://www.expressjs.com.cn/starter/installing.html)
> express-generator是啥？简单说，就是一个工程模版生成器，它将express标准
> 工程中的配置和初始化资源文件包括目录都给你生成好。但是本质上说，它生成的仍然
> 是一个标准的基于npm管理的nodejs工程.

* [Express(使用express-generator)](http://www.expressjs.com.cn/starter/generator.html)
> 上面，解释了生成器的作用。这里说一点，就是express工程的管理最好基于这个生成器，
> 因为这样有利于所有协作者都建立在同一种标准的基础上。这样项目结构划分hehe

* [Express路由是🐎](http://www.expressjs.com.cn/starter/basic-routing.html)


[1]: http://lostjs.com/2014/04/24/router-in-express-4/
