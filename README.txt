这是一个使用GET 方法检测XSS漏洞的

利用 URL 中的参数，然后插入payload

检测原理：看返回的respond中是否有完整的payload，
如果不被转义，则代表存在XSS漏洞

后续：将完善方法，加上POST方法，异或改成用正则表达式对网页进行解析，查找输入框，进行payload插入