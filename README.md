# Jenkins_Setup

You can refer this official document to install jenkins in your system: https://www.jenkins.io/doc/

open your favourable linux system and update the packages installed in it

and firstly check wether yum is configured or not(because using it after some time makes it un configured sometime so do check and if it is unconfigured
then do check how to configure yum, above file consist of a document in which it has been shown how to configure yum)
using the following command:

**sudo dnf update -y --nobest**

![image](https://user-images.githubusercontent.com/64470404/117784692-720da200-b261-11eb-9b7c-777874a59ed1.png)

now install wget command using the following command:


**sudo yum install wget**

![image](https://user-images.githubusercontent.com/64470404/117784892-a5503100-b261-11eb-9b8f-3dfadef0ea79.png)


Now run the following cmd

**sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo**

![image](https://user-images.githubusercontent.com/64470404/117786268-f1e83c00-b262-11eb-99b8-0fb205b18014.png)


**sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key**


![image](https://user-images.githubusercontent.com/64470404/117786403-15ab8200-b263-11eb-90fc-e57a57c34bcb.png)


**sudo yum install jenkins java-11-openjdk-devel**

note: it'll take some time to install jenkins in your system
![image](https://user-images.githubusercontent.com/64470404/117795002-632bed00-b26b-11eb-936f-c60e71e8c9e9.png)


