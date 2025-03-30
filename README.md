# safecity

## backend
npm install bcryptjs body-parser cors dotenv express jsonwebtoken mongoose nodemon

## frontend
npm install @coreui/coreui @coreui/react @testing-library/dom @testing-library/jest-dom @testing-library/react @testing-library/user-event axios chart.js jwt-decode react react-chartjs-2 react-dom react-router-dom react-scripts recharts web-vitals


For Citizen

-- name: Lance Mirano
-- email: lance@example.com
-- password: password123
-- role: Citizen

For Officers

-- name: Peter Parker
-- email: peterparker@rcmp-grc.ca
-- password: rcmp123
-- role: officer

For Admin

-- name: Joash Daligcon
-- email: Joash.Daligcon@outlook.com
-- password: admin6467
-- role: admin






// 1. Prepare mongo DB (mongosh)  
// Insert Values for Backend  
In terminal run  

-- mongosh  
-- use safecity  

Run the following code to create options  

// For locations
db.locations.insertMany([{ name: "North" }, { name: "South" }, { name: "East" }, { name: "West" }, { name: "NorthEast" }, { name: "NorthWest" }, { name: "SouthEast" }, { name: "SouthWest" }])

// For categories
db.categories.insertMany([{ name: "Dangerous" }, { name: "Neutral" }, { name: "Safe" }])

// For statuses
db.status.insertMany([{ name: "Under Investigation" }, { name: "Resolved" }, { name: "Dismissed" }])


// 2. Import users and reports from miscellaneous  
safecity.users


// 3. Install Dependency for Backend   
-- cd backend/  
-- npm init -y  
-- npm install express mongoose bcryptjs jsonwebtoken dotenv cors body-parser  


// 4. Install Dependency for Frontend  
-- cd frontend/  
-- rm -rf node_modules package-lock.json (Fix for permission denied)  
-- npm install  
-- npm install react-router-dom axios jwt-decode chart.js react-chartjs-2  


// 5. Run backend and frontend  
-- cd backend/  
-- node server.js  
-- cd frontend/  
-- npm start  
