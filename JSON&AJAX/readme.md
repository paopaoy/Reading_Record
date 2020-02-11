# AJAX  
## 概念：
* Asynchronous Javascript And XML --- `异步的` Javascript 和 XML
* 交互式网页开发技术(无需加载整个网页情况下，部分更新网页)

  - 异步和同步：客户端和服务器端相互通信的基础上  
     * 同步：客户端必须等待服务器端的响应。在等待的期间客户端不能做其他操作。
     * 异步：客户端不需要等待服务器端的响应，在服务器处理请求的过程中，客户端可以进行其他的操作。  
     * 举例：洗衣机洗衣服的时候可以选择等待洗衣机洗完，期间什么都不做(同步)，可以选择在洗衣期间做别的家务，等到洗衣机洗完响了之后立马拿出衣服(异步)

  - 核心是提升用户的体验
     
## 实现方式：
  - 原生的JS实现方式(XmlHttpRequest)  
    
  - JQuery实现方式：
    1. $.ajax()
       * 语法：$.ajax({键值对});  
         // 使用$.ajax()发送异步请求
         $.ajax({
           url: "", // 请求路径
           type: "", // 请求方式
           data: "", // 请求参数
           success: () => {}, // 响应成功回调
           error: () => {}, // 请求响应错误回调
           dataType: "" // 接收到的响应数据格式
         })
    2. $.get()：发送 get 请求
       * 语法：$.get(url, [data], [callback], [type])  
    3. $.post()：发送 post 请求
       * 语法：$.post(url, [data], [callback], [type]) 


# JSON
## 概念
* JavaScript Object Notation --- JavaScript对象表示法
* JSON 现在多用于存储数据和交换文本信息的语法
* 进行数据的传输
* JSON 比 XML 更小、更快、更易解析

## 语法
   1. 基本规则  
      * 数据是名称/值对
      * 数据由逗号分隔  
      * 花括号保存对象  
      * 方括号保存数组  