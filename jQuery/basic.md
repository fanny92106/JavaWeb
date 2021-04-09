# jQuery


1. Definition:
        
        - jQuery = JavaScript + Query, 即辅助JavaScript开发的js类库
        - 核心: write less, do more
        - $()是jQuery的核心函数
        - jQuery对象的本质是DOM对象数组 + jQuery提供的一系列功能函数
        - jQuery对象不能使用DOM对象的属性和方法; DOM对象也不能使用jQuery对象的属性和方法
        - DOM对象与jQuery对象之间相互转换
![conversionBetweenDOMandjQueryObjs](imagePool/conversionBetweenDOMandjQueryObjs.png)
               
               
2. $( ) 核心函数

        - $(function() {..}) 代表页面加载完之后自动调用
        - $(DOM_ele) 返回一个jQury对象
        - jQuery选择器选择页面元素
              a. 基本选择器: 
                - $("tag_name")
                - $("#element_id")
                - $(".class")
                - $("*") 选择所有元素
                - $(selector_01, selector_02) 组合选择器, 合并多个选择器选择的结果一并返回, 返回的DOM元素集是按其在页面的顺序排序
                
        - $("HTML tag").appendTo("body") 代表向html页面添加HTML元素
        

