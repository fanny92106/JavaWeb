# json


0. 用途

        - 前后端进行数据交互的格式
        - 轻量级, 相较于xml
        
        
1. json的两个常用方法

        json的存在有两种形式:
            一种是: 对象的形式存在, 叫做json对象
            一种是: 字符串的形式存在, 叫做json字符串
        
        - JSON.stringify(): 把json对象转换成为json字符串
        - JSON.parse(): 把json字符串转换成为json对象

        note: 一般我们在操作json中的数据时, 需要json对象的格式
        一般我们在客户端和服务器之间进行数据交换的时候, 使用json字符串
