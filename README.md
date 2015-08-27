# JSP

Web pages can be either static or dynamic. 

JavaServer Pages (JSP) is a technology that helps software developers create dynamically generated web pages based on HTML, XML, or other document types. 

Servlet is html in java
JSP is java in html


Difference between danamical web techonologes:

    1.JSP: Java, platform Independence, more secure, suitable for large size and enterprise web application;

    2.Asp.net: less security, less platform Independence.

    3.PHP:  easy, efficiency, low cost, short development cycle, suitable for middle and small size enterprise web application.

Direcotry of Web-INFO:

    1. web.xml.

    2. classees folder, store *.class file.

    3. lib folder, store jar files.

 Comment in JSP:
 
     1.HTML comment: <!-- Write your comments here --> This can be seen in the broswer.
 
     2.JSP comment: <%-- Comment --%> This cannot be seen in the broswer.
 
     3. // dingle line comment
     /*   */ multiply line comment
 
page指令语法格式：

<%@ page 属性="属性值"%>

属性1. language JSP脚本语言 default to be JAVA

属性2. import 默认为无 

属性3. contentType 默认text/html ISO-8859-1 文本文件/网页 默认字符集是一个纯英文的字符集

JSP Life Cycle: 

    1. Page Translation: In this phase the JSP page is translated into the corresponding Servlet. 

    2. Page Compilation: compile that Servlet.

    3. Load Class and Create Instance

    4. JSP initialization (Call jspinit() )

    5. JSP execution (Call _jspServcie())

    6. JSP clean up (Call jspDestroy() )


Implicit Object:

Implicit Objects and their corresponding classes:

1.out: This is used for writing content to the client (browser). It has several methods which can be used for properly formatting output message to the browser and for dealing with the buffer.

    void print()

    void println()

    void newLine()

    void clear()

    void clearBuffer()

    void flush()

    boolean isAutoFlush()

    int getBufferSize()

    int getRemaining()

2.request: The main purpose of request implicit object is to get the data on a JSP page which has been entered by user on the previous JSP page. While dealing with login and signup forms in JSP we often prompts user to fill in those details, this object is then used to get those entered details on an another JSP page (action page) for validation and other purposes.



3.response: It is basically used for modfying or delaing with the response which is being sent to the client(browser) after processing the request.

4.session: Session is most frequently used implicit object in JSP. The main usage of it to gain access to all the user’s data till the user session is active.

5.application	

6.exception

7.page

8.pageContext	

9.config


get vs post:

    •	The Get method transfer data through url, while Post method put data into a packet before transferring.

    •	Get method has better performance than Post

    •	Post method is more secure than Get

    •	For Get method, it has an upper limit of how much data it can transfer, while Post method does not have this limit. 
    
Difference between forward and redirect:

    •	If page1 forward to page2, then url is page1 and the content is page2
    
    •	If page1 redirect to page2, then both url and the content is page2
    
    •	To make forward, we can use <jsp:forward page=”somePage”/>
    
    •	To make redirect, we need to write a scriptlet
        <% response.sendRedirect(“somePage”); %>
        
JSP tag:

    •	JSP expression: <%=      %>
    
    You can output the value of k calculated in scriptlet
    
    •	JSP declaration: <%!      %>
    
    You can declare a Java variable and method like “add” inside it
    
    •	JSP scriptlet: <%       %>
    
    You can write java code, call method inside. But you can’t define a method inside 
    
    •	JSP direct: <%@       %>
    
    You can include another file. This can be used inside <body> 
    
    (1)	Page direct: <%@page import=”...” %>
    
    (2)	Include direct: <%@include file=”... %>
    
    (3)	Taglib direct: <%@taglib uri=”...” prefix=”...”%>
    
    
What are advantages of using JSP? 
    JSP offer several advantages as listed below:   
        1)   Performance  is  significantly  better  because  JSP allows  embedding  Dynamic  Elements  in  HTML                     Pages itself.   
        2)   JSP  are  always  compiled  before  it's  processed  by the  server  unlike  CGI/Perl  which  requires                 the server to load an interpreter and the target script each time the page is requested.   
        3)   JavaServer Pages are built on top of the Java Servlets API, so like Servlets, JSP also has access to all                 the powerful Enterprise Java APIs, including JD
        BC, JNDI, EJB, JAXP etc. 
        4)   JSP  pages  can  be  used  in  combination  with  servlets  that  handle  the  business  logic,  the                    model supported by Java servlet template engines. 








