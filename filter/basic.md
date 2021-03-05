# Filter (resource Filter)


### Definition:
    - Java Web 三大组件之一: listener, filter, servlet
    - 用途: 资源拦截器，过滤响应 (rare)


### 拦截请求
    - 权限检查
    - 日志操作
    - 事务管理
    ...
    

### 多个过滤器的工作原理 & 执行顺序

![filter](imagePool/filter.png)

    - doFilter() 方法做的两件事: 1.执行下一个filter, 2. 执行目标资源的获取
    - 执行顺序是根据在 web.xml 中 filter 的配置决定的
    - 多个filter 共享同一个 request 且都执行在同一个线程中
    - filter的 <url-pattern> 可以拦截多个地址



### Filter 拦截资源路径的三种配置方式

    1) 精准匹配
    <url-pattern>/target.jsp</url-pattern>
    代表: http://ip:port/工程路径/target.jsp
    
    
    2) 目录匹配
    <url-pattern>/admin/*</url-pattern>
    代表: http://ip:port/工程路径/admin/*
    
    
    3) 后缀名匹配
    <url-pattern>*.html</url-pattern>
    代表: 请求地址必须以.html结尾才能被拦截到; 后缀名匹配不能加 ”/“
    
    
