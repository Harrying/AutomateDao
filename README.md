# AutomateDao
实体类自动生成器

在配置文件中设置数据库属性   
dto.driverClass = com.mysql.jdbc.Driver    
dto.jdbcUrl = jdbc:mysql://localhost:3306/hrm_db   
dto.user = xlei    //用户   
dto.password = 003197   //密码   
dto.package = org.fkjava.hrm.domain //实体类包名   
dto.mapper = org.fkjava.hrm.mapper  //映射包名   
dto.tablePrefix = hrm_            //数据库表的前缀  例如en_user  此处写en_     
     
建立一个main方法，new一个DTOHelper对象。调用creatDto()方法，运行即可，例如：
```
pblic void main(String[] args)throws Exception{
    DTOHelper dto = new DTOHelper();
    dto.createDto();
}
```
