## Ctrip FE

###One part(written examination): 
1. 简述什么是闭包以及它的应用场景。
2. 简述promise以及使用场景。
3. 简述你学过的css处理器。（如sass，less）。
4. 简述js的面向对象，以及es6引入了class后对面向对象有哪些影响。
5. 实现快速排序，说说你知道的浏览器sort中用了哪些排序算法。

###Two part(Technical interview)

1. 根据你的笔试进行提问。

###Three part(复试)
1. 简单介绍一下自己。
2. jquery的`$('.test').on('click',function(){})`,自己实现一下on事件。我大概写了一个:

        var jquery = function(){}
        jquery.prototype.on = function (type,func) {
            switch(type){
                case 'click':
                    this.addEventListener('click',func)
            }
        }
