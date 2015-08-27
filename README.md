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

1. out: This is used for writing content to the client (browser). It has several methods which can be used for properly formatting output message to the browser and for dealing with the buffer.

    void print()

    void println()

    void newLine()

    void clear()

    void clearBuffer()

    void flush()

    boolean isAutoFlush()

    int getBufferSize()

    int getRemaining()

2. request: The main purpose of request implicit object is to get the data on a JSP page which has been entered by user on the previous JSP page. While dealing with login and signup forms in JSP we often prompts user to fill in those details, this object is then used to get those entered details on an another JSP page (action page) for validation and other purposes.



3.response: It is basically used for modfying or delaing with the response which is being sent to the client(browser) after processing the request.

4. session: Session is most frequently used implicit object in JSP. The main usage of it to gain access to all the user’s data till the user session is active.

5. application	

6. exception

7. page

8. pageContext	

  9 .config


get vs post:

•	The Get method transfer data through url, while Post method put data into a packet before transferring.

•	Get method has better performance than Post

•	Post method is more secure than Get

•	For Get method, it has an upper limit of how much data it can transfer, while Post method does not have this limit. 



