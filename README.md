# Implementing Azure Container Instances

## Objective

In this lab, I learnt how to implement and deploy Azure Container Instances.

## Architecture diagram
![image](https://github.com/user-attachments/assets/80099cda-fad9-4b4d-bd21-3351b223ed1c)
 


### Job Skills

- Deploying an Azure Container Instance using a Docker image.
- Testing and verifying deployment of an Azure Container Instance.


### Tools Used

- Azure portal - https://portal.azure.com
- Docker Image


## Steps





## Task 1: Deploy an Azure Container Instance using a Docker image

In this task, I will create a simple web application using a Docker image. Docker is a platform that provides the ability to package and run applications in isolated environments called containers. Azure Container Instances provides the compute environment for the container image.

1.	Sign in to the Azure portal - https://portal.azure.com.
2.	In the Azure portal, search for and select Container instances and then, on the Container instances blade, click + Create.
![image](https://github.com/user-attachments/assets/0457ea23-63a5-4944-824a-15b35d471bb9)
 
3.	On the Basics tab of the Create container instance blade, specify the following settings (leave others with their default values):
 ![image](https://github.com/user-attachments/assets/266cc540-074f-46af-8b20-00ba23757d49)

4.	Click Next: Networking > and specify the following settings (leave others with their default values):
![image](https://github.com/user-attachments/assets/53e7eef6-2f0e-425e-88e3-9f0f8d86927b)
 
5.	Click Next: Monitoring > and uncheck Enable container instance logs.
![image](https://github.com/user-attachments/assets/3aca1871-f6c6-4d13-b9bf-69bb208b67fe)
 
6.	Click Next: Advanced >, review the settings without making any changes.
![image](https://github.com/user-attachments/assets/e4101659-f2b6-47be-857c-836df9d142d6)
 
7.	Click Review + Create, ensure that the validation passed and then select Create.
![image](https://github.com/user-attachments/assets/2452fe53-7d5c-468c-84b1-0009ed75e298)
![image](https://github.com/user-attachments/assets/07f819b5-a907-4ade-9de8-40f6295e929b)



## Task 2: Test and verify deployment of an Azure Container Instance

In this task, I review the deployment of the container instance. By default, the Azure Container Instance is accessible over port 80. After the instance has been deployed, you can navigate to the container using the DNS name that you provided in the previous task.

1.	On the deployment blade, click the Go to resource link.
2.	On the Overview blade of the container instance, verify that Status is reported as Running.
 ![image](https://github.com/user-attachments/assets/d629371e-a6aa-4693-93bd-f3b13462f4a2)

3.	Copy the value of the container instance FQDN, open a new browser tab, and navigate to the corresponding URL.
4.	Verify that the Welcome to Azure Container Instance page is displayed. Refresh the page several times to create some log entries then close the browser tab.
 ![image](https://github.com/user-attachments/assets/d7015986-9104-4c6e-b587-7eb080505330)


5.	In the Settings section of the container instance blade, click Containers, and then click Logs.
![image](https://github.com/user-attachments/assets/a4163731-5968-4f6a-9304-b8c2963a991b)
 
6.	Verify that you see the log entries representing the HTTP GET request generated by displaying the application in the browser.

