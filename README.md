# Jenkins_Setup

You can refer this official document to install jenkins in your system: https://www.jenkins.io/doc/

open your favourable linux system and update the packages installed in it

and firstly check wether yum is configured or not(because using it after some time makes it un configured sometime so do check and if it is unconfigured
then do check how to configure yum, above file consist of a document in which it has been shown how to configure yum)

using the following command:
````
sudo dnf update -y --nobest
````
![image](https://user-images.githubusercontent.com/64470404/117784692-720da200-b261-11eb-9b7c-777874a59ed1.png)

now install wget command using the following command:

````
sudo yum install wget
````
![image](https://user-images.githubusercontent.com/64470404/117784892-a5503100-b261-11eb-9b8f-3dfadef0ea79.png)


Now run the following cmd
````
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
````

![image](https://user-images.githubusercontent.com/64470404/117786268-f1e83c00-b262-11eb-99b8-0fb205b18014.png)

````sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key````


![image](https://user-images.githubusercontent.com/64470404/117786403-15ab8200-b263-11eb-90fc-e57a57c34bcb.png)


````sudo yum install jenkins java-11-openjdk-devel````

note: it'll take some time to install jenkins in your system
![image](https://user-images.githubusercontent.com/64470404/117795002-632bed00-b26b-11eb-936f-c60e71e8c9e9.png)

Now check jenkins status usng command :

````systemctl status jenkins````

![image](https://user-images.githubusercontent.com/64470404/117845363-19a8c580-b29e-11eb-9076-8a5895cbd2f6.png)

Now to start jenkins
use the following command:

````systemctl start jenkins````

![image](https://user-images.githubusercontent.com/64470404/117845545-48bf3700-b29e-11eb-82d1-d5a93aa6f4c1.png)
-----------
to open jenkins...
disable your firewall from the vm 
and write your local host ip with port no. 8080 as url to open it..


![image](https://user-images.githubusercontent.com/64470404/117847102-ae5ff300-b29f-11eb-91f3-a04091f3f170.png)


and then the very next step is to find its password..
so for that.. copy the path given there in the page..

![image](https://user-images.githubusercontent.com/64470404/117847246-cc2d5800-b29f-11eb-9c0b-7d5506f6fe8d.png)


and the next step is to paste that path in your linux..
and write the following amd to show your password

````sudo cat /var/lib/jenkins/secrets/initialAdminPassword````

![image](https://user-images.githubusercontent.com/64470404/117847490-01d24100-b2a0-11eb-94bf-17ca2c6aed0e.png)


![image](https://user-images.githubusercontent.com/64470404/117848176-a94f7380-b2a0-11eb-97b9-f82e19553333.png)

click on install plugin

![image](https://user-images.githubusercontent.com/64470404/117848686-25e25200-b2a1-11eb-8234-acefd026bdb5.png)


And now create your username and set password according to you:

![image](https://user-images.githubusercontent.com/64470404/117849946-74dcb700-b2a2-11eb-8ebe-0737cb5d96ad.png)

![image](https://user-images.githubusercontent.com/64470404/117850160-ac4b6380-b2a2-11eb-8440-672d626a3157.png)



AND THATS ALL
THIS COMPLETES JENKINS SETUP... (❁´◡`❁)
