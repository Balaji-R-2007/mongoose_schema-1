# **User Management System - MongoDB Schema**

## **Overview**

Design a user management system for a web application to handle user authentication, role-based access control, and profile management. The system will use a MongoDB schema to store user data.

---

create schema.js file and creat the schema in that file.

## **Schema Requirements**

### **General Requirements**

- The schema should ensure data integrity, including unique constraints and required fields.

### **User Fields**

1. **`username`**

   - **Type**: String
   - **Constraints**: Required, Unique
   - **Purpose**: Ensures each user has a distinct username.

2. **`email`**

   - **Type**: String
   - **Constraints**: Required, Unique
   - **Purpose**: Stores the user's email for communication and login.

3. **`password`**

   - **Type**: String
   - **Constraints**: Required
   - **Purpose**: Stores securely hashed user login credentials.

4. **`roles`**
   - **Type**: Array of Strings
   - **Purpose**: Defines user roles for access control (e.g., `['user', 'admin']`).

### **Profile Fields**

- An embedded document containing personal details:
  1. **`firstName`**
     - **Type**: String
     - **Purpose**: Stores the user's first name.
  2. **`lastName`**
     - **Type**: String
     - **Purpose**: Stores the user's last name.
  3. **`age`**
     - **Type**: Number
     - **Purpose**: Records the user's age.

### **Activity Tracking**

1. **`lastLogin`**
   - **Type**: Date
   - **Purpose**: Records the date and time of the user's last login.

---

## **Deliverable**

- Write a MongoDB schema for the above user management system, ensuring all required fields, unique constraints, and data types are correctly implemented.

# **How to Fork and Set Up Your Repository**

---

## **1. Fork the Repository on StackBlitz**

- You will be provided with a **StackBlitz** link for the assignment.
- Open the link in your browser and click on the **Fork** button in StackBlitz.  
  This will create a copy of the repository in your StackBlitz account.

---

## **2. Clone the Repository to Your Personal GitHub**

- After forking, you can download the project or push it directly to your personal GitHub repository:
  - **Option 1: Download and Push**
    1. Download the repository files from StackBlitz.
    2. Open your terminal/command prompt, navigate to the project folder, and run:
       ```bash
       git init
       git remote add origin <your_github_repo_url>
       ```
       Replace `<your_github_repo_url>` with your personal GitHub repository URL.
    3. Commit and push the files to your GitHub repository:
       ```bash
       git add .
       git commit -m "Completed the assignment"
       git push -u origin main
       ```
  - **Option 2: Push Directly**
    1. Use the **Push to GitHub** option in StackBlitz to directly connect and push the repository to your GitHub account.

---

## **3. Submission Instructions**

- Once your code is successfully pushed to GitHub:
  1. Copy the link to your GitHub repository.
  2. Submit the link on the assignment submission portal.  
     The link should follow this format:  
     **`https://github.com/<your_username>/<repository_name>`**

---

### **Example Submission**

If your GitHub username is `johnDoe` and the repository name is `assignment-repo`, the submission link would look like this:  
**`https://github.com/johnDoe/assignment-repo`**
