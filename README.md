# mybatis-generator-field-comment
## introduce
my custom comment,result like this;
```java

private class Account{
              
    /**
     *   32-bit encryption
     */
    private String password;
} 
```

## install

add this to pom.xml 
```xml
<pluginRepositories>
	<pluginRepository>
		<id>mybatis-generator-my-comment</id>
		<url>https://raw.github.com/zgj1024/mybatis-generator-my-comment/mvn-repo/</url>
	</pluginRepository>
</pluginRepositories>
```

and dependencies 

```xml
<dependency>
	<groupId>com.zgj</groupId>
	<artifactId>mybatis-generator-my-comment</artifactId>
	<version>1.0.5</version>
</dependency>
```

## use

add this to your mybatis generator configuration xml file  

```xml
<commentGenerator type="com.zgj.mybatis.generator.MyCommentGenerator"/>
```