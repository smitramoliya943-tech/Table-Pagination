# 📊 React Table Pagination

A simple and responsive **React JS Table Pagination** project built using React, Bootstrap, CSS, and JSON Server.

This project displays student data in a table and provides pagination functionality with different records-per-page options.

---

## 🚀 Features

- 📋 Display student data in a table
- 🔢 Pagination functionality
- 📄 Select records per page
- ⬅️ Previous page button
- ➡️ Next page button
- 🆔 Student ID display
- 👤 Student name display
- 📚 DSA marks
- ➗ Maths marks
- 🗄️ DBMA marks
- 🌐 Networking marks
- 🔄 Data fetched from JSON Server
- 📱 Responsive design
- 🎨 Simple and clean UI
- 🟦 Bootstrap integration

---

## 🛠️ Technologies Used

- React JS
- JavaScript
- Bootstrap
- CSS
- JSON Server
- Vite
- HTML

---

## 📁 Project Structure

```text
table-pagination/
│
├── public/
│
├── src/
│   ├── assets/
│   │
│   ├── App.jsx
│   ├── App.css
│   ├── main.jsx
│   └── index.css
│
├── db.json
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md


## ⚙️ Installation

### 1. Create React Project

```bash
npm create vite@latest table-pagination -- --template react


2. Go to Project Folder

cd table-pagination

3. Install Dependencies

npm install

4. Install Bootstrap

npm install bootstrap

5. Install JSON Server

npm install json-server



▶️ Run the Project

First, start the JSON Server:

npx json-server --watch db.json --port 3000


📡 API

This project uses JSON Server for student data.

API Endpoint
GET http://localhost:3000/students

The db.json file contains student information such as:

{
  "id": 1,
  "name": "Aarav Patel",
  "dsa": 82,
  "maths": 76,
  "dbma": 89,
  "networking": 85
}
📄 Pagination

The table supports different numbers of records per page.

Available options:

5 records
10 records
20 records
50 records

Users can move between pages using:

← Previous
Next →

The current page and displayed records are also shown.

🖥️ User Interface

The application contains:

Student Table

The table displays:

Column	Description
ID	Student ID
Name	Student Name
DSA	DSA Marks
Maths	Maths Marks
DBMA	DBMA Marks
Networking	Networking Marks
🔄 How Pagination Works

The application gets all student records from the JSON Server API.

The data is divided according to the selected number of records per page.

For example:

Total Students: 100
Records Per Page: 5

Page 1 → Students 1 - 5
Page 2 → Students 6 - 10
Page 3 → Students 11 - 15
...
Page 20 → Students 96 - 100
🎨 Styling

The project uses a simple and clean UI design.

Styling is handled through:

src/App.css

Bootstrap is also used for responsive layout and form components.

📱 Responsive Design

The table layout is designed to work on:

💻 Desktop
💻 Laptop
📱 Tablet
📱 Mobile
📌 Main Concepts Learned

This project helps understand:

React Components
useState
useEffect
API Fetching
JSON Server
Pagination
Array slice()
Event Handling
Bootstrap
CSS Styling
Responsive Design
🧠 React Concepts
useState

Used for storing:

Student data
Current page
Records per page

Example:

const [allData, setAllData] = useState([]);
const [currentData, setCurrentData] = useState(1);
const [perpageData, setPerpageData] = useState(5);
useEffect

Used to fetch student data from the API when the application loads.

useEffect(() => {
  fetch(API)
    .then((res) => res.json())
    .then((data) => setAllData(data));
}, []);
📊 Pagination Logic

The starting index is calculated using:

const firstIndex = (currentData - 1) * perpageData;

The ending index is calculated using:

const lastIndex = firstIndex + perpageData;

The current page data is then selected using:

allData.slice(firstIndex, lastIndex);
🔮 Future Improvements

The project can be extended with:

🔍 Search functionality
🔃 Sorting
📊 Student marks calculation
🏆 Grade system
➕ Add student
✏️ Edit student
🗑️ Delete student
🌙 Dark mode
📈 Student performance charts
👨‍💻 Author

Smit Ramoliya

React JS / Full Stack Developer

⭐ Project

If you like this project, you can give it a ⭐ on GitHub.

📜 License

This project is created for learning and educational purposes.


**Fileનું નામ:** `README.md`

તમારા `table-pagination` folderની અંદર આ file રાખજો:

```text
table-pagination
│
├── db.json
├── package.json
├── src
└── README.md
