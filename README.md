# DB configuration in SpringBoot

### Steps to configure MYSQL

* application.yml

spring:
  datasource:    
    url: jdbc:mysql://IPAddress:3306/DatabaseName        
    username: xxxxx
    password: xxxxx
    driver-class-name: com.mysql.cj.jdbc.Driver  

* build.gradle	

dependencies {    
    runtimeOnly 'com.mysql:mysql-connector-j'    
}

### Steps to configure SQLServer

* application.yml

spring:
  datasource:    
    url: jdbc:sqlserver://IPAddress:5001;databaseName=xxxxx        
    username: xxxxx
    password: xxxxx
    driver-class-name: com.microsoft.sqlserver.jdbc.SQLServerDriver  

* build.gradle	

dependencies {    
    runtimeOnly 'com.microsoft.sqlserver:mssql-jdbc'    
}


