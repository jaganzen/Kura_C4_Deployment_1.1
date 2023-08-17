<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>
<h1 align="center">C4_deployment-1.1</h1> 

## Deployment Steps:

### 1. Download the Repo 📥

   The first step is to download the Repo from Kura Labs Github account in the form of a zip file.

&nbsp;

### 2. Extract and Create a New Repo 📂

   The second step is to extract the zip file. After that, we will create a new repo and drag the contents of the extracted folder into the Github client.

&nbsp;

### 3. Procure a Personal Access Token on Github 🔑

   The third step is to procure a Personal Access Token on Github and selecting the “repo” and “admin:repo_hook” parameters, securing the access token into a safe place for our Jenkins server.

&nbsp;

### 4. Build, Test, and Deploy on Jenkins 🚧

   The fourth step is to log into our Jenkins Server to build, test and deploy our build. In order to set up the build, we will create a pipeline using our Github credentials with Jenkins Credentials Provider verification with the proper authentication using our Github username and Personal Access Token as our password.

![Deployment](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/f471c912-f731-4bd9-94de-a4edb3bffd5e)

&nbsp;

### 5. Prepare Local File for Elastic Beanstalk 📦

   Following the fourth step, we will then go back to our Github repo and download said repo as a Zip file. We will extract the contents from the folder, and then go into the folder and compress the contents inside again to make sure the Local File is prepped for Elastic Beanstalk.

&nbsp;

### 6. Setup IAM Roles on AWS 🛠️

   The sixth step is to set up our IAM roles on AWS according to our given parameters based on the service we need, choosing the “Use Case(s)”, and other specifications as outlined.

&nbsp;

### 7. Setup EC2 Instance on AWS 🚀

   The seventh step is to set up our EC2 instance on AWS where we select the type of application that we are uploading, the raw file itself, picking out our selected service roles as outlined in the instructions given by instructors.

&nbsp;

### 8. Error Mitigation ❗

   After we set up our EC2 instance we should have an application that launches, but we have come across an error. In order to mitigate the issue, I checked the Last 100 log entries. The error we received was “ModuleNotFoundError: No module named ‘application’.

![Degraded](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/92eda675-0602-4891-a9bd-8e96d845bccc)

![502 Error](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/9652d751-40f5-4ef6-b8e6-97d19916ab83)

![Error Log](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/79d08f09-de31-4561-81e0-268648a0ab20)

   Our next step will then be to go back into the Zip file we originally uploaded, extract it, and select the appropriate "module", and correct the issue. Then we will rezip the contents of our folder into a new Zip file, and reupload our Zip file into AWS.

&nbsp;

### 9. Launch URL Shortener 🚀

   Success! And our url_shortener has launched.

&nbsp;

![Success](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/5c146104-7465-4cf1-a316-bb20f74f32b8)

### 10. And now we have access to our application! 🎉

   And our application is now live 🥳

![Url Shortener](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/554b9a03-6d9c-48eb-897a-552cfa796134)

&nbsp;

### 11. And my diagram 📊

![Copy of Deployment1_1 drawio](https://github.com/jaganzen/Kura_C4_Deployment_1.1/assets/101806502/832257c1-f920-4303-b517-455f8875122c)


&nbsp;
