# spring-roo-customer-data-sample
Spring roo - introduction and handson - generate spring boot application

====================================

Contact and feedback:

- https://www.youtube.com/channel/UCVyvT1t3p-ciOeInzaSbIcQ

- https://github.com/TechPrudent/

- techprudent91@gmail.com

- https://trello.com/b/8QKy3byG/techprudent

- https://techprudent91.blogspot.com/

- https://www.facebook.com/techprudents/

- https://twitter.com/techprudent

- https://www.linkedin.com/in/tech-prudent-37831216b/

- https://plus.google.com/u/0/114035390968854033062

====================================

Spring roo - introduction and handson
=====================================

- Community project
- Rapid application dev framework - RAD
- active community
- 100% java
- quick projects and easy to use
- sts integration and cmd line integration

- what all you can generate on a spring roo project
	-	spring boot starter project
	- 	soap/ rest web services with json response
	-	database support for mysql, h2, oracle, db2, mssql, postgres,...
	- 	UI - html5, thymeleaf, jquery, css3, datatables
	-	spring mvc, security, cache, mail
	
Download spring roo from, https://projects.spring.io/spring-roo/

ROO_HOME
C:\spring-roo-2.0.0.RELEASE

path = %ROO_HOME%\bin;

- package
- jpa
- entity and fields
- repository
- services
- web mvc
- view
- controller respose

Customer data application

mvn spring-boot:run

https://docs.spring.io/spring-boot/docs/current/reference/html/getting-started-installing-spring-boot.html#getting-started-installing-the-cli


============================
steps followed:

mkdir hello
cd hello
roo
roo> project setup --topLevelPackage com.foo
roo> jpa setup --provider HIBERNATE --database HYPERSONIC_IN_MEMORY
roo> entity jpa --class ~.domain.Customer
roo> field string --fieldName customerName --notNull
roo> field string --fieldName age --notNull
roo> field string --fieldName gender --notNull
roo> repository jpa --all
roo> service --all
roo> web mvc setup
roo> web mvc view setup --type THYMELEAF
roo> web mvc controller --all --responseType THYMELEAF
roo> quit
mvn spring-boot:run
