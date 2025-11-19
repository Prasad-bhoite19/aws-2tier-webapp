# 🌐 Two-Tier Web Application (PHP + AWS RDS MySQL)  

**Author:** Prasad 

**Project Type:** AWS Cloud | Two-Tier Architecture  

**Version:** 1.0  

**License:** MIT  

---

### 🧭 Project Summary:
This project demonstrates a **Two-Tier Cloud Architecture** where:  

* The **Web Tier** is hosted on a **Linux-based EC2 instance** running **PHP and Nginx/Apache**.  
* The **Database Tier** uses **AWS RDS (MySQL)** for persistent data storage.  

It’s designed as a **beginner-friendly yet industry-relevant** implementation that simulates how scalable web apps are structured on the AWS Cloud.  

---

### 🔄 Data Flow:
**User Input → PHP Script → Database Insert → Confirmation Message**  

---

### 💡 Key Highlights:
✅ Secure connection between EC2 and RDS  
✅ Real-world 2-tier design following AWS best practices  
✅ Minimal setup and lightweight architecture  
✅ Beginner-friendly project for Cloud & DevOps learners  
✅ Easily extendable to 3-tier architecture (add API or load balancer)  

---

### 🧠 Learning Outcomes:
* Learned how to deploy a web application on **AWS EC2**  
* Understood **2-Tier Cloud Architecture**  
* Connected **PHP application with AWS RDS (MySQL)**  
* Practiced using **Linux commands** and **AWS networking setup**  

---

### 🧱 Application Overview:
The app allows users to submit data via an HTML form. The PHP backend processes this input and securely stores it inside an **RDS MySQL** database.  

**Core Components:**  
* **Frontend:** `index.html` → Form for user input  
* **Backend:** `process.php` → Handles form submission and DB connection  
* **Database:** AWS RDS (MySQL)  
* **Server:** EC2 instance with Linux OS  

---

### 📁 Folder Structure:
```
two-tier-app/
│
├── form.html # Frontend web form
├── submit.php # Handles form submission and DB connection
├── images/ # Screenshots go here
└── README.md # Project documentation
```
---

### 🛠️ Tech Stack:
* **Frontend:** HTML  
* **Backend:** PHP  
* **Database:** MySQL (RDS)  
* **Server:** Nginx on Ubuntu (EC2)  
* **Platform:** Amazon Web Services (AWS)  

---

### 🐧 Linux Commands Used:
These Linux commands were commonly used while setting up and managing the EC2 instance:  

Update the OS packages:
```
sudo apt update && sudo apt upgrade -y
```
Install Nginx:
```
sudo apt install nginx -y
```
Install PHP and required modules:
```
sudo apt install php php-mysql php-cli php-fpm -y
```
Start and enable Nginx:
```
sudo systemctl start nginx
sudo systemctl enable nginx
```
Start and enable PHP-FPM:
```
sudo systemctl start php8.3-fpm
sudo systemctl enable php8.3-fpm
```
Navigate to web root directory:
```
cd /var/www/html/
```
Upload files to web root (example using SCP from local machine):
```
scp -i your-key.pem form.html submit.php ubuntu@ec2-ip:/var/www/html/
```
Set proper permissions:
```
sudo chown -R www-data:www-data /var/www/html/
sudo chmod -R 755 /var/www/html/
```
Check PHP version:
```
php -v
```
Check Nginx status:
```
sudo systemctl status nginx
```
Connect to MySQL RDS from EC2:
```
mysql -h your-rds-endpoint -u your-username -p
```
### 🖥️ Future Enhancements:

Add CSS for better UI

Implement prepared statements for SQL security

Add validation in form submission

Introduce a Load Balancer (ALB) for horizontal scaling

Migrate to 3-Tier Architecture with a separate application layer

### 🚀 Deployment Steps:
Follow these key steps to deploy:

1️⃣ Launch an EC2 instance with Nginx/Apache and PHP installed.
2️⃣ Create a MySQL Database using AWS RDS.
3️⃣ Update your PHP files with the correct RDS endpoint, username, and password.
4️⃣ Configure security groups:

EC2 inbound: Allow HTTP (80), SSH (22)

RDS inbound: Allow MySQL/Aurora (3306) from EC2’s security group
5️⃣ Upload your project files to /var/www/html/ on EC2.
6️⃣ Start your web server and access your app via EC2 public IP.

### 🏁 Conclusion:
This project provides a complete, deployable 2-Tier Web App using AWS EC2 + RDS. It’s a foundational exercise for anyone starting their Cloud, DevOps, or AWS journey, demonstrating how real-world cloud apps are structured and deployed.

### 👤 Author:
Prasad

LinkedIn: linkedin.com/in/prasad-cloud-devops
License: MIt
----
## 📩 Connect With Me:
If you’d like to collaborate, discuss projects, or just say hello — feel free to reach out!  

### 🔗 Social & Professional Links:
- 🌐 [Portfolio Website](https://prasad-bhoite19.github.io/prasad-portfolio/)  
- 💼 [LinkedIn](http://linkedin.com/in/prasad-bhoite-a38a64223)  
- 🐙 [GitHub](https://github.com/Prasad-bhoite19)  
- ✉️ [Email](prasadsb2002@gmail.com)  

💬 Always open for opportunities in **Cloud, DevOps, and Full-Stack Projects**
