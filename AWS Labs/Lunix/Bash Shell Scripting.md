
---

# Bash Shell Scripting Challenge Lab 

## Lab Objective

The purpose of this challenge lab is to demonstrate the ability to:

* Connect to an Amazon Linux EC2 instance using SSH
* Create a Bash script using automation
* Generate files dynamically without hard-coding values
* Validate results using Linux commands

---

##  Task Description

The Bash script must:

* Create **25 empty (0 KB) files**
* Use a **name + number** naming format
  Example: `lufuno1`, `lufuno2`, `lufuno3`, ...
* Automatically detect the **last existing file number**
* On each execution, the **next batch of 25 files** is created

---

##  Script Name

```
create_files.sh
```

---

## Full Bash Script

```bash
#!/bin/bash

# Set your name prefix
NAME="lufuno"

# Find the highest number used so far
LAST_NUM=$(ls ${NAME}* 2>/dev/null | sed "s/$NAME//" | sort -n | tail -1)

# If no files exist yet, start from 1
if [ -z "$LAST_NUM" ]; then
  START=1
else
  START=$((LAST_NUM + 1))
fi

# End at next 25 files
END=$((START + 24))

# Create the files
for ((i=START; i<=END; i++))
do
  touch "${NAME}${i}"
done

echo "✅ Created files ${NAME}${START} to ${NAME}${END}"
```

---


### Making the script executable

```bash
chmod +x create_files.sh
```

---

### 2️⃣ Run the script (First Execution)

```bash
./create_files.sh
```

✅ Output:

```
✅ Created files lufuno1 to lufuno25
```

---

### 3️⃣ Validate File Creation

```bash
ls -l
```

✅ Expected result:
25 empty files starting from `lufuno1` to `lufuno25`, each showing **0 KB**

---

### 4️⃣ Run Script Again (Automation Test)

```bash
./create_files.sh
```

✅ Output:

```
✅ Created files lufuno26 to lufuno50
```

✅ This confirms that:

* The script correctly detects the last file number
* Files are created automatically without hard-coded values

---

## ✅ Validation Command Used

```bash
ls -l
```

This confirms:

* File quantity
* File naming structure
* File size (0 KB)

---





## 🧠 Key Concepts Demonstrated

* Bash scripting
* File automation
* Conditional logic
* Loops
* Linux file permissions
* Directory validation

---

Tell me what format you are submitting in.

