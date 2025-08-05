# How to Setup & Run


## 🛠️ Install Node.js (Skip if already installed)

1. Visit the [official Node.js website](https://nodejs.org/en/download/)
2. Download the installer for your OS.
3. Run the installer and follow the prompts.

---

## 🚀 Run Order:
> **First run Backend**, then **Frontend & Admin**

---

## 🔧 Backend Setup Instructions

1. Open the project folder in **VS Code**
2. Open the integrated terminal  
   → Right-click the sidebar → Select **"Open in Integrated Terminal"**
3. Run:
   ```bash
   npm install
   ```
4. ### 💾 Setup MongoDB
   a. Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register)  
   b. Sign up and log in  
   c. Create a **new project**  
   d. Navigate to **Database** section and build a database  
   e. Select **M0**, choose your **region**, and create database  
   f. Create a **username & password** (Do not use `@` in password)  
   g. Finish setup and close  
   h. **Whitelist IP**: Add `0.0.0.0/0`  
   i. Click **Connect**  
   j. Choose **Compass** and copy the connection string  
   k. In the project, open `db.js` and:
   - Paste the connection string
   - Replace `<password>` with the password from step 4f  
   - Save the file

5. ### 💳 Setup Stripe
   - Open `.env` file in the **backend folder**
   - Set your secret key like:
     ```
     STRIPE_SECRET_KEY=your_stripe_secret_key
     ```

6. To start backend server:
   ```bash
   npm run server
   ```

---

## 💻 Frontend & Admin Setup

1. Open the project folder in **VS Code**
2. Open integrated terminal in the **frontend/admin folder**
3. Run:
   ```bash
   npm install
   ```
4. Wait for installation to complete. You should see the `node_modules` folder.
5. Start the frontend:
   ```bash
   npm run dev
   ```

6. Your project will now launch in your default browser.

---


