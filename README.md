# IMS
Intern Management System Java 

//Connection Database AnujDev67
import java.sql.*;
import javax.swing.*;
public class Connect {
Connection con=null;
public static Connection ConnectDB(){
    
               try{
           
          Class.forName("com.mysql.jdbc.Driver");
         Connection con = DriverManager.getConnection("jdbc:mysql://localhost/tps_db","root","");
          return con;
            
        }catch(ClassNotFoundException | SQLException e){
            JOptionPane.showMessageDialog(null, e);
            return null;
    
    }      
}
}


//or this method 
import java.sql.*;

public class Connect {
    public static Connection ConnectDB() {
        try {
            Class.forName("com.mysql.cj.jdbc.Driver"); // Updated driver class name for MySQL 8 and later
            Connection con = DriverManager.getConnection("jdbc:mysql://localhost/tps_db?useSSL=false", "root", "");
            return con;
        } catch (ClassNotFoundException | SQLException e) {
            e.printStackTrace(); // Print the error stack trace for debugging
            return null;
        }
    }
    
    public static void main(String[] args) {
        Connection connection = ConnectDB();
        if (connection != null) {
            System.out.println("Connected to the database.");
            // You can perform database operations here
        } else {
            System.out.println("Failed to connect to the database.");
        }
    }
}
