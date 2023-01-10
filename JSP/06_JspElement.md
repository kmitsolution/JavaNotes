# Jsp Elements
<img src =https://github.com/kmitsolution/JavaNotes/blob/main/JSP/images/Expressions.jpg />

## Example

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
<%! public int i=10; %>
2+5= <%= 2+5 %> <br />
i= <%= i %> <br />
String Declaration= <%= new String("Jsp String") %> <br />
String Print= <%= "Jsp String" %> <br />
Java util function = <%= new java.util.Date() %> <br />
<b>Conditional Statement with Scriptlet</b>
<% if(i>=10){ 
     out.println("True"); }
   else{
     out.print("False");}  	 
%>
<br />
You cannot declare visibility in side the scriptlet <br />
Variable in scriptlet can be accessed with in other scriptlets as well. <br />
<% int i=10; %>
<% out.print("Value of i= " + i); %>

<br />
Declare a method=
<%!
 String method(){
	return "method is returning a string value";
}

 %>
 <%= method() %>
</body>
</html>
```
