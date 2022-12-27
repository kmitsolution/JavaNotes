# Servlet life cycle
<img src=https://github.com/kmitsolution/JavaNotes/blob/main/JSP/images/ServletLifeCycle.jpg width=700 height=300 />

There are 3 states for Servlet life cycle in Web Container.
1. <b>New</b> :- In this state web container invokes Init() to create the servlet instance and it is called once in servlet life cycle.
```java
public void init(ServletConfig config) throws ServletException
```
2. <b>Ready</b> :- In ready state servlet executes the tasks(using service()) which are called during Program execution.
```java
public void service(ServletRequest request, ServletResponse response)   
  throws ServletException, IOException
```

3. <b>End</b> :- In end state, web container calls destroy() to end the lifecycle.
```java
public void destroy()  
```

