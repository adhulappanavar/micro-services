# micro-services

Building the User Microservice Jar File
----------------------------------------
Step 1 : Change to directory to  micro-services/ecommerce-microservices/user-microservice

Step 2 : Run $ mvn package

Step 3 : The above will create a JAR in the target directory

Building jar: target/user-microservice-0.0.1-SNAPSHOT.jar

Running the User Microservice (JAR)
--------------------------------------
 $ java -jar target/user-microservice-0.0.1-SNAPSHOT.jar
 
 
Running the Gatling test using Maven
-------------------------------------
Step 1 : Open another command prompt

Step 2 : Change to directory micro-services/tests/user-microservice-gatling-tests

Step 3 : mvn clean gatling:execute

References :
-------------
1. Checkout the original video at https://www.youtube.com/watch?v=U8nmVUBRmFQ&t=372s
2. Orginal Github URL - https://github.com/dheeraj-mummareddy/micro-services

