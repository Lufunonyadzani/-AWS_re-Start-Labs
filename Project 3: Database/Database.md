Here is a clean, professional **GitHub README** you can use for this lab.
I made it simple, clear, and structured — perfect for a school, AWS or SQL practice repository.

---

# 📘 Database Table Operations — AWS SQL Lab

This repository contains my notes and steps from the **Database Table Operations Lab**, where I practiced working with relational databases on an AWS-provisioned environment using MySQL.

## ✅ Lab Objectives

In this lab, I learned how to:

* ✔️ Create databases and tables using `CREATE`
* ✔️ View existing databases and tables using `SHOW`
* ✔️ Modify table structures using `ALTER`
* ✔️ Delete tables and databases using `DROP`
* ✔️ Connect to a MySQL database through an EC2 instance (Command Host)

---

## 🖥️ **Task 1: Connect to the Command Host**

Commands used to connect after opening Session Manager:

```bash
sudo su
cd /home/ec2-user/
mysql -u root --password='re:St@rt!9'
```

---

## 🗄️ **Task 2: Create Database & Tables**

### ✔️ Show databases

```sql
SHOW DATABASES;
```

### ✔️ Create a database

```sql
CREATE DATABASE world;
```

### ✔️ Create the `country` table

```sql
CREATE TABLE world.country (
  `Code` CHAR(3) NOT NULL DEFAULT '',
  `Name` CHAR(52) NOT NULL DEFAULT '',
  `Conitinent` enum('Asia','Europe','North America','Africa','Oceania','Antarctica','South America') NOT NULL DEFAULT 'Asia',
  `Region` CHAR(26) NOT NULL DEFAULT '',
  `SurfaceArea` FLOAT(10,2) NOT NULL DEFAULT '0.00',
  `IndepYear` SMALLINT(6) DEFAULT NULL,
  `Population` INT(11) NOT NULL DEFAULT '0',
  `LifeExpectancy` FLOAT(3,1) DEFAULT NULL,
  `GNP` FLOAT(10,2) DEFAULT NULL,
  `GNPOld` FLOAT(10,2) DEFAULT NULL,
  `LocalName` CHAR(45) NOT NULL DEFAULT '',
  `GovernmentForm` CHAR(45) NOT NULL DEFAULT '',
  `HeadOfState` CHAR
```
