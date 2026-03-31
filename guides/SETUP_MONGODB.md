# MongoDB Atlas Setup Guide

## 1. Sign Up for MongoDB Atlas
1. Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. Click on "Sign Up" and fill in the required information, or sign in with your Google account.

## 2. Create a New Project
1. Once logged in, click on "Projects" in the left sidebar.
2. Click on the "Create Project" button.
3. Enter a project name and click "Next."  
   - Optionally, add team members.

## 3. Create a Database Cluster
1. After creating the project, click on "Build a Cluster."
2. Select the "Free Tier" option.
3. Choose your preferred cloud provider and region.
4. Click on the "Create Cluster" button. 
   - The cluster creation may take a few minutes.

## 4. Configure Database Access
1. In the left sidebar, click on "Database Access."
2. Click on the "Add New Database User" button.
3. Choose a username and password for your database user and click "Add User."

## 5. Configure Network Access
1. In the left sidebar, click on "Network Access."
2. Click on the "Add IP Address" button.
3. Click on "Allow Access from Anywhere" or enter a specific IP address.
4. Click on "Confirm."

## 6. Connect to Your Cluster
1. Go back to the "Clusters" view.
2. Click on the "Connect" button for your cluster.
3. Select your preferred connection method:
   - **Connect using MongoDB Shell**
   - **Connect your application**
4. Follow the on-screen instructions for your chosen method to connect to the database.

## 7. Verify Your Connection
1. Use the connection string provided to connect to your database using your application or MongoDB shell.
2. Ensure you can perform operations (e.g., create a database or a collection).

## Conclusion
You have successfully set up a free MongoDB Atlas database cluster! You can now start using it in your applications or projects.