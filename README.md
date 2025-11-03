# 🌐 Two-Tier Web Application (PHP + AWS RDS MySQL)

**Author:** Prasad
**LinkedIn:** [linkedin.com/in/prasad-cloud-devops](#)
**Project Type:** AWS Cloud | Two-Tier Architecture
**Version:** 1.0
**License:** MIT

---

## 🧭 Project Summary

This project demonstrates a **Two-Tier Cloud Architecture** where:

* The **Web Tier** is hosted on a **Linux-based EC2 instance** running **PHP and Nginx/Apache**.
* The **Database Tier** uses **AWS RDS (MySQL)** for persistent data storage.

It’s designed as a **beginner-friendly yet industry-relevant** implementation that simulates how scalable web apps are structured on the AWS Cloud.


---

## 🔄 Data Flow Summary

**User Input → PHP Script → Database Insert → Confirmation Message**

---

## 💡 Key Highlights

✅ Secure connection between EC2 and RDS
✅ Real-world 2-tier design following AWS best practices
✅ Minimal setup and lightweight architecture
✅ Beginner-friendly project for Cloud & DevOps learners
✅ Easily extendable to 3-tier architecture (add API or load balancer)

---

## 🧠 Learning Outcomes

* Learned how to deploy a web application on **AWS EC2**
* Understood **2-Tier Cloud Architecture**
* Connected **PHP application with AWS RDS (MySQL)**
* Practiced using **Linux commands** and **AWS networking setup**

---

## 🧱 Application Overview

The app allows users to submit data via an HTML form.
The PHP backend processes this input and securely stores it inside an **RDS MySQL** database.

**Core Components:**

* **Frontend:** `index.html` → Form for user input
* **Backend:** `process.php` → Handles form submission and DB connection
* **Database:** AWS RDS (MySQL)
* **Server:** EC2 instance with Linux OS

---

## 📁 Folder Structure

```
two-tier-app/
│
├── form.html        # Frontend web form
├── submit.php       # Handles form submission and DB connection
├── images/           # Screenshots go here
└── README.md         # Project documentation
```

---

## 🛠️ Tech Stack

* **Frontend:** HTML
* **Backend:** PHP
* **Database:** MySQL (RDS)
* **Server:** Nginx on ubuntu (EC2)
* **Platform:** Amazon Web Services (AWS)

---

## 🖥️ Future Enhancements

* Add CSS for better UI
* Implement prepared statements for SQL security
* Add validation in form submission
* Introduce a **Load Balancer (ALB)** for horizontal scaling
* Migrate to **3-Tier Architecture** with a separate application layer

---

## 🚀 Deployment Steps

Follow these key steps to deploy:

1. Launch an **EC2 instance** with Nginx/Apache and PHP installed.
2. Create a **MySQL Database** using AWS **RDS**.
3. Update your PHP files with the correct **RDS endpoint, username, and password**.
4. Configure **security groups**:

   * EC2 inbound: Allow HTTP (80), SSH (22)
   * RDS inbound: Allow MySQL/Aurora (3306) from EC2’s security group
5. Upload your project files to `/var/www/html/` on EC2.
6. Start your web server and access your app via **EC2 public IP**.

---

## 🏁 Conclusion

This project provides a complete, deployable **2-Tier Web App using AWS EC2 + RDS**.
It’s a foundational exercise for anyone starting their **Cloud, DevOps, or AWS** journey, demonstrating how real-world cloud apps are structured and deployed.

---

**👤 Author:** Prasad
**LinkedIn:** [linkedin.com/in/prasad-cloud-devops](#)
**License:** MIT
