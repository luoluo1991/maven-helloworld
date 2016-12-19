# maven-helloworld
The project is a maven project, in this project created a simple servlet to response a web request.
testmaven.zip presents the structure of entire project and includes source code.
testmaven.war can be deloped on tomcat.
myeclipse vesion:10.7
tomcat version:7.0.40
jdk version:1.7
---
how to build a test maven project?

1.open myeclipse and create a web project, in the creting page check the option "add maven support", before create project, I config apache-maven-3.1.0 in "window/Preferences/MyEclise/Maven4MyEclipse/installations/"

2.create a new package named "com.redhat" under "src/main/java"

3.create a servlet file named "Hello.java" under "src/main/java/com.redhat" and create a jsp file named "register.jsp" under "WEB-INF/pages",when "Hello.java" finished will forward page to register.jsp.

4.create a servlet file named "Register.java" under "src/main/java/com.redhat" and create a page named "success.jsp" under "WEB-INF/pages". "Register.java" can accept name and password from client browser. "success.jsp" is created to tell client that register is finished.

5.update web.xml to finish the servlet url pattern match the real class path.

---

how to run this project?

1.deploy the war under tomcat/webapps and start tomcat.

2.input "http://localhost:8080/testmaven/hello" in address bar and press enter key.

3.client will forword to a page including two input box and a button, user can input "name" and "password" and kick the button to submit a request, "name" could include chinese charcter.

4.when press enter key ,user will see a register success page.
