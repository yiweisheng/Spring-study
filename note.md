##常用依赖
```xml

<!-- https://mvnrepository.com/artifact/org.springframework/spring-webmvc -->
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.3.4</version>
        </dependency>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.12</version>
            <scope>test</scope>
        </dependency>
```

##注解说明
- @Autowired：自动装配，通过类型、名字
    如果Autowired不能唯一自动装配上属性。则需要通过@Qualifier(value="xxx)
- @Nullable：字段标记了这个注解，说明这个字段可以为Null
- @Resource：自动装配，通过名字、类型

- @Component：组件。放在类上，说明这个类被Spring管理了，就是Bean
    dao【@Repository】
    service【@Service】
    controller【@Controller】
    这四个注解都是一样的，都是代表将某个类注册到Spring容器中，装配Bean