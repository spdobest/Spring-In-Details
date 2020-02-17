# Spring AOP and IOC  
The core spring can be thought of a framework and a container for managing **Business objects** and their relationship. 
  
The beauty of the framework is that, in most of the times we dont need to depend on spring specific classes and interfaces.  
  -This is unlike other frameworks, where they will force the client aplplications to depend on their prope=riety implementations.   
    
Business components in spring are **POJO**(plain old java object) or **POJI**(Plain old java interface) only, which facilititates:  
- easy unit testing in the application  
- Easy TDD (Test driven development)  
  
- There are 2 ways in which clients can use the functionality of the Spring framework  
1. BeanFactory  
2. ApplicationContext  
Both  of the above are containers.  
  
Two of the most fundamental and important packages in spring are:  
- or.springframework.beans
- or.springframework.context  

Code in these packages provides the basis for spring's ***Inversion control-IOC*** (alteranatively called Dependency Injection) eatures.  
  
The ***BeanFactory*** provides an advance configuration mechanism capable of managing beans (Objects) of any nature, Using potentially any kind of storage facility.  
  
The ***ApplicationContext*** builds on top of the ***BeanFactory*** and adds other functionality such as :  
- Easier integration with spring AOP features  
- Message Resource handling (for use in intenationalization)  
- Event propagation  
- Declarative mechanism to create the applicationContext  
  
The core API in spring is very limited and it generally involves in :  
- Configuration  
- Creating  
- and Making associatios  
between various Business components.  
  
Spring refers to these business components as Beans.  
  
The following are the core classes or the interfaces that are available in the spring for achieving the goal.  
- Resource   
- BeanFactory  
  
Interface for a resource descriptor that abstracts from the actual type of underlying resource, such as a file or class path resource.  
  
Package: org.springframework.core.io  
  
various classes which provides concrete implementation of **Recource** are  
- FileSystemResource  
-ClasspathResource  
-UrlResource  
-ByteArrayResource  
-InputStreamResource  
-ServletContextResource  
  
  
  
```
