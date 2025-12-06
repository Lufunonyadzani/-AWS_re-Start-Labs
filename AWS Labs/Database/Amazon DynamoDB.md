
Perfect — here is a **clean, professional `README.md`** you can use for your **Introduction to Amazon DynamoDB Lab**. This is **submission-ready** and formatted for GitHub or PDF.

---

# 📘 Introduction to Amazon DynamoDB – Lab README

## 📌 Lab Overview

This lab introduces **Amazon DynamoDB**, a fully managed **NoSQL key-value and document database** designed for applications that require **fast, consistent performance at any scale**. The lab demonstrates how to create a DynamoDB table, insert and modify data, query and scan records, and finally delete the table.

DynamoDB is widely used for:

* Web and mobile applications
* Gaming platforms
* IoT solutions
* Ad-tech systems
* High-performance APIs

---

## ✅ Lab Objectives

By completing this lab, I was able to:

* Create a DynamoDB table
* Insert items into the table
* Modify existing items
* Query and scan the table
* Delete the DynamoDB table

---

## ⏱ Estimated Duration

**35 minutes**

---

## 🛠 AWS Services Used

* Amazon DynamoDB
* AWS Management Console

---

## 🧱 Task 1: Create a New DynamoDB Table

A new DynamoDB table was created using the following configuration:

| Setting       | Value           |
| ------------- | --------------- |
| Table Name    | Music           |
| Partition Key | Artist (String) |
| Sort Key      | Song (String)   |
| Capacity Mode | Default         |
| Indexes       | Default         |

The table was successfully created and waited until the status was **Active** before proceeding.

---

## 📝 Task 2: Add Data to the Table

Three items were added to the `Music` table using different attributes to demonstrate DynamoDB’s **schema-less flexibility**.

### 🎵 Item 1:

* Artist: Pink Floyd
* Song: Money
* Album: The Dark Side of the Moon
* Year: 1973

### 🎵 Item 2:

* Artist: John Lennon
* Song: Imagine
* Album: Imagine
* Year: 1971
* Genre: Soft rock

### 🎵 Item 3:

* Artist: Psy
* Song: Gangnam Style
* Album: Psy 6 (Six Rules), Part 1
* Year: 2011
* LengthSeconds: 219

✅ Each item successfully demonstrated the ability to store **different attributes per record** without pre-defining a schema.

---

## ✏️ Task 3: Modify an Existing Item

The following update was performed:

* Artist: Psy
* Song: Gangnam Style
* Year changed from **2011 → 2012**

✅ The update was saved successfully.

---

## 🔍 Task 4: Query and Scan the Table

### ✅ Query Operation

A query was performed using:

* Artist (Partition Key): Psy
* Song (Sort Key): Gangnam Style

✅ The correct item was returned instantly.

---

### ✅ Scan Operation

A scan was performed with the following filter:

* Attribute: Year
* Value: 1971

✅ Only the song released in **1971 (Imagine – John Lennon)** was displayed.

---

## 🗑 Task 5: Delete the Table

The `Music` table was successfully deleted using the DynamoDB console:

* Action: Delete table
* Confirmation: Typed **delete**
* Result: Table permanently removed along with all stored data

---

## ✅ Learning Outcomes

This lab reinforced my understanding of:

* NoSQL data models
* DynamoDB partition & sort keys
* Schema-less database design
* Fast querying using primary keys
* Differences between **Query vs Scan**
* Safe deletion of cloud resources

---

## ✅ Lab Status

**✔ Successfully Completed**

---

If you want, I can also:

✅ Add a **Screenshots section**
✅ Add **AWS CLI-based DynamoDB commands**
✅ Convert this README into **PDF or DOCX**
✅ Add a **real-world use case section**

Just tell me what format you need next.
