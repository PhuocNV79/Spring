- Congfiguration Spring Container :
  + XML configuration file (legacy, but most legacy apps still use this)
  + Java Annotations 
  + Java Source Code
  
 - Spring Development Process:
  + Configure your Spring Beans
  + Create a Spring Container (ApplicationContext)
  + Retrieve Beans from Spring Contrainer
  
 - XML configuration : file applicationContext.xml
 
 - Create a spring container : ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("applicationContext.xml");
 - Retrieve Beans from Spring Contrainer : ClassA obj = context.getBean("idBean", InterfaceName.class)
 
 - Injection Types:
  + Constructor Injection
  + Setter Injection
  
  
