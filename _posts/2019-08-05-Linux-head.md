---
title: 每日一Linux命令 - head
mathjax: true
key: 20190805head
tags:
- Linux
---
### 所有参数
1. -c, --bytes=[-]K
2. -n, --lines=[-]K
3. -q, --quiet, --silent 不显示包含给定文件名的文件头
4. -v, --verbose 总是显示包含给定文件名的文件头

5. K 后面可以跟乘号:
    - b 512, kB 1000, K 1024, MB 1000*1000, M 1024*1024,
    - GB 1000*1000*1000, G 1024*1024*1024, 对于T, P, E, Z, Y 同样适用。

### 常用参数
#### -cX
从头开始读取X个字节
```
head -c300 20190805.log
```

#### -n / -nX
从有开始读取X(缺省时=10)行
```
head -n 20190805.log
head -n100 20190805.log
```

#### -q
不显示文件名的文件头
```
head -q 20190805.log
```

#### -v
显示文件名的文件头
```
head -v 20190805.log
```