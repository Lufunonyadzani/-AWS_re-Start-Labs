


# Introduction to Amazon DynamoDB – Lab README

## Lab Overview

This lab introduces **Amazon DynamoDB**, a fully managed **NoSQL key-value and document database** designed for applications that require **fast, consistent performance at any scale**. The lab demonstrates how I created a DynamoDB table, insert and modify data, query and scan records, and finally delete the table.


---

## Lab Objectives

By completing this lab, I was able to:

* Create a DynamoDB table
* Insert items into the table
* Modify existing items
* Query and scan the table
* Delete the DynamoDB table

---


##  Task 1: Create a New DynamoDB Table
The image shows a DynamoDB “Create table” screen with the following fields filled in:
1. Table name: Music.
2. Partition key: Artist.
3. Sort key : Song.

<img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/cb69660d-39de-4bc3-8165-b861ac84c18d" />

---
The image shows an AWS DynamoDB “Create item” screen with four attributes:

1. Artist (Partition key) – value “Pink Floyd”.
2. Song (Sort key) – value “Money”.
3. Album – value “The Dark Side of the Moon”.
4. Year – value 1973.

## Task 2: Add Data to the Table
<img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/d58e8efa-b353-4a10-b73d-1ea486727b64" />

---

## Task 3: Modify an Existing Item
<img width="1366" height="768" alt="image 3 1" src="https://github.com/user-attachments/assets/8fd64061-f550-454d-89e8-aa15603fe5d8" />
<img width="1366" height="768" alt="image 3 2" src="https://github.com/user-attachments/assets/0b4cdabd-5a96-4c3d-9386-d2617a08e776" />

---

## Task 4: Query and Scan the Table
The image shows an AWS DynamoDB query interface.

1. Value: Psy
2. Sort key: Song
<img width="1366" height="768" alt="image 4" src="https://github.com/user-attachments/assets/bcf0aa65-d3c7-4c06-a258-856f025dad08" />


## Task 5: Delete the Table
<img width="1366" height="768" alt="image 5" src="https://github.com/user-attachments/assets/a54476f4-9846-4f43-b68f-8b31e22ac246" />

