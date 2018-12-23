在shell里面打开java文件实在是太麻烦了    
正好学了点shell， 所以就做了个小玩意@.@   

{java-finger}   

使用说明：   
	必要！！！   
	mkdir /etc/jf  

jc 改变工作目录  
jf 创建多级包，寻找并打开包  



.  
├── java  
│   └── com  
│       └── oyyd  
│           ├── dao  
│           │   └── impl  
│           │       └── DaoImpl.java  
│           ├── domain  
│           │   └── User.java  
│           └── service  
│               ├── impl  
│               └── UserService.java  
└── ptyhon  


> jc ./java				# 改变finger的工作目录  
> jc -p					# 打印finger工作目录  
/root/temp/java  
> jf DaoImpl			#使用vim打开DaoImpl.java		#已知缺陷：查找到多个时，仅打开第一个  
> jf com.oyyd.utils		#在java目录下创建包  
> jf domain Address		#在com.oyy.domain 下创建 Address.java 并使用vim打开  #已知缺陷：查找到多个时，仅选中第一个  

v0.01  
by oyydd  
