🌱 Plantsy – Plant Shop (React + Vite)

A simple plant shop application built with React and Vite that allows users to:

View all plants from a backend API

Add new plants

Mark plants as out of stock

Search/filter plants by name

This project demonstrates React fundamentals including state management, props, controlled forms, conditional rendering, and working with a REST API.

## Features

✅ Render all plants on page load
✅ Add a new plant (POST to backend + update UI)
✅ Toggle plant stock status (In Stock / Out of Stock)
✅ Filter plants using a search input
✅ Fully passing test suite

🛠 Tech Stack

React

Vite

JSON Server (mock backend)

Vitest + Testing Library

## Project Structure

plantshop-cr-vite/
│
├── src/
│ ├── components/
│ │ ├── App.jsx
│ │ ├── Header.jsx
│ │ ├── PlantPage.jsx
│ │ ├── PlantList.jsx
│ │ ├── PlantCard.jsx
│ │ ├── NewPlantForm.jsx
│ │ └── Search.jsx
│ │
│ ├── **tests**/
│ ├── main.jsx
│ └── index.css
│
├── db.json
├── package.json
└── README.md

## Installation & Setup

1️⃣ Clone the repository
git clone <your-repo-url>
cd plantshop-cr-vite

2️⃣ Install dependencies
npm install

3️⃣ Start the backend (JSON Server)
npx json-server --watch db.json --port 6001

Backend will run at:

http://localhost:6001/plants

4️⃣ Start the frontend (Vite)
npm run dev

App will run at:

http://localhost:5173

5️⃣ Run Tests
npm test

All test suites should pass.

## Application Behavior

🔹 Render Plants on Load

Plants are fetched from:

http://localhost:6001/plants

On load, each plant is initialized with:

inStock: true

🔹 Add New Plant

Submitting the form:

Sends a POST request to the backend

Updates frontend state immediately

New plant defaults to In Stock

🔹 Toggle Stock Status

Clicking the button:

Switches between:

In Stock

Out of Stock

Updates UI dynamically using React state

🔹 Search Functionality

The search bar:

Filters plants by name

Is case-insensitive

Updates in real-time

## Testing

The project includes automated tests that verify:

Plants render correctly on startup

Plants are not hardcoded

New plants are added correctly

Stock status toggles correctly

Search filtering works

Run tests with:

npm test

## Learning Objectives

This project demonstrates:

React state management (useState)

Side effects with useEffect

Controlled form inputs

Conditional rendering

Lifting state up

Immutable state updates

Working with REST APIs

Passing frontend test suites

👨‍💻 Author

Developed as part of a React code challenge, code completed by Mark Warunge
