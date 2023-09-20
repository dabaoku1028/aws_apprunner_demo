# AWS-AppRunner-Demo

### Speaker
* Aaron Huang - 2021 AWS Educate Student Ambassador @AWS 

### Reminder
* AWS AppRunner is a new service and it's not available to use promotion credits or AWS Educate to lauch service.

### Hands-on Lab
* Deployed from GitHub(using source code)
```
- STEP 0: Click "Create service" Button
- STEP 1: Source and deployment
    - Source
        * Repository type : Source code repository
        * Connect to GitHub
            1. Connection Name : <CONNECTION NAME>
            2. Repository : <GITHUB REPOSITORY NAME>
            3. Branch : <PRODUCTION BRANCH>
    - Deployment settings
        * Deployment trigger : Automatic
- STEP 2: Configure build
    - Build settings
        * Configuration file : Configure all settings here
        * Runtime : Nodejs 12
        * Build command : npm install
        * Start command : node index.js
        * Port : 3000
- STEP 3: Configure service
    - Service settings
        * Service name : <SERVICE NAME>
        * Virtual CPU & memory : default setting
    - Auto scaling(default setting)
    - Health check(default setting)
    - Security(default setting)
    - Tags(default setting)
- STEP 4: Review and create
- STEP 5: DONE!
```

* Deploy from ECR(using public image)
```
- STEP 0: Click "Create service" Button
- STEP 1: Source and deployment
    - Source
        * Repository type : Container registry
        * Provider : Amazon ECR Public
        * Container image URI : public.ecr.aws/aws-containers/hello-app-runner:latest
    - Deployment settings
        * Deployment trigger : Manual
- STEP 2: Configure service
    - Service settings
        * Service name : <SERVICE NAME>
        * Virtual CPU & memory : default setting
        * Port : 8000
    - Auto scaling(default setting)
    - Health check(default setting)
    - Security(default setting)
    - Tags(default setting)
- STEP 3: Review and create
- STEP 4: DONE!
```

### Resources
* [PowerPoint](https://drive.google.com/file/d/1AJ9VmEJ7HxCZG4cmOb2nAy_euSxnBWdE/view?usp=sharing)
* Special thanks to Nick Chao and Wyne Tan(2020 AWS Educate Student Ambassador @AWS) for the [material](https://github.com/sefx5ever/SITCON_AWS_AppRunner_Sample)


### Power By: AWS Educate
![AWS Educate](https://d1.awsstatic.com/WWPS/AWS_Educate_Logo2.914df33100523a7d60c9c897d79d1cec23cc7e0c.png)
