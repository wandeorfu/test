**First, download the source code and set up the environment**

source code:

[miansen/Roothub at vhttps://github.com/miansen/Roothub/tree/v2.52.5](https://github.com/miansen/Roothub/tree/v2.5)

<img src="png/sql1.png">

**There is SQL injection in the search bar on the home page**

<img src="png/sql2.png">

**Use sqlmap for injection**

sqlmap.py -u "http://192.168.125.15:8080/search?s=1" --dbs --batch

<img src="png/sql3.png">

**In the source code, there is no filtering here, and ${} is used**

src/main/java/cn/roothub/web/front/IndexController.java

<img src="png/sql4.png">