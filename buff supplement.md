# Learning never stops,ithinkbeforeiam.
- ### Pwntools I/O语句

1.https://blog.csdn.net/weixin_45556441/article/details/113982718
```
interactive() : 在取得shell之后使用,直接进行交互，相当于回到shell的模式。
recv(numb=字节大小, timeout=default) : 接收指定字节数。
recvall() : 一直接收直到达到文件EOF。
recvline(keepends=True) : 接收一行，keepends为是否保留行尾的\n。
recvuntil(delims, drop=False) : 一直读到delims的pattern出现为止。
recvrepeat(timeout=default) : 持续接收直到EOF或timeout。
send(data) : 发送数据。
sendline(data) : 发送一行数据，相当于在数据末尾加\n。
sendlineafter("字符串",data)
在这一串字符串结束之后发送数据
sendline 多发送了一次回车
```
2.https://blog.csdn.net/whatday/article/details/128090860
```
接收数据
recv(n) - 接收任何数量的可用字节
recvline() - 接收数据，直到遇到换行
recvuntil(delim) - 接收数据，直到找到一个分隔符
recvregex(pattern) - 接收数据，直到满足一个与pattern重合的内容为止
recvrepeat(timeout) - 继续接收数据，直到发生超时
clean() - 丢弃所有缓冲的数据
发送数据
send(data) - 发送数据
sendline(line) - 发送数据加一个换行
接收数据
pack(int) /p(32/64)- 打包发送一个字（word）大小的整数
unpack() u(32/64)- 接收并解包一个字（word）大小的整数
```

