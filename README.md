# Node.js App with MySQL Database on AWS

## AWS Infrastructure with Terraform

This project deploys a **Node.js application** with a **MySQL database** on AWS using **Terraform** for infrastructure as code (IaC). The setup ensures scalability, security, and efficient resource management by leveraging AWS services like **EC2, RDS, S3, and VPC**.

## Architecture Overview

1. **GitHub** hosts the **Node.js** application source code.
2. **Terraform** provisions the AWS infrastructure, including:
   - **EC2 instance** to host and run the Node.js application.
   - **RDS MySQL database** for persistent data storage.
   - **S3 bucket** for file storage and retrieval.
3. The **Node.js application** securely connects to the **RDS MySQL database** via **port 3306**, with security groups enforcing access control.
4. The application interacts with **Amazon S3** for file uploads and downloads.
5. The entire setup is deployed within an AWS **VPC**, ensuring network isolation and secure communication between components.

This infrastructure provides a robust foundation for hosting and scaling a Node.js application with a relational database on AWS.

![architecture](https://github.com/user-attachments/assets/c4765ba9-e225-495e-b1a0-8d29d7e55f58)

## Getting Started

1. Add the Node Js application [source Code](https://github.com/verma-kunal/nodejs-mysql) in the directory:
   ```bash
   cd project
   git clone https://github.com/verma-kunal/nodejs-mysql.git ./app
   ```
2. Initialize the terraform project
   ```bash
   terraform init
   ```
3. Make relevant changes to the terraform code.
4. Apply the changes and provision the infrastructure:
   ```bash
   terraform apply
   ```

A simple nodejs app connected with mySQL database.

## Getting Started

1. Clone the repo

```bash
git clone https://github.com/maniadav/tf_mysql_node.git
cd tf_mysql_node
```

2. Create a `.env` file in root directory and add the environment variables:

```bash
DB_HOST="localhost"
DB_USER="root" # default mysql user
DB_PASS=""
DB_NAME=""
TABLE_NAME=""
PORT=3000
```

> Make sure to create the database and the corresponding table in your mySQL database.

3. Initialize and start the development server:

```bash
npm install
npm run dev
```

![running app](https://github.com/user-attachments/assets/d882c2ec-2539-49eb-990a-3b0669af26b6)

## Tech Stack

### **Infrastructure & Cloud**

- **AWS EC2**
- **AWS RDS (MySQL)**
- **AWS S3**
- **AWS VPC**
- **Terraform**

### **Backend**

- **Node.js**
- **Express.js**
- **MySQL**

### **Version Control & Deployment**

- **GitHub** – Code repository hosting
