# IP_INFO
获取IP相关信息。如：IP所属地区，所属运用商

数据来源：

1、apnic 全球IP地址段分配获取： http://ftp.apnic.net/apnic/stats/apnic/delegated-apnic-latest
![image](https://user-images.githubusercontent.com/97394404/156863920-1425ae1b-a7e0-4e1c-bb1b-15c2ba9f6f57.png)
2、bczs IP地址段分配，同时有的还带运营商：http://ip.bczs.net/countrylist
![image](https://user-images.githubusercontent.com/97394404/156864007-596a204b-0cb5-4919-b672-4d8a37406ee7.png)

使用sqlite进行数据存储，后续如需添加数据，则自行在db中添加

使用方式：

1、在命令行运行 ./CHECK_IPV4_ADRESS_mac_arm  
开启一个web服务端口为10001，同时会进行数据的加载
![image](https://user-images.githubusercontent.com/97394404/156863634-ca23679a-4022-40a7-a56b-46b86297f3c5.png)

2、在浏览器使用  http://ip:10001/{ip|ip number}

使用url带ip访问。http://127.0.0.1:10001/1.0.1.0
![image](https://user-images.githubusercontent.com/97394404/156864110-056c9db6-fdc5-4d5c-96aa-33f7bc738d1d.png)

使用url带ip转数字访问 http://127.0.0.1:10001/345678912
![image](https://user-images.githubusercontent.com/97394404/156864166-2599faa0-b6a2-44ab-9023-cd1fa7e8ea35.png)

python调用方式：
![image](https://user-images.githubusercontent.com/97394404/156864400-75c7824b-0ef3-4c4f-a320-38cc1644354f.png)

批量获取IP信息，可使用python的方式，烂机器并发也可1000以上

后台：
![image](https://user-images.githubusercontent.com/97394404/156864221-4524bde6-2340-46a7-aa3f-9d5ecef70432.png)
