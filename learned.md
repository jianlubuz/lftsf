### 1. 在注释中写代码这样写
A {@code null} return value is not an error



### 2. `spring-webmvc`模块下每一个包，每一个子包都有`package-info.java`



### 3.  Collections.unmodifiableList



### 4. `@Repository`dao层 component



### 5. mvn 单独下载指定jar包

**Short form:**

```
mvn dependency:get -Dartifact=GROUPID:ARTIFACTID:VERSION:PACKAGING:CLASSIFIER -DrepoUrl=repo1.maven.org
```

**Longer form (default packaging may be omitted):**

```
mvn dependency:get -DgroupId=com.atomikos -DartifactId=transactions-jta -Dversion=3.8.0 -Dclassifier=sources -DrepoUrl=repo1.maven.org
```

**Super-long form, when a designated version of dependency plugin is needed (i.e. because the "classifier" parameter is available since 2.3):**

```java
mvn org.apache.maven.plugins:maven-dependency-plugin:2.3:get -DgroupId=com.atomikos -DartifactId=transactions-jta -Dversion=3.8.0 -Dclassifier=sources -DrepoUrl=repo1.maven.org
```

e.g

`mvn dependency:get -Dartifact=com.free:database-client:0.0.1-SNAPSHOT`



### 6. For instance, if you are running your application by using `java -jar`, you can enable the `debug` property as follows:

```shell
$ java -jar myproject-0.0.1-SNAPSHOT.jar --debug
```



### 7. 就绪状态英语

`Readiness State`



### 8. Event listeners should not run potentially lengthy tasks as they execute in the same thread by default. Consider using application and command-line runners instead.

### 9. The following example shows how to specify two distinct files:

```shell
$ java -jar myproject.jar --spring.config.location=\
    optional:classpath:/default.properties,\
    optional:classpath:/override.properties
```

|      | Use the prefix `optional:` if the [locations are optional](https://docs.spring.io/spring-boot/docs/2.6.6/reference/html/features.html#features.external-config.files.optional-prefix) and you do not mind if they do not exist. |
| ---- | ------------------------------------------------------------ |
|      |                                                              |

 ### 10. 子目录 `subdirectories`

