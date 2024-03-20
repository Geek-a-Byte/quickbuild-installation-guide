# quickbuild-installation-guide

- https://wiki.pmease.com/display/QB80/Server+Installation+Guide
- https://www.pmease.com/downloads

- https://dev.mysql.com/downloads/mysql/
- https://dev.mysql.com/downloads/workbench/

- https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html
- https://dev.mysql.com/downloads/connector/j/

In C:\quickbuild-14.0.7\conf folder, open hibernate file and change the root and password according to your mysql setup
``
hibernate.dialect=org.hibernate.dialect.MySQL5InnoDBDialect
hibernate.connection.driver_class=com.mysql.cj.jdbc.Driver
hibernate.connection.url=jdbc:mysql://localhost:3306/quickbuild?serverTimezone=UTC&allowPublicKeyRetrieval=true&useSSL=false&disableMariaDbDriver=true
hibernate.connection.username=root
hibernate.connection.password=root
``
Open cmd in C:\quickbuild-14.0.7\bin
run ``server.bat console``
