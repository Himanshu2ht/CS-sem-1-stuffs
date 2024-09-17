# Hosting a Website on AWS with Apache2 Using PowerShell
### (These are the steps after launching instance and downloading .pem passkey)<br><br><br><br><br><br>
## Step 1: Connect to EC2 Instance Using PowerShell
1. Open **PowerShell** in Windows.
2. Navigate to your PEM file:
First, ensure you’re in the directory where your .pem file is located.
Use cd to change directories:
```bash
cd path\to\your-pem-file
```
4. Use the `ssh` command to connect to your EC2 instance:
   ```bash
   ssh -i "path_to_your_key.pem" ec2-user@your_instance_public_IP
Replace path_to_your_key.pem with the location of your private key.
Replace your_instance_public_IP with the public IP of your EC2 instance.
## Step 2: Update the Package List on Your EC2 Instance
Run the following command after logging in to update your packages:
```bash
sudo apt update
```
## Step 3: Install Apache2
To install the Apache2 web server:
```bash
sudo apt install apache2 -y
```
## Step 4: Delete the Default index.html and Create Your Own
Navigate to the Apache web directory:
```bash
cd /var/www/html
```
1. Delete the default index.html file:
```bash
sudo rm index.html
```
2. Create a new index.html file:
```bash
sudo vi index.html
```
### Add your website's HTML content and save the file.

## YAY! Your link or IP adress of your instance will now work.








ChatGPT can make 
