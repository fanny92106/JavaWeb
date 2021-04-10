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
                
              b. 高级选择器: 查文档
                
        - $("HTML tag").appendTo("body") 代表向html页面添加HTML元素
        

3. jQuery主要函数

    1. 操作标签内容/文本/value
    
            - html(): 获取或设置start标签和end标签内的内容(包括标签或文本)
    ![jQueryHtml()](imagePool/jQueryHtml().png)
            
            - text(): 获取或设置start标签和end标签内的文本
    ![jQueryText()](imagePool/jQueryText().png)
            
            - val(): 获取或设置表单项的value属性值
    ![jQueryVal()](imagePool/jQueryVal().png)
    
    
    
    2. 操作标签属性

            - attr(): 获取或设置属性值, 但不推荐使用在checked, readOnly, selected, disabled等, 因为如果不设置会返回undefined
    ![jQueryAttr()](imagePool/jQueryAttr().png)
                
            attr()还可以添加自定义标签属性
    ![jQueryAttrCustom](imagePool/jQueryAttrCustom.png)
            
           - prop(): 获取或设置属性值, 推荐使用, 尤其在需要checked, readOnly, selected, disabled时推荐使用, 但不能设置自定义标签属性
    ![jQueryProp()](imagePool/jQueryProp().png)
