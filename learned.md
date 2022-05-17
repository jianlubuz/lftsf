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
