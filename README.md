## What is it?
Java project that populate faker data on DynamoDB using the aws-sdk version 2.

## Detailed components' creation/modification
You can find more detail of the configurations and components coded in this project in the following post:
[Using Java Faker to populate data on DynamoDB employing AWS-SDK](https://aosolorzano.medium.com/adding-amplify-auth-to-your-ionic-angular-projects-4c8b6337e4e6).

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

## Exporting created data from DynamoDB to S3 (Optional)
1. Go to AWS Console and select DynamoDB service.
2. In the menu select the option "Export to S3".
3. Select the table that you want to export, and the bucket name to store the exporting files.
4. When the process will finish, go to the selected S3 bucket and download the .gz files generated.
5. On Mac, use the *gunzip* command to decompress those files, and you can open it.
