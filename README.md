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


Institute IDs Has a lot of benefits :)

so first, start from the point of what is a student ID. I know many of u are aware of it, but just for the sake of completion, the Institute ID is the email id where the domain is of your school or college; for example, I am an IIT BHU student, MY institute ID is like ………..che20@iitbhu.ac.in.

the institute obviously provides this to us :)

Office 365 : with the help of institute ID, You can avail the whole Microsoft suite for free on your desktop. office 365 Also provide 1TB space in One drive (like google drive )

2. Grammarly Education: Grammarly Education Which is I am using to write this answer as well (XD) . Grammarly education is almost equal to Grammarly premium, which you can avail with your school id for free


3. Notion premium: Notion is one of the best tools for productivity. It provides you with many tools like Making a ToDo, also saves any webpage page and a lot more than that (I am still much not aware of Notion), but it is a great tool.


4. Git Hub Student Developer pack: It is one of the best things to avail with your institute ID. GitHub Gives a student pack that covers a lot and a lot of stuff related to many fields. One of the most useful is Canva Premium and domain name (For me as of now); also, you can host your website using GitHub. It is, I guess, only 10% or maybe less than that. Great deal :)


5. Coursera Campus Plan: If your institute has been registered on the Coursera campus plan, you can take 1 course each year and many projects for free from Coursera.

You can also apply for financial aids as well :)


6. Unlimited Google drive Space: If you have an institute account, there is literally no boundation on data, normally google provides us 15GB, but it becomes huge when it comes to your institute id.


7. Zoom Premium: The 40 Moin meet boundation on zoom will not be there if you have registered for Zoom for education with your institute id.


8. There are apps like Spotify, Youtube premium, Amazone Prime, Lastpass, which you can avail for free or with some discounted price like 50–60%.

So this is what I have used and remember it till now if I missed something than suggestion are welcomed in the comment section.

And if you are in an outstanding university like IISC, IITs, NITs, IISER, BITS, IIITs, these are very easy to avail for all of you.

Thanks for reading
