# Spring MVC Web Page 🌐  

This is a simple **Spring MVC** web application that serves as a basic webpage with multiple sections, including **Home, Hello Page, About Us, and Contact Us**. The project is built using **Spring MVC, JSP, and Apache Tomcat** for deployment.  

---

## 📁 Project Structure  

```sh
SpringWebMvc1SP
│── src/
│   ├── main/
│   │   ├── java/in/sp/main/
│   │   │   ├── MyController.java
│   │   ├── resources/
│   │   ├── webapp/
│   │   │   ├── WEB-INF/views/
│   │   │   │   ├── aboutUs.jsp
│   │   │   │   ├── contactUs.jsp
│   │   │   │   ├── hello.jsp
│   │   │   ├── index.jsp
│   │   │   ├── myds-servlet.xml
│   │   │   ├── web.xml
│── pom.xml
│── target/
```

---

## ⚙️ **Technologies Used**  

- **Spring MVC** (Model-View-Controller framework)  
- **JSP (JavaServer Pages)** for views  
- **Apache Tomcat 10.1** as the server  
- **Maven** for dependency management  
- **Java 11** (JDK 11)  

---

## 🏗 **Project Features**  
✅ Simple MVC structure  
✅ Organized JSP pages in `WEB-INF/views/`  
✅ Dispatcher Servlet configuration in `myds-servlet.xml`  
✅ Navigation between multiple pages  
✅ Works with Apache Tomcat  

---

## 🔧 **Configuration (web.xml & myds-servlet.xml)**  

### `web.xml`
```xml
<servlet>
    <servlet-name>dispatcher</servlet-name>
    <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
    <load-on-startup>1</load-on-startup>
</servlet>
<servlet-mapping>
    <servlet-name>dispatcher</servlet-name>
    <url-pattern>/</url-pattern>
</servlet-mapping>
```

### `myds-servlet.xml`
```xml
<bean class="org.springframework.web.servlet.view.InternalResourceViewResolver">
    <property name="prefix" value="/WEB-INF/views/" />
    <property name="suffix" value=".jsp" />
</bean>
```

### 🎯 *Happy Coding! 🚀*

