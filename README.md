# EventManagement_SpringProject

Here are the steps to run a Spring Boot application:
------------------------------------------------------------

Install JDK: Ensure Java JDK (11 or above) is installed.
Set up IDE: Use an IDE like Spring Tool Suite (STS) or IntelliJ.
Build Project: Use Maven/Gradle to build the project (mvn clean install or gradle build).
Run Application:
From IDE: Right-click the main class and select "Run as Spring Boot App."
From command line: Run mvn spring-boot:run or execute the JAR file with java -jar target/your-app.jar.
====================================================================

applications.properties(MySQL)
-----------------------------------
spring.application.name=EventManagement_SpringProject   //project Name
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=jdbc:mysql://localhost:3306/EventDataSpring    #Create EventDataSpring DB In MySQL
spring.datasource.username= username   #MySQl UserName
spring.datasource.password=  password   #Password
spring.jpa.show-sql=true
#print the query on u r console
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
spring.jpa.hibernate.ddl-auto=update
====================================================================

These are two Demo Queries that u have to add in MySQL in events_entity table:
----------------------------------------------------------------------------------------------  
INSERT INTO EventDataSpring.events_entity (event_id, event_amount, event_category, event_details, event_img1, event_img2, event_img3, event_name)
 VALUES ('1', '85000', 'Birthday', 'Birthday event Data', 'Birthday8.jpg', 'Birthday2.jpg', 'Birthday3.jpeg', 'Birthday');

INSERT INTO EventDataSpring.events_entity (event_id, event_amount, event_category, event_details, event_img1, event_img2, event_img3, event_name) 
VALUES ('', '75000', 'Marriage', 'Wedding event Data', 'wedding.jpeg', 'wedding2.jpg', 'wedding3.jpeg', 'Wedding');
