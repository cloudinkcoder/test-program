## Web Book

### Run in Local

mdbook 默认只监听 localhost (即 WSL2 内部的 127.0.0.1), 而 WSL2 与 Windows 宿主机处于不同的网络栈, Windows 的浏览器无法直接访问这个内部地址

最直接的方法, 就是让 mdbook 监听所有网络接口 (0.0.0.0), 这样 WSL 就会把端口暴露给宿主机

`mdbook serve -n 0.0.0.0` in WSL2
