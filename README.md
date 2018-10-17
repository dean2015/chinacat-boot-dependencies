### 管理依赖pom工程

这个工程的主要目的是在父pom工程无法被使用的时候，可以管理依赖此工程进行第三方库的jar依赖管理

同样，如果在父pom工程无法被使用的时候，也可以使用此工程进行开发框架中的jar包依赖管理。

### 使用方式
```
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>com.chinacat.boot</groupId>
            <artifactId>chinacat-boot-dependencies</artifactId>
            <version>1.0.0</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
```