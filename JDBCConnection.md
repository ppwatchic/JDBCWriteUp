##How to create JDBC connection?

**A**: Two steps to create JDBC connection:  
* Register the database driver with java.sql.DriverManager, where DriverManager is a class which is given under JDBC specifications. 
Use a Class.forName() like this: 'Class.forName("com.mysql.jdbc.Driver");'.   
* Open a session (or connection) to the database. By calling DriverManager.getConnection(parameters) method, which returns Connection Object. 

**PS**The connection should be close at the end. 
