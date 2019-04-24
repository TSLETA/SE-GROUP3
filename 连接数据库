public class jdbcDrive {
public static Connection connection;
public static Statement statement;
public static ResultSet  resultset;
public static void jdbcConnection(){
  try {
		    connection = DriverManager.getConnection(jdbc.dbURL, jdbc.userName,jdbc.userPwd);
			  System.out.println("连接数据库成功！");
			} 
      catch (Exception e) 
      {
			System.out.print("SQL Server连接失败！"); 
      }
	}
	
public static void jdbcConnectionClose(){
		try {
			connection.close();
			System.out.println("数据库连接成功关闭");
		} catch (SQLException e) {
			System.out.println("数据库连接关闭失败");
		}
	}
	
public static void jdbcExecuteUpdate(String s) throws SQLException{
		jdbcConnection();
		statement=connection.createStatement();
		statement.executeUpdate(s);
	}
	
public static void jdbcExecuteQuery(String s) throws SQLException{
		jdbcConnection();
		statement=connection.createStatement();
		resultset=statement.executeQuery(s);
	}
public static void main(String [] args) {
	}
}
