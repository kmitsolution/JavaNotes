# JSP Directive
The jsp directives are messages that tells the web container how to translate a JSP page into the corresponding servlet.

There are three types of directives:

1. page directive
2. include directive
3. taglib directive

### page directive.
page directive defines the attributes on JSP page level

```
 <%@page attribute=value %>
```

#### Attributes of JSP page directive
1. import
2. contentType
3. extends
4. info
5. buffer
6. language
7. isELIgnored
8. isThreadSafe
9. autoFlush
10. session
11. pageEncoding
12. errorPage
13. isErrorPage

##### import
import attribute is used to import the classes, interfaces,packages etc on jsp page level. It is same as import statement in java class file.

##### Example
```jsp
<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
    pageEncoding="ISO-8859-1"%>
<!-- Page Import Example -->    
<%@ page import="java.util.Random,java.util.ArrayList" %>    
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Insert title here</title>
</head>
<body>
 <%
   int rn = new Random().nextInt(20);
   out.println(rn);
 %>
</body>
</html>
```
