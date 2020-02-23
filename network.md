# network

## 1.FTP - authentication
进入题目，发现下载一个pcap文件，使用wireshark打开查看，即可发现flag。

## 2.TELNET - authentication
进入题目，发现下载一个pcap文件，使用wireshark打开查看，即可发现flag。

## 3.ETHERNET - frame
发现一串十六进制编码，解码为字符串

将basic后面的字符串再使用base64解码（一般后面有等号的编码可以考虑base64），即得答案。

## 4.Twitter authentication

4.1<br>
## 5.IP - Time To Live
考察TTL，使用wireshark打开文件，由数据包可知道，ttl小于13时，没有应答，而等于13时则有了回答，说明ttl=13。
注：ttl是每过一个路由就减1。

## 6.LDAP - null bind
ldap的题目，使用ldapsearch工具（kali里自带），带上题干给的条件。
注：需要了解ldapsearch的相关参数。