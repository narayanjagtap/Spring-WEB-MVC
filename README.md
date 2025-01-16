# Spring MVC Web Page 🌐  

This is a simple **Spring MVC** web application that serves as a basic webpage with multiple sections, including **Home, Hello Page, About Us, and Contact Us**. The project is built using **Spring MVC, JSP, and Apache Tomcat** for deployment.  

---

## **📌Spring MVC Web Page Architecture**
```sh
+------------+     +----------------------+     +------------------+     +-----------------+     +------------+     +----------+
|  Client    | --> |  Front Controller    | --> |  Handler Mapping | --> |   Controller    | --> | View       | --> | Response |
| (Browser)  |     | (DispatcherServlet)  |     | (Maps URL)       |     | (Processes Req.)|     | (JSP Page) |     | (Sent to |
|            |     |                      |     |                  |     | (Returns Model)|     | (Renders)  |     |  Client) |
+------------+     +----------------------+     +------------------+     +-----------------+     +------------+     +----------+
```

## 📌 Spring MVC  

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
│   │   │   ├── MyController.java  <-- (Handles requests)
│   │   ├── resources/
│   │   ├── webapp/
│   │   │   ├── WEB-INF/views/
│   │   │   │   ├── aboutUs.jsp     <-- (UI Pages)
│   │   │   │   ├── contactUs.jsp
│   │   │   │   ├── hello.jsp
│   │   │   ├── index.jsp           <-- (Home Page)
│   │   │   ├── myds-servlet.xml    <-- (Spring Config)
│   │   │   ├── web.xml             <-- (Servlet Config)
│── pom.xml                          <-- (Maven Dependencies)
│── target/                          <-- (Compiled Output)
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

## 📌 **Configuration & Flow**

1️⃣ Client (Browser/User) sends a request.
2️⃣ DispatcherServlet (Front Controller) handles the request.
3️⃣ Handler Mapping routes the request to the correct Controller.
4️⃣ Controller processes the request and returns a Model & View.
5️⃣ View Resolver maps the logical view to an actual JSP page.
6️⃣ JSP (View Layer) renders the response.
7️⃣ Response is sent back to the client.

---

### 🎯 *Happy Coding! 🚀*

