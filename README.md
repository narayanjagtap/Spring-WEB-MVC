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

## 🚀 **How to Run the Project**  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/your-username/SpringWebMvc1SP.git
cd SpringWebMvc1SP
```

### 2️⃣ Configure Dependencies  
Ensure **Maven** is installed, then run:  
```sh
mvn clean install
```

### 3️⃣ Deploy on Apache Tomcat  
- Place the project in the **Tomcat webapps folder** or use an **IDE (Eclipse/IntelliJ)** to deploy.  
- Start the Tomcat server.  

### 4️⃣ Access the Web Pages  
Open the browser and go to:  
```
http://localhost:8080/SpringWebMvc1SP/
```
Available Pages:  
- **Home Page:** `/`  
- **Hello Page:** `/helloPage`  
- **About Us:** `/about-Us`  
- **Contact Us:** `/contact-Us`  

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

---

## 📜 **License**  
This project is open-source and available under the **MIT License**.  

---

## 🤝 **Contributing**  
Contributions, issues, and feature requests are welcome! Feel free to submit a **pull request** or report an issue.  

---

## 📬 **Contact**  
For any queries, reach out via:  
📧 Email: your-email@example.com  
🔗 LinkedIn: [Your Profile](https://linkedin.com/in/your-profile)  
💻 GitHub: [Your GitHub](https://github.com/your-username)  

---

### 🎯 *Happy Coding! 🚀*
```

---

### **What’s Included?**  
✅ **Project Overview**  
✅ **Folder Structure**  
✅ **Setup & Running Instructions**  
✅ **Technology Stack**  
✅ **Feature List**  
✅ **Configuration (web.xml & servlet.xml)**  
✅ **License & Contribution Info**  
✅ **Contact Links**  

Let me know if you want **any modifications or additions**! 🚀😊
