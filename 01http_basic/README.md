什么是 HTTP Basic Authentication？见Basic_access_authentication ,在真实场景中的表现是：当用访问需要登录验证的页面时，浏览器会自动弹出一个对话框，要求输入用户名/密码，输入正确后可以正常访问。
在这种方式，浏览器会把用户名和密码通过BASE64编码在HTTP HEAD 里面
Authorization: Basic QWxhZGRpbjpPcGVuU2VzYW1l

服务器端解析之后做身份验证，并给客户端返回
WWW-Authenticate: Basic realm="User Visible Realm"

作者：ntop
链接：https://www.jianshu.com/p/eaf9197abb6b
來源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。