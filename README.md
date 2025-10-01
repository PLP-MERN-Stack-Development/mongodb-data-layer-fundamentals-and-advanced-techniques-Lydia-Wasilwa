# Week 1

## 🚀 Overview
This project demonstrates the fundamentals and advanced techniques of working with **MongoDB**.  
It includes creating a database, inserting book documents, performing CRUD operations, running advanced queries, and optimizing performance with indexing.

---

## 🛠️ Setup Instructions

### 1. Install MongoDB
- Download and install **MongoDB Community Edition** from [MongoDB Official Downloads](https://www.mongodb.com/try/download/community).
- Ensure that the MongoDB service (`mongod`) is running on your local machine (default port: **27017**).  
- Download and install [**MongoDB Shell**](https://www.mongodb.com/try/download/shell)

  You can test this in CMD:
  ```bash
  mongosh
  ```
  If it connects successfully, MongoDB is running.

### 2. Install Node.js
- Download and install **Node.js** from [Node.js Official Website](https://nodejs.org/).
- Verify installation:
  ```bash
  node -v
  npm -v
  ```

### 3. Clone the Repository
```bash
git clone https://github.com/PLP-MERN-Stack-Development/mongodb-data-layer-fundamentals-and-advanced-techniques-Lydia-Wasilwa.git
cd mongodb-data-layer-fundamentals-and-advanced-techniques-Lydia-Wasilwa
```

### 4. Node.js Package Setup

Once you have Node.js installed, run the following commands in your assignment directory:

```bash
# Initialize a package.json file
npm init -y

# Install the MongoDB Node.js driver
npm install mongodb
```

## 📂 Files in this Project
- `insert_books.js` → Script to insert sample book data into the `books` collection.  
- `queries.js` → Contains MongoDB queries for CRUD operations, advanced queries, and indexing.  
- `README.md` → Instructions on how to set up and run the project.  
- `screenshot.png` → Proof of MongoDB Compass showing sample data.  

---

## ▶️ Running the Scripts

### 1. Insert Books into Database
Run the provided script to insert sample book data:
```bash
node insert_books.js
```

This will connect to `mongodb://localhost:27017`, create a database called **plp_bookstore**, and insert documents into the `books` collection.

### 2. Run Queries in MongoDB Shell
Open the MongoDB shell:
```bash
mongosh
```
Then switch to your database:
```javascript
use plp_bookstore
```
Now copy-paste the queries from `queries.js` to test them.

---

## 📌 Notes
- Make sure MongoDB is running before executing the scripts.  
- Use **MongoDB Compass** if you prefer a GUI to view and manage data.  
- Indexing results can be checked with:
```javascript
db.books.getIndexes();
```

## Requirements

- Node.js (v18 or higher)
- MongoDB (local installation or Atlas account)
- MongoDB Shell (mongosh) or MongoDB Compass

## Resources

- [MongoDB Documentation](https://docs.mongodb.com/)
- [MongoDB University](https://university.mongodb.com/)
- [MongoDB Node.js Driver](https://mongodb.github.io/node-mongodb-native/) 