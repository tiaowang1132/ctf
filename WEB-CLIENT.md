# WEB-CLIENT

## 1.HTML - disabled buttons
进入题目，打开审查元素，输入框和button都被disable了，删去即可，然后在输入框中随便输入字符，点击button即可得flag。

## 2.Javascript - Authentication
进入题目，发现一个登陆框，查看源代码，发现login.js，查看该文件，<br>
2.1
使用这个password即可。

## 3.Javascript - Source
该题目直接查看源代码即可。

## 4.Javascript - Authentication 2
查看源代码中的login.js，分析代码得知密码为HIDDEN。<br>
2.2

## 5.Javascript - Obfuscation 1
2.3
查看源代码得知，pass为url编码的字符串，使用urldecode即可得flag。

## 6.Javascript - Obfuscation 2
2.4
先使用url解码两次，得到unescape("unescape("String.fromCharCode(104,68,117,102,106,100,107,105,49,53,54)")")
然后再使用fromcharcode解码，即ASCII码。

待续