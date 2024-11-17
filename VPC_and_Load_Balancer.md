# CREATING A VPC AND LOAD BALANCER

* First we have to go on to aws , then we have to go on to VPC (Virtual Private Cloud).
* Thn we have to create a vpc with our choice name tags and thn create.
* Next step , is to make subnet , here we are making 4 subnet were 2 subnets are private with two different zones , and other two subnets are ublic subnets which are also , with two other different zones , we have to check also that one private and one public subnets has same zones .
* ![subnetscreation](https://github.com/user-attachments/assets/8bfe36be-3f1e-4ba8-8537-3d05cc1b7821)

* After createing the subnets , we have to create IGW (Internet Gatways), after creation we have to attach that to our VPC that we have created
* ![creating igw ](https://github.com/user-attachments/assets/b823b827-522e-4e56-9c43-fb84948f51e7)
* ![attach to vpc igw](https://github.com/user-attachments/assets/ccf19fa4-c5e8-4eaa-8c82-15fae8fb9b78)

* Then we have to create the VGW(Virtual Gateway), it has also be connect to our VPC .
* ![attaching vgw wit the vpc](https://github.com/user-attachments/assets/233c2504-27c2-4070-bb53-dbcf46486686)
* ![creating vgw ](https://github.com/user-attachments/assets/60cd06bd-428b-4397-af81-73e986881323)

* After that we have to create the 2 Route table where one is for IGW and other is for VGW also we have to associte the public subnets with the IGW route table and private once with VGW route table .
* In the below images I have change some settings of rooute tables where I have connect them to my IGW & VGW , with some other port number .
* ![creating route tables](https://github.com/user-attachments/assets/cf513e63-9693-45ba-bba0-248524a7b673)
* ![associating subnets to the route tables](https://github.com/user-attachments/assets/28e4200e-9457-46a7-8343-0a960d0645ed)
* ![editing route table r1 ](https://github.com/user-attachments/assets/23ef3efa-099e-4d0d-9f98-52815bad9197)
* ![in r1 ip](https://github.com/user-attachments/assets/d2be1bef-adec-498c-9958-518d571eea32)
* ![for r2 ](https://github.com/user-attachments/assets/02110d42-4dda-409f-917b-90502fa4e7e3)

* After completion of that task , we have to make two EC2 instnaces which will help in our load balancer task, where we have changes the settings of EC2 instnaces these setting are done on both the instnaces .
* ![changing settings in the ec2 unstance](https://github.com/user-attachments/assets/7ae32a2b-938c-4f18-a376-d66ac88ea46c)
* ![created the ec2 instances ](https://github.com/user-attachments/assets/109b2d21-c81e-47ff-8f5e-fa80c0e864fa)
* ![adding a web server on the instance](https://github.com/user-attachments/assets/6231f8f3-f420-4172-a21d-96be26d31795)
* 
* After the creation we have to add the web server on that , so I have enter the Apache2 server on the both the instances .

* Then we have to create the load balancer , and we have to create the target gr also where we have to connect our instnaces , alos we haveto edit the health check setting which are requied
* ![crreating a load balancer](https://github.com/user-attachments/assets/f896d602-a3ac-4c0d-a43f-32b133ea5da6)
* ![creataed the load balancer](https://github.com/user-attachments/assets/12a42278-a2bc-4133-80d1-24ae3f131741)
* ![settinmgs of load ](https://github.com/user-attachments/assets/62f4e224-4618-4768-b20a-18b4c56fa5da)
* ![creating target grps](https://github.com/user-attachments/assets/dc6a0846-ef2e-404c-bed6-83edd0643f3b)
* ![security grp ](https://github.com/user-attachments/assets/65e577ff-ae4a-4d6f-88b1-8b9668829c15)
* ![editing health checks](https://github.com/user-attachments/assets/5a6ea968-a6c0-414c-9bd6-6a2852eaa431)
* ![health steeing 2](https://github.com/user-attachments/assets/b45ef372-b95c-4d65-a3b6-d7149497ca18)
* ![connecting the instances ](https://github.com/user-attachments/assets/060a96d1-4ae6-4a72-9910-28dd26daeabd)

* After all the completeion we have tpo created the load balancer where , we have changes the setting .
* After creating the load balancer there is the DNS address which is to be copy and paste it to the chrome , or any other web browser .
* If you reload the page you will see the two web server of two differnet instances which you have created before.
* ![adding a web server on the instance](https://github.com/user-attachments/assets/ef14708f-858a-4741-88d6-c0d6cce891fa)

* Then on one linux web server you have to enter some commands to check the load balancer
```
seq 99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999 > /dev/null &
```
```
htop
```
![final](https://github.com/user-attachments/assets/053a2e2a-3ba3-4a0c-b8af-315bfe92aa55)
