**First, let's set up the environment and download the branch of version 2.6**

<img src="img/xss0.png">

**After building, log in to the background and follow the location in the picture**

<img src="img/xss1.png">

**After saving, the XSS vulnerability will be triggered and a window will pop up**

<img src="img/xss2.png">

<img src="img/xss3.png">

**In the backend code, there is no filtering here**

src/main/java/cn/roothub/web/admin/SystemConfigAdminController.java

<img src="img/xss4.png">

