# Repository Web Scripts to improve SOLR performance

This project includes Repository services to be used with Alfresco Search Services 1.5+

These services are not available by default in:

* 6.0 - 201806 GA
* 6.1 - 201901 GA
* 6.2 - 201911 GA

The improvements provided by these services and Alfresco Search Services 1.5+ are recommended when:

* Re-indexing repositories
* Using DB_ID_RANGE Sharding method

# Project

This is an ACS project for Alfresco SDK 4.0 Platform/Repo JAR Module to be deployed in Alfresco 6.0+

Run with `./run.sh build_start` or `./run.bat build_start` and verify that it:

 * Runs Alfresco Content Service (ACS)
 * Runs Alfresco Search Service (ASS)
 * Runs PostgreSQL database
 * Deploys the JAR assembled module

## Building the JAR Module

Use default Maven command (requires Java 8 for 6.0 and Java 11 for 6.1/6.2)

```
$ mvn clean package

$ ls target/*.jar
target/solr-performance-services-repo-1.0.0-tests.jar
target/solr-performance-services-repo-1.0.0.jar
```

`solr-performance-services-repo-1.0.0.jar` can be deployed to `alfresco.war`
