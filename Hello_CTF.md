Hello CTF

strcat()函数

字符串连接

char *strcat(char *strDestinayion,const char* strSource)

把source所指字符串追加到destination的结尾，覆盖\0,复制\0'.

memset()函数

extern void *memset(void *s,int a,size_t count)

s:数组

void：初始化的首地址

a:数据

count：长度

sprintf()函数

int sprintf(char *buffer,const char *format,[argument]...)

把格式化的数据写入某个字符串中

sprintf是一个变参函数，对于写入的buffer字符数没有限制，存在buffer溢出的可能

buffer：目的字符串

format：格式

[argument]：内容（写入buffer）



加密逻辑：

![1585226760214](C:\Users\SUNMINGYANG\AppData\Roaming\Typora\typora-user-images\1585226760214.png)

输入字符串v9，用v4、v3对v9进行遍历，经asc_408044变换后得到v13，则v9为正确的flag。



