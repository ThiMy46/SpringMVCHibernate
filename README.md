# SpringMVCHibernate

Các bước thêm Hibernate vào 1 project Spring MVC

1. Thêm thư viện hibernate trong pom.xml (mySQL, hibernate-core, spring-orm)

2. Tạo file application.properties và khai báo file này trong file config spring-servlet.xml

3. Khai báo Datasource(DriverManagerDataSource): mapping driver,url,user,password với file .properties

Khai báo sessionFactory(LocalSessionFactoryBean): mapping một số config khác với file .properties, sử dụng đối tượng dataSource, 
khai báo packagesToScan(package chứa model or entity)

4. Khai báo transactionManager(HibernateTransactionManager): quản lý những sesionFactory được tạo ra


@Entity - @Id,@GeneratedValue, @Repository - @Autowired, @Service - @Transactional, @Controller - @RequestMapping,@ModelAttribute
