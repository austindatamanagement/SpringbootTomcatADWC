Updated: December 10, 2018

## Introduction

This lab guide will walk you through the process of creating a User Credential in Autonomous Database through Notebook.

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

## Objectives

- Create credential.

## Required Artifacts

- An oracle cloud account with Autonomous Data Warehouse Cloud Service.
- Dataset uploaded in Object Storage
- Notebook imported in Oracle Machine Learning.

### **STEP 1**: Create a **Credential**.

- **Get Auth token.**

    - Go to Oracle Compute instance. Click on **Menu**, **Identity**, **Users**.
    
      ![](images/SpringbootWebApp/compute34.png)
        
    - Click on your username.
    
      ![](images/SpringbootWebApp/compute35.png)
    
    - Click on **Auth Tokens**. 
    
      ![](images/SpringbootWebApp/compute36.png)  
     
    - Click on **Generate Token**  
     
      ![](images/SpringbootWebApp/compute37.png)
        
    - Give a **Description** and click on **Generate Token**
    
      ![](images/SpringbootWebApp/compute38.png)
    
      **Note:  Make sure to save the token in a text file for future reference.** 
 
- **Create Credential** 
      
    - Go back to your Notebook which you just imported in OML.
    
    - Change the following parameters in your first script:
      
      - **username**: `your username`
    
      - **password**: `Generated token`
      
      **Script should look like**: 
      
       ![](images/SpringbootWebApp/script.png)
            
    - **Run the script** by clicking on the run button on the top right of the script.

      ![](images/SpringbootWebApp/run.png)
