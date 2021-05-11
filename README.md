# Jenkins_Setup

You can refer this official document to install jenkins in your system: https://www.jenkins.io/doc/

open your favourable linux system and update the packages installed in it

using the following command:

**sudo dnf update -y --nobest**

![image](https://user-images.githubusercontent.com/64470404/117784692-720da200-b261-11eb-9b7c-777874a59ed1.png)

now install wget command using the following command:


**sudo yum install wget**

![image](https://user-images.githubusercontent.com/64470404/117784892-a5503100-b261-11eb-9b8f-3dfadef0ea79.png)

**sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo**
![image](https://user-images.githubusercontent.com/64470404/117786268-f1e83c00-b262-11eb-99b8-0fb205b18014.png)

**sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key**

![image](https://user-images.githubusercontent.com/64470404/117786403-15ab8200-b263-11eb-90fc-e57a57c34bcb.png)

**sudo yum install jenkins java-11-openjdk-devel**
