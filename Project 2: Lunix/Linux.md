
# Bash Shell Lab

## Overview

This lab demonstrates the use of Bash shell commands on an Amazon Linux EC2 instance. The objectives include:

* Creating and working with an alias for backing up directories
* Exploring and updating the `PATH` environment variable

---

## Lab Objectives

1. **Create an alias for backups**:

   * Use the `tar` command with an alias to backup any specified folder.
   * Example usage:

     ```bash
     backup backup_companyA.tar.gz CompanyA
     ```
   * This creates a compressed `.tar.gz` archive of the `CompanyA` folder.

2. **Explore and update PATH**:

   * Understand how the `PATH` environment variable affects script execution.
   * Add `/home/ec2-user/CompanyA/bin` to `PATH` to run scripts without specifying the full path.
   * Example:

     ```bash
     PATH=$PATH:/home/ec2-user/CompanyA/bin
     hello.sh
     ```

---

## Steps Performed

### Task 1: Connect to EC2 Instance

* Download the `.pem` key file and set permissions:

  ```bash
  chmod 400 labsuser.pem
  ```
* SSH into the instance:

  ```bash
  ssh -i labsuser.pem ec2-user@<public-ip>
  ```

### Task 2: Create Backup Alias

* Confirm the current directory:

  ```bash
  pwd
  ```
* Create a backup alias:

  ```bash
  alias backup='tar -cvzf'
  ```
* Backup a folder:

  ```bash
  backup backup_companyA.tar.gz CompanyA
  ```
* Verify the backup:

  ```bash
  ls
  ```

### Task 3: Explore and Update PATH

* Navigate to the script folder:

  ```bash
  cd /home/ec2-user/CompanyA/bin
  ```
* Run the script:

  ```bash
  ./hello.sh
  ```
* Add the folder to `PATH` for easier execution:

  ```bash
  PATH=$PATH:/home/ec2-user/CompanyA/bin
  hello.sh
  ```

---

## Key Learnings

* Aliases simplify repetitive tasks, like backups, in Bash.
* The `PATH` variable controls where Linux searches for executables.
* Scripts not in `PATH` require the full path to execute.
* `tar` can compress directories into `.tar.gz` archives for backup.

---

## References

* [GNU Tar Manual](https://www.gnu.org/software/tar/manual/tar.html)
* [Linux PATH Environment Variable](https://linuxize.com/post/how-to-add-directory-to-path-in-linux/)

---
