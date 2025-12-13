

---

#  Database Table Operations — AWS SQL Lab

This repository contains my notes and steps from the **Database Table Operations Lab**, where I practiced working with relational databases on an AWS-provisioned environment using MySQL.

## Lab Objectives

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
<img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/31b6773f-5bbf-4761-b254-1ad0f0940709" />

## 🗄️ **Task 2: Create Database & Tables**

### ✔️ Show databases command is used to show all Databases

```sql
SHOW DATABASES;
```

### ✔️ Create a database

```sql
CREATE DATABASE world;
```
<img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/d80104e5-b61d-459b-9f12-e76929684d18" />


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
<img width="1366" height="768" alt="image 3" src="https://github.com/user-attachments/assets/229d3c14-eaa3-4076-8503-97d81404e8fd" />

## 🖥️ **Task 4: Alter the Table**

Commands used to alter the Table:

```bash
ALTER TABLE world.country RENAME COLUMN Conitinent TO Continent;

```
<img width="1366" height="768" alt="image 5" src="https://github.com/user-attachments/assets/5f8f68af-eb0a-401c-9057-7dab86b12fc4" />


---

## 🖥️ **Task 5: Delete a database and tables**

Commands used to delete a database and tables:

```bash
DROP DATABASE world;
```
<img width="1366" height="768" alt="image 6" src="https://github.com/user-attachments/assets/817f8a2d-2d66-4a4b-bc3d-16cf14c1cec6" />


---
