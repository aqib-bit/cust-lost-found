# Deployment Instructions for Cust Lost Found

This document contains step-by-step deployment instructions for both the frontend on Vercel and the backend on Render.com, including necessary configurations for MongoDB Atlas, Cloudinary, and Gmail SMTP.

---

## Frontend Deployment on Vercel

1. **Create a Vercel Account**  
   Go to [vercel.com](https://vercel.com) and sign up for an account if you don't have one. You can use your GitHub or email to sign up.

2. **Import GitHub Repository**  
   - On your Vercel dashboard, click on "New Project".  
   - Connect your GitHub account if prompted, and import the `cust-lost-found` repository.

3. **Configure Project Settings**  
   - After importing, Vercel will detect your frontend framework.  
   - Set your environment variables from the settings tab as needed.

4. **Deploy**  
   - Once everything is set, click the "Deploy" button.  
   - Your frontend will be built and made live.

---

## Backend Deployment on Render.com

1. **Create a Render Account**  
   Visit [render.com](https://render.com) and sign up using an email address or with GitHub.

2. **Create a New Web Service**  
   - Click on "New" and then "Web Service".  
   - Choose your repository repository (`cust-lost-found`) and deploy it.

3. **Environment Variables**  
   - Go to the "Environment" section and set the necessary environment variables, including MongoDB URI, Cloudinary credentials, and Gmail credentials.

4. **Specify Build & Start Commands**  
   - Under build options, specify the commands required to build your backend, e.g., `npm install` or `yarn install`.
   - For the start command, you can use `npm start` or any relevant command for your setup.

5. **Deploy the Service**  
   - Click on "Create Web Service" to start deployment.

---

## MongoDB Atlas Setup

1. **Create a MongoDB Atlas Account**  
   Go to [mongodb.com](https://www.mongodb.com/cloud/atlas) and create an account.

2. **Create a New Project**  
   - Click on "Projects" and create a new project.

3. **Create a Cluster**  
   - Click on "Build a Cluster" and choose the free tier.  
   - Follow the prompts to set up your cluster.

4. **Database Access**  
   - Go to the Database Access section and create a new database user with read and write permissions.

5. **Network Access**  
   - Add your IP address to the IP Whitelist.

6. **Connection String**  
   - Click on the cluster, select "Connect", and configure your connection string to use in your application.

---

## Cloudinary Configuration

1. **Create a Cloudinary Account**  
   Visit [cloudinary.com](https://cloudinary.com) and sign up for an account.

2. **Obtain API Credentials**  
   - In your Cloudinary dashboard, navigate to the "Dashboard" to find your Cloud Name, API Key, and API Secret.

3. **Save Credentials in Environment Variables**  
   - Add these credentials to your Render.com environment variables.

---

## Gmail SMTP Setup

1. **Create a Google Account**  
   If you don't have one, create a Google account.

2. **Enable Less Secure Apps**  
   In your Google account settings, enable "Less secure app access" to allow your backend to send emails using SMTP.

3. **SMTP Configuration**  
   - Use the settings:  
     - SMTP Server: `smtp.gmail.com`  
     - Port: `587` (TLS)  
     - Email: Your Gmail address  
     - Password: Your Gmail password

4. **Store Credentials**  
   - Add your Gmail email and password as environment variables in Render.com.

---

By following these steps, you can successfully deploy the `cust-lost-found` project to Vercel for the frontend and Render.com for the backend.