---
layout: post
title: "Charechar包装类获取ASCII码（大小写）"
date:  2019-05-26 14:06:05
categories: java  Charechar ASCII码
tags: java Charecher ASCII码
excerpt: iava学习Charechar相关
---

## Charechar包装类获取ASCII码（大小写）

### 输出ASCII码小写字母

代码：

```html
	for(char c = 0;c < 128 ;c++){
			if(Character.isLowerCase(c)){
				System.out.println("value:"+(int)c+" Character:"+c);
			}/*else{
				System.out.println("value:"+(int)c+" Character:"+c);
			}*/
		}
```

输出：

```
value:97 Character:a
value:98 Character:b
value:99 Character:c
value:100 Character:d
value:101 Character:e
value:102 Character:f
value:103 Character:g
value:104 Character:h
value:105 Character:i
value:106 Character:j
value:107 Character:k
value:108 Character:l
value:109 Character:m
value:110 Character:n
value:111 Character:o
value:112 Character:p
value:113 Character:q
value:114 Character:r
value:115 Character:s
value:116 Character:t
value:117 Character:u
value:118 Character:v
value:119 Character:w
value:120 Character:x
value:121 Character:y
value:122 Character:z
```

### 输出ASCII码大写字母

代码：

```html
value:65 Character:A
value:66 Character:B
value:67 Character:C
value:68 Character:D
value:69 Character:E
value:70 Character:F
value:71 Character:G
value:72 Character:H
value:73 Character:I
value:74 Character:J
value:75 Character:K
value:76 Character:L
value:77 Character:M
value:78 Character:N
value:79 Character:O
value:80 Character:P
value:81 Character:Q
value:82 Character:R
value:83 Character:S
value:84 Character:T
value:85 Character:U
value:86 Character:V
value:87 Character:W
value:88 Character:X
value:89 Character:Y
value:90 Character:Z
```

### 键盘出入String字符串，转换为对应字符的ADCII码值

代码：

```html
//lowerCaseDemo();
	 	//UpperCaseDemo();
		Scanner sc = new Scanner(System.in);
		System.out.println("输入String:");
		String s = sc.nextLine();
		for(int i = 0; i < s.length(); i++){
			System.out.println("String中第"+(i+1)+
					"个字符对应的ASCII码value值为："+(int)s.charAt(i));
		}
		sc.close();
```

输出：

```html
输入String:
123asd #$[]\=-
String中第1个字符对应的ASCII码value值为：49
String中第2个字符对应的ASCII码value值为：50
String中第3个字符对应的ASCII码value值为：51
String中第4个字符对应的ASCII码value值为：97
String中第5个字符对应的ASCII码value值为：115
String中第6个字符对应的ASCII码value值为：100
String中第7个字符对应的ASCII码value值为：32
String中第8个字符对应的ASCII码value值为：35
String中第9个字符对应的ASCII码value值为：36
String中第10个字符对应的ASCII码value值为：91
String中第11个字符对应的ASCII码value值为：93
String中第12个字符对应的ASCII码value值为：92
String中第13个字符对应的ASCII码value值为：61
String中第14个字符对应的ASCII码value值为：45
```

主要利用String的charAt()方法。