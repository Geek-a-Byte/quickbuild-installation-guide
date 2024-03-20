# quickbuild-installation-guide

## Server Installation Guide
- https://wiki.pmease.com/display/QB80/Server+Installation+Guide
- https://www.pmease.com/downloads

- https://dev.mysql.com/downloads/mysql/
- https://dev.mysql.com/downloads/workbench/ --> set path in env system variable as "C:\Program Files\MySQL\MySQL Server 8.3\bin"

- https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html --> set path in env user variable as "C:\Program Files\Java\jdk1.8.0_202\bin"
- https://dev.mysql.com/downloads/connector/j/ --> save the driver jar file under quickbuild installation directory/plugins/com.pmease.quickbuild.libs


- In C:/quickbuild-14.0.7/conf folder, open hibernate file and change the root and password according to your mysql setup


```cpp
hibernate.dialect=org.hibernate.dialect.MySQL5InnoDBDialect
hibernate.connection.driver_class=com.mysql.cj.jdbc.Driver
hibernate.connection.url=jdbc:mysql://localhost:3306/quickbuild?serverTimezone=UTC&allowPublicKeyRetrieval=true&useSSL=false&disableMariaDbDriver=true
hibernate.connection.username=root
hibernate.connection.password=root
```

- Open cmd in C:\quickbuild-14.0.7\bin run ``server.bat console``
