# HttpServlet


### 常用 API

    - getRequestURI(): 获取工程资源路径 
    
![uniformResourceIdentifier](imagePool/uri.png)    

    - getRequestURL(): 获取工程路资源全限定路径 (服务器中)
    
![uniformResourceLocator](imagePool/url.png)    

    - getRemoteHost: 获取客户端ip
    - getHeader(str): 获取 请求头 信息
    - getParameter(str): 获取参数
    - getParameterValues(str): 获取参数(含有多值, eg: checkbox)
    - getMethod(): 获取 http 方法， GET or POST
    - setCharacterEncoding("UTF-8")
    - setAttribute(key, value)
    - getAttribute(key)
    - getRequestDispatcher: 获取转发对象
    


### 请求转发

![requestForward](imagePool/requestForward.png)

    - Definition: 服务器收到请求后，从一次资源跳转到另一个资源的操作叫做请求转发
    - 浏览器地址栏没有变化，相当于只有一次请求，尽管访问了多个资源
    - 共享 request 域中的数据
    - 可以转发到 WEB-INF 目录下
    - 不能访问工程之外的资源
