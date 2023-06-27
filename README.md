# DB configuration in SpringBoot

### Steps to configure MYSQL

* application.yml

spring:  
&ensp; datasource:    
&emsp; url: jdbc:mysql://IPAddress:3306/DatabaseName          
&emsp; username: xxxxx  
&emsp; password: xxxxx  
&emsp; driver-class-name: com.mysql.cj.jdbc.Driver  

* build.gradle

dependencies {     
&ensp; runtimeOnly 'com.mysql:mysql-connector-j'      
}

### Steps to configure SQLServer

* application.yml

spring:  
&ensp; datasource:  
&emsp; url: jdbc:sqlserver://IPAddress:5001;databaseName=xxxxx        
&emsp; username: xxxxx  
&emsp; password: xxxxx  
&emsp; driver-class-name: com.microsoft.sqlserver.jdbc.SQLServerDriver  

* build.gradle

dependencies {  
&ensp; runtimeOnly 'com.microsoft.sqlserver:mssql-jdbc'     
}


