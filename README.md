# Apache Nifi and Apache Registry
### You can run instances of Apache Nifi and Apache Registry using this compose file
#### how to use:
 1. Pull the repositry  
 2. Create a file named .env in the repository folder and add variables SINGLE_USER_CREDENTIALS_USERNAME  SINGLE_USER_CREDENTIALS_PASSWORD to it.
        SINGLE_USER_CREDENTIALS_USERNAME=admin
        SINGLE_USER_CREDENTIALS_PASSWORD=ctsBtRBKHRAx69EqUghvvgEvjnaLjFEB

 3. Run the following commands:

        cd apache-nifi/

        docker-compose up

 4. Wait around 20 seconds then open link http://localhost:8443
 5. Use the username and password set in the .env file for login
 6. To connect the Nifi application  to the registry, add the registry address (http://registry:18080) in the Nifi Setting → Registry Client
 7. Open link http://localhost:18080/nifi-registry
 8. From the settting, click on NEW BUCKET and create a bucket for storing Nifi flows
 9. Now you can save your Nifi flows in this configured registry.
