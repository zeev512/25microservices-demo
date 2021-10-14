# Running the application
- Please enter the correct credentials in twitter4j.properties file.
- Then run mvn install -DskipTests command
- Then go to docker-compose folder and run docker-compose up command to run kafka cluster and twitter-to-kafka-service together
- Check playground module, where we have a test class to encrypt passwords using jasypt
- Check twitter-to-kafka-service and config server, where we added jasypt-spring-boot-starter dependency and
changed bootstrap.yml file and set encrypted password 
- Remember to add JASYPT_ENCRYPTOR_PASSWORD as environment variable before starting config server and twitter to kafka service