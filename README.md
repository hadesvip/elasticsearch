#Elasticsearch 源码编译
> 基于Elasticsearch 7.13

## clone 源码
```java
git clone https://github.com/elastic/elasticsearch.git
git checkout --track origin/7.13
```


## 依赖版本
1. JDK
   jdk 14
2. Gradle
   * gradle7.x
   * 本地gradle 配置下仓库
   ```java
    vim ~/.gradle/init.gradle
    allprojects {
        repositories {
            maven { url 'https://maven.aliyun.com/repository/public/' }
            maven { url 'https://maven.aliyun.com/repository/spring/'}
            maven { url 'https://maven.aliyun.com/repository/gradle-plugin' }
            maven { url 'https://maven.aliyun.com/repository/google' }
            mavenLocal()
            mavenCentral()
        }
    }
    ```
注意: idea gradle 配置jvm 需要设置jdk14，项目java版本设置11即可



## 编译
1. 执行 gradle idea
2. 导入idea
