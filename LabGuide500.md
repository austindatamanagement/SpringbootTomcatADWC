Updated: December 10, 2018

## Introduction

This lab guide will walk you through the process of setting Spring Boot Application as per your Autonomous Environment. 

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

## Objectives

- Set up instant client with Autonomous Database Wallet.
- Set up environment parameters in Spring Boot Application. 

## Required Artifacts

- An oracle cloud account with Autonomous Data Warehouse Cloud Service.

### **STEP 1**: Set up instant client with Autonomous Database Wallet.  
    
- Download and follow the guideline in the document to configure instant client in your system [InstantClient](images/SpringbootWebApp/InstantClient.docx)

### **STEP 2**: Set up environment parameters in Spring Boot Application. 

- Unzip the downloaded Spring Boot application and navigate to the WebController.java file:

    ![](images/SpringbootWebApp/webcontroller.png)

- Change the following paramerters in WebController.java:

    . Service name: Your Service name.
    . TNS_ADMIN: Path of the TNS_ADMIN that you have set. 
    . User: username
    . Password: Password
    
    ![](images/SpringbootWebApp/parameters.png)

- Download ojdbc8-full.tar.gz fromt he following site: https://www.oracle.com/technetwork/database/features/jdbc/jdbc-ucp-122-3110062.html
  Unzip it and note down the location of ojdbc8.jar file alonf with the file name.
  
- Navigate to the SpringBootWarDeployment directory where the pom.xml file is located.

    ![](images/SpringbootWebApp/apploc.png)

- Make sure that you have the Maven installed. If not, follow the following link:
  https://maven.apache.org/install.html
  
- Change the location of ojdbc8.jar in the following command and run it:

  **mvn install:install-file -Dfile=location of ojdbc8.jar -DgroupId=com.github.noraui -DartifactId=ojdbc8 -Dversion=12.2.0.1 -Dpackaging=jar -DgeneratePom=true**
  

Youa re all set to go to the next lab.