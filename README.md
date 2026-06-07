# Introduction to Linux

**Below is the process and code to connect linux server. It also involves creating a database**

**1. Connecting to server**
ssh root@159.65.222.96

**2. Changing working Directory**
mkdir BrianM

**3. Listing**
ls

**4. Checking if Postgres is working.**
psql --version

**5. Connecting to postgres**
sudo -i -u postgres

**6. Creating Database**
CREATE DATABASE BrianM

**7. Creating Schema**
CREATE SCHEMA staging

**8. CREATING TABLE**

CREATE TABLE staging.employees (
    employee_id INT,
    employee_name VARCHAR(100),
    department VARCHAR(50),
    salary NUMERIC(10,2));

**9. Inserting Data**
INSERT INTO staging.employees VALUES
(1,'Brian Muriiki','Data Engineer',85000),
(2,'Mary Wanjiku','Finance',95000),
(3,'David Otieno','HR',70000);
   







