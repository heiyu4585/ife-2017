# [动态数据绑定（四）](http://ife.baidu.com/course/detail/id/22)

[梁少峰](http://ife.baidu.com/mentor/detail/id/26) | [斌斌学院](http://ife.baidu.com/college/detail/id/10)

时间  平均用时0.7天

### 课程概述

作业提交截止时间：04-24

## 重要说明

百度前端技术学院的课程任务是由百度前端工程师专为对前端不同掌握程度的同学设计。我们尽力保证课程内容的质量以及学习难度的合理性，但即使如此，真正决定课程效果的，还是你的每一次思考和实践。<br />
课程多数题目的解决方案都不是唯一的，这和我们在实际工作中的情况也是一致的。因此，我们的要求不仅仅是实现设计稿的效果，更是要多去思考不同的解决方案，评估不同方案的优劣，然后使用在该场景下最优雅的方式去实现。那些最终没有被我们采纳的方案，同样也可以帮助我们学到很多知识。所以，我们列出的参考资料未必是实现需求所必须的。有的时候，实现题目的要求很简单，甚至参考资料里就有，但是背后的思考和亲手去实践却是任务最关键的一部分。在学习这些资料时，要多思考，多提问，多质疑。相信通过和小伙伴们的交流，能让你的学习事半功倍。

## 任务目的

1. 熟练使用原生 JS对操作 DOM 结构

## 任务描述

这是“动态数据绑定”的第四题。有了前面的充分准备，相信你能搞定这一题。请实现如下的这样一个 Vue，传入参数是一个 Selector 和一个数据对象，程序需要将 HTML 模板片段渲染成正确的模样。 这就是一次性的静态数据绑定。<br />

1. 如果传入参数对象是一个“比较深”的对象（也就是其属性值也可能是对象），那该怎么办呢？举个例子。

```javascript
let app = new Vue({
  el: '#app',
  data: {
    user: {
      name: 'youngwind',
      age: 25
    }
  }
});
```

```html
<!-- 页面中原本的 html 模板片段 -->
<div id="app">
    <p>姓名：{{user.name}}</p>
    <p>年龄：{{user.age}}</p>
</div>
```

```html
<!-- 最终在页面中渲染出来的结果 -->
<div id="app">
    <p>姓名：youngwind</p>
    <p>年龄：25</p>
</div>
```

PS：此题尚未要求实现动态数据绑定<br />

## 任务注意事项

1. 不能使用任何第三方的库
2. 程序执行环境为浏览器