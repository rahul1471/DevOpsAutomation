# DevOpsAutomation

## In this project, I will automate the deployement, testing and development phase of software development or web development using DevOps concepts and tools like Git, GitHub, Docker and Jenkins.

### This is how this project will work:

![Pipeline](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/intro.jpeg)

1. Developer created two branch in their repo. as master and dev1, In which dev1 is trying to implement something new in their seperate branch of repo.
2. Master only consist the robust code and production level of code in which no error or ambiguity is their.
3. Here Jenkins used to automate the lengthy process of testing and deployemnt by applying the pollSCM to both of the branch.
4. Here,Jenkins constantly checking the update in the repository by which it can copy the new code to the production and testing path.
5. After the job 1 and job 2 succesfull completion, Job3 and Job4 automatically started to create testing and Production environment using containerization technique by Docker tool.
6. Till now, as developer changing the code it is reflecting to the respective environment in the real time without any manual work.
7. Now, Admin will evaluate the testing results and trigger the Job5 to merge the dev1 and master node by which it automatically deploy to the production environment and to the final product.

Here are the some screenshots of the scripts and commands used to configure the Jenkins for the whole integration:

# 1.Here in PollSCM we can assign the interval in which Jenkins will go and find the newer commit on the repository.

![Image of Job1](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job1.jpg)

# 2. After it traces the newer commit, it will trigger the following command and copy the files to the production path.

![Image of Job1](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job12.jpg)

# 3. Same as the job1, the job2 is configured to copy the newly commit files to the testing path.

![Image of job2](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job2.jpg)

![Image of job2](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job21.jpg)

![Image of job2](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job23.jpg)

# 4. Just after the completion of Job1, Job3 will be trigger to launch docker image of production environment(httpd) web server.

![Image of job3](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job3.jpg)
![Image of job3](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job31.jpg)

# 5. Just after the comletion of Job2(test job), Job4 will trigger to launch docker image of webserver to host the testing codes.

![Image of job4](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job4.jpg)
![Image of job4](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job42.jpg)
![Image of job4](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job43.jpg)

# 6. After the approval of Admin, Admin will trigger the job5 to delete the testing environment or docker image and merge of dev1 and master branch by which the code developed by the dev1 will deploy.

![Image of job5](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job5.jpg)
![Image of job5](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job51.jpg)
![Image of job5](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job52.jpg)
![Image of job5](https://github.com/rahul1471/DevOpsAutomation/blob/master/Screenshots/job53.jpg)

**This is my automation project which I created as an assignment in the online training program in MLOps by Viaml Daga sir and Linux World India.**
