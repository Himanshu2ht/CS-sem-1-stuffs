 # Host a website using Docker and Nginx <br/>
 - Login to your AWS account and download your passkey and launch the EC2 instance.  
- Launch PuTTY and add the IP address from instance and add key pair file and open the PuTTY terminal.
- Login to the OS by writing "ubuntu"
- After that I have to install docker in my OS .<br/>
- Now install Docker using following command:
```bash
curl -sL https://github.com/ShubhamTatvamasi/docker-install/raw/master/docker-install.sh | bash
```
-Type:
```bash
newgrp docker
```
Then type
```bash
docker ps
```
This will provides a list of the Docker containers on your machine.

- You can check your docker version by typing:
```bash
docker --version
```
- Now, to use ``Nginx`` in our container use:
```bash
docker pull nginx
```
- And:
```bash
docker run --name docker-nginx -p 80:80 nginx
```
- Now you can type your instance's IP and see Nginx default web page.
Use following command to stop the container from running:
```bash
ctrl + c
```
- Use following command to reveals that the Docker container has been exited:
```bash
docker ps -a
```
- Use following command to see container's ID
```bash
docker run --name docker-nginx -p 80:80 -d nginx
```
- Use following command to see new information about container:
```bash
docker ps
``- Use following command to stop the container:
```bash
docker stop docker-nginx
```
- Then remove default Nginx page and create new custom html file using following commands:
```bash
docker rm docker-nginx
```
```bash
mkdir -p ~/docker-nginx/html
```
Now navigate to file created:
```bash
cd ~/docker-nginx/html
```
Now create a ``index.html`` and write a html code on ``vim`` code editor:
```bash
sudo vi index.html
```
>> 17. cd html/<br/>
>> 18.ls # will show index.html file<br/>
>> 19.<br/>
>> 20.  press {"i"} # help to insert in the web server<br/>
>>  21. <html> hi </html> # write whatever you want to write I write only hi<br/>
>>  22. ctrl + c<br/>
>>  23. shift + ;<br/>
>> 24. wq   press {ENTER}<br/>
>>  25. docker run --name docker-nginx -p 80:80 -d -v ~/docker-nginx/html:/usr/share/nginx/html 