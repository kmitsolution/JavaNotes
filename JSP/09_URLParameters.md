# Parameters
1. These the query string which is the part of url. For example https://google.com?search=web, in this url <b>search</b> is name of parameter which has value <b>web</b>.
2. It is the part of request object therefore servlet can read using <b>request.getParameter("name of parameter")</b>
3. You can read the parameter using JSP Page also using scriptlet  <b> request.getParameter("name of parameter")</b>

```java
protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		// TODO Auto-generated method stub
		//response.getWriter().append("Served at: ").append(request.getContextPath());
		PrintWriter out = response.getWriter();
		out.println(request.getParameter("search"));
	}
```

### jsp code
```html
<%
out.println(request.getParameter("search"));
%>
```
