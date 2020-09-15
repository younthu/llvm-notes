第一章很简单，一个简单的字符扫描函数(gettok)，把输入内容分成未知字符和以下几类。

~~~
tok_eof, 

// commands
tok_def, tok_extern, 

// primary
tok_identifier, tok_number
~~~


扫描的时候用了全局变量 IdentifierStr用来记录tok_identifier

用NumVal记录tok_number. 该语言只支持浮点数操作。
