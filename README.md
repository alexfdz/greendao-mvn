greenDAO Maven Integration
============

greenDAO is a light & fast ORM solution for Android that maps objects to SQLite databases. Being highly optimized for Android, greenDAO offers great performance and consumes minimal memory.

Example based in greenDAO DAOExample (https://github.com/greenrobot/greenDAO).

For more information about greenDAO see http://greendao-orm.com .

### Contents

* greendao-example-daogenerator: Maven project as a container of the dao and dao-generator modules

 > greendao-example-generator: Defines the schema and launchs the source generation
 
 > greendao-example-dao: Target of the source generation to execute the artifact generation

* greendao-example: Android-maven project (uses the greendao-example-dao artifact)


### Build

* Go to greendao-example-daogenerator/dist and execute the maven-install.txt defined commands to install greenDAO dependencies in your local repository.


* Execute the maven install phase in greendao-example-daogenerator to generate the ORM artifact

```
$ cd greendao-example-daogenerator
$ mvn clean install 
```

 >  Generation of greendao-example-generator artifact
 
 >  greendao-example-daogenerator/greendao-example-generator/target/greendao-example-generator-[version].jar

 >  Generation of greendao-example-dao artifact (the ORM API)
 
 >  greendao-example-daogenerator/greendao-example-dao/target/greendao-example-dao-[version].jar

 

 
* Execute the maven install phase in greendao-example to generate the APK artifact

```
$ greendao-example
$ mvn clean install 
```

 > Generation of greendao-example APK artifact
 
 > greendao-example/target/greendao-mvn-example-[version].apk

