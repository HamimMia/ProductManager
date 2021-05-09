# ProductManager
 ProductManager - by Spring boot
 
 
 Manual Initialization (optional)
If you want to initialize the project manually rather than use the links shown earlier, follow the steps given below:
Navigate to https://start.spring.io. This service pulls in all the dependencies you need for an application and does most of the setup for you.
Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.
Click Dependencies and select Spring Web.
Click Generate.
Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.

If your IDE has the Spring Initializr integration, you can complete this process from your IDE.

________________________________________________________________________________________________________________________________________________________
Please follow this table of content:
 1. Create MySQL Database
 2. Create Maven Project in Eclipse
 3. Configure Data Source Properties
 4. Code Domain Model Class
 5. Code Repository Interface
 6. Code Service Class
 7. Code Spring MVC Controller Class
 8. Code Spring Boot Application Class
 9. Implement List Products Feature
 10. Implement Create Product Feature
 11. Implement Edit Product Feature
 12. Implement Delete Product Feature
 13. Test and package the Spring Boot CRUD Web Application


In this Project useing dependencies>>

<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-data-jpa</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-thymeleaf</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-devtools</artifactId>
			<scope>runtime</scope>
			<optional>true</optional>
		</dependency>
		<dependency>
			<groupId>mysql</groupId>
			<artifactId>mysql-connector-java</artifactId>
			<scope>runtime</scope>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-configuration-processor</artifactId>
			<optional>true</optional>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
			<exclusions>
				<exclusion>
					<groupId>org.junit.vintage</groupId>
					<artifactId>junit-vintage-engine</artifactId>
				</exclusion>
			</exclusions>
		</dependency>
	</dependencies>
	
	
Spplication Properties >
spring.jpa.hibernate.ddl-auto=update
spring.datasource.url=jdbc:mysql://localhost:3306/sales?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=12345
server.port=8082

