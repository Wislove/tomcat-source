## Http协议

---

#### Http请求

 一个 HTTP 请求包括三个组成部分:

 1. 方法—统一资源标识符(URI)—协议/版本
 2. 请求的头部(header)
 3. 请求主体内容(body)

请求头部与主体内容之间有一个换行符 \n
```
POST /examples/default.jsp HTTP/1.1
Accept: text/plain; text/html
Accept-Language: en-gb
Connection: Keep-Alive
Host: localhost
User-Agent: Mozilla/4.0 (compatible; MSIE 4.01; Windows 98)
Content-Length: 33
Content-Type: application/x-www-form-urlencoded Accept-Encoding: gzip, deflate

lastName=Franks&firstName=Michael
```
---
#### Http响应

类似于 HTTP 请求，一个 HTTP 响应也包括三个组成部分:

1. 方法—统一资源标识符(URI)—协议/版本
2. 响应头部(header)
3. 响应主体内容(body)

响应的主体部分与头部也有一个换行符\n。请求成功以后，返回一段html代码
```
HTTP/1.1 200 OK
Server: Microsoft-IIS/4.0
Date: Mon, 5 Jan 2004 13:13:33 GMT
Content-Type: text/html
Last-Modified: Mon, 5 Jan 2004 13:13:12 GMT
Content-Length: 112

<html>
<head>
<title>HTTP Response Example</title>
</head>
<body>
Welcome to Brainy Software
</body>
</html>
```

