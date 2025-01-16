# Spring MVC Web Page 🌐  

This is a simple **Spring MVC** web application that serves as a basic webpage with multiple sections, including **Home, Hello Page, About Us, and Contact Us**. The project is built using **Spring MVC, JSP, and Apache Tomcat** for deployment.  

---

## 📌 Spring MVC Flow Diagram  

![Spring MVC Flow](image.png)  

### **Spring MVC Workflow**  

1️⃣ **Client (User)** sends a request.  
2️⃣ **Front Controller (DispatcherServlet)** receives and forwards the request.  
3️⃣ **Handler Mapping** determines the controller handling the request.  
4️⃣ **Controller** processes the request and returns a Model & View object.  
5️⃣ **View Resolver** maps the logical view name to the actual JSP file.  
6️⃣ **View (JSP Page)** renders the UI.  
7️⃣ **Response** is sent back to the client.  

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

