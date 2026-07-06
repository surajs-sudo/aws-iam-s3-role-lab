![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws)
![IAM](https://img.shields.io/badge/IAM-Security-blue)
![EC2](https://img.shields.io/badge/EC2-Virtual%20Machine-orange)
![Amazon S3](https://img.shields.io/badge/S3-Storage-green)
![Cloud Security](https://img.shields.io/badge/Cloud-Security-red)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

# ☁️ AWS IAM & EC2 S3 Role Lab

> Secure AWS IAM Access Management and EC2 IAM Role Configuration for Amazon S3 Read-Only Access following the Principle of Least Privilege (PoLP).

---

## 📌 Project Overview

This project demonstrates the implementation of AWS Identity and Access Management (IAM) best practices by creating secure IAM users, organizing users into IAM groups, assigning least-privilege permissions, creating an EC2 IAM Role, and attaching the role to an EC2 instance for secure Amazon S3 Read-Only access.

The lab focuses on reducing credential exposure and implementing role-based access control (RBAC) using AWS managed policies.

---

## 🎯 Objectives

- Create IAM Users
- Create IAM User Groups
- Apply Least Privilege permissions
- Create an IAM Role for EC2
- Attach the IAM Role to an EC2 Instance
- Grant secure Amazon S3 Read-Only access
- Eliminate the need for hardcoded AWS credentials

---

## 🏗️ Architecture

```
                 AWS IAM

        +---------------------+
        |     IAM Users       |
        +---------------------+
                  |
                  |
                  ▼
        +---------------------+
        |    IAM Group        |
        | S3_ReadOnly_Group   |
        +---------------------+
                  |
                  |
 AmazonS3ReadOnlyAccess Policy
                  |
                  ▼

            EC2 Instance
        +----------------+
        |  EC2_S3_Role   |
        +----------------+
                  |
                  ▼
           Amazon S3 Bucket
          (Read Only Access)
```

---

# 🔐 Security Concepts Implemented

- Principle of Least Privilege (PoLP)
- Role-Based Access Control (RBAC)
- IAM Users
- IAM Groups
- IAM Roles
- AWS Managed Policies
- Temporary Credentials
- EC2 Instance Profile
- Secure AWS Authentication

---

# 🛠 Technologies Used

| Service | Purpose |
|----------|---------|
| AWS IAM | Identity & Access Management |
| Amazon EC2 | Virtual Machine |
| Amazon S3 | Cloud Storage |
| IAM Groups | Permission Management |
| IAM Roles | Secure Access |
| AWS Console | Management Interface |

---

# 🚀 Implementation Steps

## Step 1 — Created IAM Users

- Created IAM users.
- Configured secure identities.
- Prepared users for group-based permission management.

📸 Screenshot:

(Add Screenshot Here)

---

## Step 2 — Created IAM Group

Created an IAM Group named:

```
S3_ReadOnly_Group
```

Benefits

- Centralized permission management
- Easier administration
- Scalable identity management

📸 Screenshot:

(Add Screenshot Here)

---

## Step 3 — Attached AmazonS3ReadOnlyAccess Policy

Attached the AWS Managed Policy:

```
AmazonS3ReadOnlyAccess
```

Benefits

- Read-only access
- Prevents accidental deletion
- Follows Principle of Least Privilege

📸 Screenshot:

(Add Screenshot Here)

---

## Step 4 — Added Users to IAM Group

Added IAM Users into the group.

Benefits

- Simplifies permission assignment
- Consistent access control
- Easy future management

📸 Screenshot:

(Add Screenshot Here)

---

## Step 5 — Created EC2 IAM Role

Created an IAM Role named

```
EC2_S3_Role
```

Trusted Entity

```
Amazon EC2
```

Attached Policy

```
AmazonS3ReadOnlyAccess
```

Benefits

- Eliminates hardcoded credentials
- Uses temporary credentials
- More secure authentication

📸 Screenshot:

(Add Screenshot Here)

---

## Step 6 — Attached IAM Role to EC2

Successfully attached the IAM Role to the EC2 instance.

Benefits

- Secure authentication
- Automatic credential rotation
- AWS best practice

📸 Screenshot:

(Add Screenshot Here)

---

# 🔒 Security Best Practices

✔ Principle of Least Privilege

✔ IAM Groups instead of assigning permissions individually

✔ IAM Roles instead of Access Keys

✔ AWS Managed Policies

✔ No hardcoded AWS credentials

✔ Temporary AWS Credentials

✔ Role-Based Access Control (RBAC)

✔ Secure EC2 Authentication

---

# ⚠ Common Mistakes to Avoid

❌ Giving AdministratorAccess unnecessarily

❌ Sharing AWS Access Keys

❌ Embedding credentials inside source code

❌ Assigning permissions directly to users

❌ Using the Root Account for daily activities

❌ Ignoring IAM Roles for EC2

---

# 📚 Skills Demonstrated

- AWS IAM
- AWS EC2
- Amazon S3
- Identity & Access Management
- IAM Policies
- IAM Groups
- IAM Roles
- EC2 Instance Profiles
- AWS Security Best Practices
- Principle of Least Privilege
- Cloud Security
- Role-Based Access Control

---

# 📁 Repository Structure

```
aws-iam-s3-role-lab/
│
├── README.md
│
├── report/
│   └── AWS_IAM_Role_Assignment.pdf
│
├── screenshots/
│   ├── 01-iam-users.png
│   ├── 02-iam-group.png
│   ├── 03-policy.png
│   ├── 04-users-added.png
│   ├── 05-role-created.png
│   ├── 06-role-attached.png
│
└── images/
    └── architecture.png
```

---

# 📄 Project Report

Complete project report:

📄 **AWS_IAM_Role_Assignment.pdf**

(Add PDF Link Here)

---

# 🎓 Learning Outcomes

Through this lab I learned:

- AWS IAM fundamentals
- Identity management
- Permission management
- IAM Groups
- IAM Roles
- EC2 Role Attachment
- Secure access to Amazon S3
- AWS Security Best Practices
- Principle of Least Privilege
- Role-Based Access Control

---

# 👨‍💻 Author

**Suraj Somkuwar**

Aspiring Cloud Security & DevSecOps Engineer

GitHub:
https://github.com/surajs-sudo

---

## ⭐ If you found this project useful, consider giving it a Star!
