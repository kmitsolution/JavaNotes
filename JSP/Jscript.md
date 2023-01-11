# JspScript
You can run java code inside the JSP

### Example
```jsp
<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
    pageEncoding="ISO-8859-1"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Insert title here</title>
</head>
<body>
<h1>JSP Scripting </h1>
<h2>Run a Java Code</h2>
<%
 for( int i=0;i<5;i++)
 {
	 out.println("i=" + i + "<br/>");
	 
 }
%>
</body>
</html>
```
