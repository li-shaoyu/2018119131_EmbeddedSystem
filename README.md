# 2018119131_EmbeddedSystem
《stm32单片机》课程仓库

void main(){
    int tmpVar;
}

test

test9.12

java语言测试

//测试
public class StuLoginServlet extends HttpServlet {
	private static final long serialVersionUID = 1L;
       
 
   
	protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		String name = request.getParameter("name");
		String pwd = request.getParameter("pwd");
		try{
			Class.forName("com.mysql.jdbc.Driver");
			Connection conn =DriverManager.getConnection("jdbc:mysql://localhost:3306/1909","root","629629");
			String sql="select * from person where pname=? and pwd=?";
			conn.prepareStatement(sql);
			PreparedStatement ps = conn.prepareStatement(sql);
			
			
		}catch(ClassNotFoundException e){
			e.printStackTrace();
		} catch (SQLException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
	}

	
	protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		doGet(request,response);
	}

}
