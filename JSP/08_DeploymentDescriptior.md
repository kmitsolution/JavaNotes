# Deployment Descriptor

1. File that contains configuration of your java application.
2. It is <b>web.xml</b> resides under WEB-INF folder
3. During the web application deplyment, Webserver refers to this file.
4. It contains the information like servelet declaration, servlet-mapping, initialization parameter etc. which is in <webapp> </webapp>
```xml
<webapp>
  servlet declartion
  servlet mapping
  Initialization parameter
  welcome-file-list ( which contains the file start up file name)
  etc..
```
### Demo
1. Create a Dynamic Web project. 
2. Add a servlet (Add-> servlet) and select <b>Deployment Descriptor</b> check box.
3. web.xml file will be added in WEB-INF folder.
4. In the servlet class there is one annotation is added like @WebServlet("/ServeletDesc") which is part of the URL of the application.
5. Add an index.jsp file(which is part of welcome-file-list in web.xml)
6. Run the application ( the URL will have annotation (@WebServlet("/ServeletDesc")) in the end(and it will open the doGet() of the servlet). if you remove annotation in the url then it will open index.jsp page.
 
Sample of web.xml  
```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://xmlns.jcp.org/xml/ns/javaee" xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd" id="WebApp_ID" version="4.0">
  <display-name>03_Descriptor</display-name>
  <welcome-file-list>
    <welcome-file>index.html</welcome-file>
    <welcome-file>index.jsp</welcome-file>
    <welcome-file>index.htm</welcome-file>
    <welcome-file>default.html</welcome-file>
    <welcome-file>default.jsp</welcome-file>
    <welcome-file>default.htm</welcome-file>
  </welcome-file-list>
</web-app>
```
