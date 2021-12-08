# Домашнее задание к занятию 1.4: Сборка проектов. Maven и Gradle

## Задача 1: Многомодульный проект на Maven

**v. 1.0**

Задание реализовано.

Вывод после исполнения:
```
MyEntity{id=75331a2d-18b2-48b7-af08-77ca9b777c9a, name='first'}
MyEntity{id=c688941c-c75f-411a-9c12-fcf824580cc6, name='second'}
MyEntity{id=c688941c-c75f-411a-9c12-fcf824580cc6, name='second'}
```

Вывод после инсталяции:

```
[INFO] Scanning for projects...
[WARNING]
[WARNING] Some problems were encountered while building the effective model for ru.netology:api:jar:1.0-SNAPSHOT
[WARNING] 'dependencies.dependency.(groupId:artifactId:type:classifier)' must be unique: ru.netology:service:jar -> duplicate declaration of version 1.0-SNAPSHOT @ line 20, column 21
[WARNING]
[WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
[WARNING]
[WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
[WARNING]
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO]
[INFO] homeworkNetologyJavaCore4.1                                        [pom]
[INFO] db                                                                 [jar]
[INFO] service                                                            [jar]
[INFO] api                                                                [jar]
[INFO]
[INFO] --------------< ru.netology:homeworkNetologyJavaCore4.1 >---------------
[INFO] Building homeworkNetologyJavaCore4.1 1.0-SNAPSHOT                  [1/4]
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] --- maven-install-plugin:2.4:install (default-install) @ homeworkNetologyJavaCore4.1 ---
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\pom.xml to C:\Users\iamne\.m2\repository\ru\netology\homeworkNetologyJavaCore4.1\1.0-SNAPSHOT\homeworkNetologyJavaCore4.1-1.0-SNAPSHOT.pom
[INFO]
[INFO] ---------------------------< ru.netology:db >---------------------------
[INFO] Building db 1.0-SNAPSHOT                                           [2/4]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ db ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ db ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ db ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory D:\Work\uki\Code\homeworkNetologyJavaCore4.1\db\src\test\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ db ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ db ---
[INFO] No tests to run.
[INFO]
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ db ---
[INFO] Building jar: D:\Work\uki\Code\homeworkNetologyJavaCore4.1\db\target\db-1.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-install-plugin:2.4:install (default-install) @ db ---
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\db\target\db-1.0-SNAPSHOT.jar to C:\Users\iamne\.m2\repository\ru\netology\db\1.0-SNAPSHOT\db-1.0-SNAPSHOT.jar
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\db\pom.xml to C:\Users\iamne\.m2\repository\ru\netology\db\1.0-SNAPSHOT\db-1.0-SNAPSHOT.pom
[INFO]
[INFO] ------------------------< ru.netology:service >-------------------------
[INFO] Building service 1.0-SNAPSHOT                                      [3/4]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ service ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ service ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ service ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory D:\Work\uki\Code\homeworkNetologyJavaCore4.1\service\src\test\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ service ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ service ---
[INFO] No tests to run.
[INFO]
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ service ---
[INFO] Building jar: D:\Work\uki\Code\homeworkNetologyJavaCore4.1\service\target\service-1.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-install-plugin:2.4:install (default-install) @ service ---
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\service\target\service-1.0-SNAPSHOT.jar to C:\Users\iamne\.m2\repository\ru\netology\service\1.0-SNAPSHOT\service-1.0-SNAPSHOT.jar
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\service\pom.xml to C:\Users\iamne\.m2\repository\ru\netology\service\1.0-SNAPSHOT\service-1.0-SNAPSHOT.pom
[INFO]
[INFO] --------------------------< ru.netology:api >---------------------------
[INFO] Building api 1.0-SNAPSHOT                                          [4/4]
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ api ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ api ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ api ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory D:\Work\uki\Code\homeworkNetologyJavaCore4.1\api\src\test\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ api ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ api ---
[INFO] No tests to run.
[INFO]
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ api ---
[INFO] Building jar: D:\Work\uki\Code\homeworkNetologyJavaCore4.1\api\target\api-1.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-install-plugin:2.4:install (default-install) @ api ---
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\api\target\api-1.0-SNAPSHOT.jar to C:\Users\iamne\.m2\repository\ru\netology\api\1.0-SNAPSHOT\api-1.0-SNAPSHOT.jar
[INFO] Installing D:\Work\uki\Code\homeworkNetologyJavaCore4.1\api\pom.xml to C:\Users\iamne\.m2\repository\ru\netology\api\1.0-SNAPSHOT\api-1.0-SNAPSHOT.pom
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary for homeworkNetologyJavaCore4.1 1.0-SNAPSHOT:
[INFO]
[INFO] homeworkNetologyJavaCore4.1 ........................ SUCCESS [  0.588 s]
[INFO] db ................................................. SUCCESS [  2.065 s]
[INFO] service ............................................ SUCCESS [  0.097 s]
[INFO] api ................................................ SUCCESS [  0.111 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  3.055 s
[INFO] Finished at: 2021-12-08T10:02:57+03:00
[INFO] ------------------------------------------------------------------------

Process finished with exit code 0
```