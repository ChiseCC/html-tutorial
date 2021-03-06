# URL

URL 是“统一资源定位符”（Uniform Resource Locator）的首字母缩写，中文译为“网址”，表示各种资源在互联网上的地址。这些资源通常是文件，比如网页文件、图像文件、媒体文件、脚本文件等等。只要知道了它们的网址，才可能在互联网上获取它们。

## 组成

URL 由多个部分组成。

（1）协议（scheme）：互联网支持多种协议，必须指明网址使用哪一种协议，默认是 HTTP 协议。现在，HTTP 的加密版 HTTPS 协议越来越常见了。浏览器根据协议，处理网址所指向的资源。

协议后面紧跟着一个冒号和两个斜杠。但是，`mailto`协议是一个例外，它后面只有一个冒号，比如`mailto:foo@example.com`。

（2）主机（host）：资源所在的网站或服务器。

（3）路径（path）：资源在网站上的访问路径。比如，`/foo/bar.html`这个路径指的是`bar.html`在子目录`foo`里面。

有时，路径指的是一个目录，这时路径就不会包含文件名，结尾可能有斜杠，也可能没有斜杠。比如`/foo`和`/foo/`都可以是目录。如果路径是一个目录，服务器通常会默认跳转到该目录里面的`index.html`文件，但也可能列出目录里面的内容，这取决于服务器的设置。

URL只能使用ASCII字符之中的可打印字符。为了表示那些不在这个范围的字符，允许将字符转义，即在该字符十六进制的ASCII码之前加上一个百分号。举例来说，字符`a`的十六进制ASCII是`61`，因此`www.apple.com`又可以写成`www.%61pple.com`。

有些字符在URL中具有特殊含义，就不能用在路径名之中。

- `%` 转义字符
- `/` 路径分隔符
- `.` 路径组件
- `..` 路径组件
- `#` 锚点标识符
- `?` 表示参数字符串
- `&` 参数分隔符
- `:` 表示传输协议的分隔符

