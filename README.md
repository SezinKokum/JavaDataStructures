# KNOWLEDGE SHARING PLATFORM

Platform is an application which you can search for TedTalks.

## Reading the CSV File

You must change the path in the ReadAndInsertCSVToDb.java class code where your csv file is in your system.

```
CSVReader br = new CSVReader(new FileReader("YOUR PATH MUST BE HERE"));

```

## Connecting your DB with Platform

In application.properties file you must do these changes according to your MYSQL db settings.  You must write your own DB url, username and password.
```
spring.datasource.url=jdbc:mysql://localhost:3306/platform?useUnicode=true&useLegacyDatetimeCode=false&serverTimezone=Turkey

spring.datasource.username=root
spring.datasource.password=platform
```

## How to Run?

When you imported the code and connected your DB with PLATFORM you can run the code. 

You can run as Java Application the PlatformApplication.java class, it will create tedtalk and user tables into your db. All the records in csv file will also be inserted at this stage. 

You can make queries from your DB or you can search for TedTalks from Postman. 

You can review the calls I made via Postman an the results in the DocumentationTedTalk.pdf file.
