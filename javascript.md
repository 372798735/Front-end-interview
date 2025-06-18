## 一、掘金、微信公众号阅读记录总结
| 序号 | 文章质量五星评分 | 主题和链接 | 总结 |
| :---: | :---: | --- | --- |
| 1 | ⭐⭐ | [受控组件和非受控](https://juejin.cn/post/7363121890791227426) | 受控组件就是代码可以更改控制的值；非受控组件就是代码不能更改控制，只能由用户输入的值。 |
| 2 | ⭐⭐ | [快速删除node_modules](https://juejin.cn/post/7477926585087606820 ) | 用起来感觉差别不大，小tips可以使用更改 包名称的方式实现删除和下载同步进行 |
| 3 | ⭐⭐⭐ | [keep-alive原理](https://juejin.cn/post/7402891257196806156) | keep-alive组件的作用：keep-alive是vue内置的一个抽象组件，它主要作用是动态组件切换时，缓存不活动的组件实例，而不是销毁它们，这样做的好处是可以避免组件的重复创建和销毁，从而提高组件的性能和用户体验。<br/>keep-alive组件实现原理概述：keep-alive 组件的核心实现原理是通过维护一个缓存对象（ cache ）和一个键集合（ keys ）来管理组件实例的缓存。当组件被切换到 keep-alive 包裹的动态组件中时，会先检查缓存中是否存在该组件实例，如果存在则直接从缓存中获取并激活；如果不存在，则创建新的组件实例并添加到缓存中。当组件从 keep-alive 中移除时，不会真正销毁组件实例，而是将其状态保存起来，以便下次复用。 |
| 4 | ⭐⭐⭐ | [控制并发请求](https://juejin.cn/post/7356534347509645375) | 原理：利用Promise模拟任务队列(先进先出就是队列)，从而实现请求池效果。<br/>一般这种函数不自己封装，网上有成熟的库，比如： <font style="color:rgba(255, 255, 255, 0.8);background-color:rgb(24, 24, 24);">p-limit</font> |
| 5 | ⭐ | [前端中的file和blod两个对象](https://juejin.cn/post/7413921824066551842#heading-1) | Blod是纯粹的二进制数据，它可以存储任何类型的数据，但不具有文件的源数据(如文件名、最后修改时间等)。<br/>File继承了Blod类，所以File对象除了具有Blod的所有属性和方法外，还包含文件的元数据，如文件名和修改日期<br/>二者在文件上传和二进制数据处理的场景中被广泛使用。Blod更加通用，而File更加专注于与文件系统的交互。 |
| 6 | ⭐⭐⭐ | [强缓存和协商缓存](https://juejin.cn/post/7352075703859183667) | 强缓存：由后端在响应头设置字段：'Cache-Control': 'max-age=xxx'    协商缓存：由后端在响应头设置'Last-Modified': stats.mtimeMs   前端请求时请求头会带上这个时间节点：If-Modified-Since: 更新时间   执行顺序：优先执行强缓存，强缓存失效才执行协商缓存 |
| 7 | ⭐⭐ | [token应该存到localStorage还是cookie](about:blank) | 看场景使用：   localStorage更具灵活性，开发这可以手动管理 laocalStorage，这种灵活性对于一些高级用例和性能优化场景可能非常有用。缺点是不安全。<br/>cookie 的token传输更加安全，防止了XSS(跨站脚本)和CSRF(跨站请求伪造) 攻击的风险。    |


## 二、面试资源、网站
| 序号 | 网址 | 内容 |
| --- | --- | --- |
| 1 | [https://www.mianshipai.com/docs/services/1v1.html](https://www.mianshipai.com/docs/services/1v1.html) | 双越老师主导的面试网站，主要是提供(1V1）面试指导服务(需要付费) |
| 2 | [https://fe.ecool.fun/?ic=M9KOQQ](https://fe.ecool.fun/?ic=M9KOQQ) |  需要付费 |


