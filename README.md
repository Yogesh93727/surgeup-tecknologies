# surgeup-tecknologies

package surgeup;
import java.sql.*;

 * @author yogesh joshi
 */
public class yogesh {
    public static void main(String[]args){
       // Connection con*null;
       try{
           Class.forName("com.mysql.jdbc.Driver");
           System.out.println("driver loaded");
           DriverManager.getConnection("jdbc:mysql://localhost:3306/surgeup","root","");
           System.out.println("connection established");
        } 
       catch(ClassNotFoundException a){
           System.out.println("exception "+a.getMessage());
       }
       catch(SqlException a){
           System.out.println("Sql Exception "+a.getMessage());
       }
       
    }
}
}
