## What is it?
Java project that populate faker data on DynamoDB tables using the aws-sdk version 2.

## Pre-requisites
1. [Git](https://git-scm.com/downloads).
2. OpenJDK 17. You can use [SDK Man](https://sdkman.io/install).
3. [Maven](https://maven.apache.org/download.cgi).

## Packaging Java application
This project uses Apache Maven:
```
mvn clean package
```

## Running Java application
This project must run in a terminal window:
```
java -jar target/java-faker-dynamodb-example.jar
```

## Exporting created data from DynamoDB to JSON files on S3
1. Go to AWS Console and select DynamoDB service.
2. In the menu select the option "Export to S3".
3. Select the table that you want to export, and the bucket name to store the exporting files.
4. When the process will finish, go to the selected S3 bucket and download the .gz files generated.
5. On Mac, use the *gunzip* command to decompress those files, and you can open it.
