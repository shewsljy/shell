echo: echo [-neE] [arg ...]

    Write arguments to the standard output. 将数值写入标准输出
    
    Display the ARGs on the standard output followed by a newline. 在标准输出上显示数值，然后显示换行符
    
    Options:
      -n	do not append a newline 不换行
      -e	enable interpretation of the following backslash escapes 启用以下反斜杠转义解释
      -E	explicitly suppress interpretation of backslash escapes 不启用反斜杠转义解释，默认
    
    'echo' interprets the following backslash-escaped characters: 以下反斜杠转义字符的解释
      \a	alert (bell) 警报声
      \b	backspace 删除前一个字符
      \c	suppress further output 不换行，并且这个参数后面的任何字符（包括参数）都会被忽略掉不打印
      \e	escape character 删除后一个字符
      \f	form feed 清除屏幕，效果跟\v相似
      \n	new line 换行
      \r	carriage return 回车
      \t	horizontal tab 水平制表符
      \v	vertical tab 垂直制表符
      \\	backslash 反斜杠
      \0nnn	the character whose ASCII code is NNN (octal).  NNN can be
    	0 to 3 octal digits 其ASCII码为NNN（八进制）的字符，NNN可以是0到3个八进制数字
      \xHH	the eight-bit character whose value is HH (hexadecimal).  HH
    	can be one or two hex digits 值为HH（十六进制）的八位字符， HH可以是一个或两个十六进制数字
    
    Exit Status:
    Returns success unless a write error occurs. 返回成功，除非发生写错误