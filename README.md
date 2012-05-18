greendao-mvn
============

GreenDAO Maven integration

greenDAO is a light & fast ORM solution for Android that maps objects to SQLite databases. Being highly optimized for Android, greenDAO offers great performance and consumes minimal memory.

### Contents

* greendao-example-daogenerator: Maven project as a container of the dao and dao-generator modules
** greendao-example-generator: Defines the schema and launchs the source generation
** greendao-example-dao: Target of the source generation to execute the artifact generation

* greendao-example: Android-maven project (uses the greendao-example-dao artifact)


### Build

* Go to greendao-example-daogenerator/dist and execute the maven-install.txt defined commands to install greenDAO dependencies in your local repository.
* Execute the maven install phase in greendao-example-daogenerator to generate the ORM artifact
** Generation of greendao-example-generator artifact
** Generation of greendao-example-dao artifact (the ORM API)
* Execute the maven install phase in greendao-example to generate the APK artifact