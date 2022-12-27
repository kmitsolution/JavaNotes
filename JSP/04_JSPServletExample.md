# Jsp with Java Servlet

Let's create JSP page with some dynamic content using Servlet.
 <br />
 <b>Step 1: </b> Start Eclipse with a workspace (C:\Projects\JSP) <br />
 <b>Step 2: </b> Select File --> Dynamic Web Project and Provide project name (02_HelloWorldServlet) and keep rest of the options same. <br />
 <b>Step 3: </b> Add a New  --> Servlet. <br />
 <b>Step 4: </b> Give a java package name (com.kmit) and a class name (HelloServlet) <br />
 <b>Step 5: </b> Add doGet method (for this example) <br />
 <b>Step 6: </b> Add below code
 ```java
 	protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		// TODO Auto-generated method stub
		//System.out.println("Hello Servelet ");
		PrintWriter print = response.getWriter();
		print.println("<h1>Hello Servlet</h1>");
	}
  
 ```
 
 <b>Step 7: </b> Run the Application
 
 You will get Hello Servlet
