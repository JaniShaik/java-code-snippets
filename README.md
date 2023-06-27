# DB configuration in SpringBoot

### Steps to configure MYSQL

* application.yml

spring: <br/>
  datasource: <br/>    
    url: jdbc:mysql://IPAddress:3306/DatabaseName <br/>        
    username: xxxxx <br/>
    password: xxxxx <br/>
    driver-class-name: com.mysql.cj.jdbc.Driver <br/>  

* build.gradle	

dependencies { <br/>   
    runtimeOnly 'com.mysql:mysql-connector-j' <br/>    
}

### Steps to configure SQLServer

* application.yml

spring: <br/>
  datasource: <br/> 
    url: jdbc:sqlserver://IPAddress:5001;databaseName=xxxxx <br/>      
    username: xxxxx <br/>
    password: xxxxx <br/>
    driver-class-name: com.microsoft.sqlserver.jdbc.SQLServerDriver <br/> 

* build.gradle	

dependencies { <br/> 
    runtimeOnly 'com.microsoft.sqlserver:mssql-jdbc' <br/>   
}


