## session cookie 跨域问题
默认情况下，跨源请求不提供凭据(cookie、HTTP认证及客户端SSL证明等)。通过将withCredentials属性设置为true，可以指定某个请求应该发送凭据。
如果服务器接收带凭据的请求，会用下面的HTTP头部来响应。
```
Access-Control-Allow-Credentials: true
```
如果发送的是带凭据的请求，但服务器的相应中没有包含这个头部，那么浏览器就不会把相应交给JavaScript(于是，responseText中将是空字符串，status的值为0，而且会调用onerror()事件处理程序)。
另外，服务器还可以在Preflight响应中发送这个HTTP头部，表示允许源发送带凭据的请求。
支持withCredentials属性的浏览器有Firefox 3.5+、Safari 4+和Chrome。IE10及更早版本都不支持