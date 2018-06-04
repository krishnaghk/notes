# Spring Core

----------
### What is the difference between BeanFactory and ApplicationContext interfaces ?
BeanFactory is Legacy interface and ApplicationContext is sub-interface of BeanFactory.
BeanFactory exists for backward compatibility.

BeanFactory supports

 * XMLBeanFactory implementation
 
```java
BeanFactory factory = new XmlBeanFactory(new FileInputStream("spring-context.xml"));
HelloWorld helloWorld = (HelloWorld) factory.getBean("helloWorld");
```

ApplicationContext supports

 * ClassPathXmlApplicationContext/FileSystemXmlApplicationContext/XmlWebApplicationContext implementation
 * Annotation Support
 * Internationalization
 * ApplicationEvent publication to the registered listeners

```java
ApplicationContext context = new ClassPathXmlApplicationContext("spring-core-context.xml");

//You can even pass multiple bean configuration files as following
ApplicationContext context = new ClassPathXmlApplicationContext("spring-core-context.xml", 
  "spring-service-context.xml");
```
 
