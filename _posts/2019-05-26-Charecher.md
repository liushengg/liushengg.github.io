```
layout: post
title:  "打印ASCII码大小写字母方法（包装类Charecher）"
date:   2019-05-26 17:46:05
categories: Java
tags: Java
excerpt:Java

```

[TOC]

### 打印小写字母

```java
public static void lowerCaseDemo(){
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

### 打印大写字母

```
public static void UpperCaseDemo(){
		for(char c = 0;c < 128 ;c++){
			if(Character.isUpperCase(c)){
				System.out.println("value:"+(int)c+" Character:"+c);
			}
			
		}
	}
```

输出：

```
略
```

### ###键盘输入String自动判断ASCII码对应的value值

利用String.charAt()来实现

```
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

```
输入String:
123#%as <>+
String中第1个字符对应的ASCII码value值为：49
String中第2个字符对应的ASCII码value值为：50
String中第3个字符对应的ASCII码value值为：51
String中第4个字符对应的ASCII码value值为：35
String中第5个字符对应的ASCII码value值为：37
String中第6个字符对应的ASCII码value值为：97
String中第7个字符对应的ASCII码value值为：115
String中第8个字符对应的ASCII码value值为：32
String中第9个字符对应的ASCII码value值为：60
String中第10个字符对应的ASCII码value值为：62
String中第11个字符对应的ASCII码value值为：43
```

