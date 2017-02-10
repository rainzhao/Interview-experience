## Ctrip FE

###1. One part(written examination): 
1. 简述什么是闭包以及它的应用场景。
2. 简述promise以及使用场景。
3. 简述你学过的css处理器。（如sass，less）。
4. 简述js的面向对象，以及es6引入了class后对面向对象有哪些影响。
5. 实现快速排序，说说你知道的浏览器sort中用了哪些排序算法。

###2. Two part(Technical interview)

1. 根据你的笔试进行提问。

###3. Three part(复试)
1. ** 简单介绍一下自己。**
2. **jquery的`$('.test').on('click',function(){})`,自己实现一下on事件。我大概写了一个:**
```
    var jquery = function(){}
    jquery.prototype.on = function (type,func) {
        switch(type){
            case 'click':
            this.addEventListener('click',func)
            //这里有个坑，为什么不用this.click事件而是用addEventListener,因为addEventListener可以多次绑定
            
        }
    }
```
3. **页面中有个表单，如何界面刷新的时候不会清空表单中的值。**
    + 我回答的是sessionStorage。感觉不是很好，但是面试官点了点头。。。
4. **进行ajax请求的时候，如何判断你的请求和返回的结果进行匹配，有可能你请求了两次，但是第一次你的结果是错误的，第二次结果是对的，但是你拿到的是最近一次返回的，如果顺序颠倒了，怎么进行避免。**
    + 将返回的请求体拿到，进行比对。
5. **react框架是如何实现组件的。**
    + class test extends React.Component{}
6. **react-native了解的多吗？我们主要用的react-native。**
    + 私下跑过它的app，拿出手机给他看了看。。。
7. **说一下你对优化网站性能有哪些方法。**
    + 雪碧图，压缩css，js，将不必立刻加载的js放在body后加载。
8. **你搭建项目是手动搭建，还是用的什么。**
    + 用cli脚手架工具和Yeoman,因为刚开始学自己写的可能不是很全面，就用工具搭建的。
9. **如果不用任何框架包括jquery如何进行组件化的开发。**
    + 用prototype的原型链，抽象出公用的方法，如刚才的问题2。
10. **angular和react的异同点。**

###4. 技术总监面试
1. **简单介绍下自己**
2. **问的简历上的项目，挨个讲了一下。**
