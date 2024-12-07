Laptop Management System :
  - This project is designed to help organizations manage their laptop inventory efficiently. It includes features for tracking laptops, assigning them to employees, scheduling maintenance, and reporting issues.

Features :
  - User Roles
    - Admin:
       - Manage laptops: Add, update, or delete laptop details.
       - Assign laptops to employees.
       - Track laptop status and view reports.
    - Employee:
       - View assigned laptops.
       - Request a new laptop.
       - Report issues with laptops.

Core Features :
  - Laptop Inventory Management: Add, update, delete laptops.
  - Laptop Assignment: Assign or reassign laptops to employees.
  - Maintenance Tracking: Log and view maintenance history.
  - Issue Reporting: Report issues with description and priority levels.
  - Search and Filter: Filter laptops by employee, status, or maintenance details.

Project Structure :
  - Frontend :
      - Built using React.js, the frontend includes:
          - Admin Dashboard: Overview cards, laptop management, and assignment workflows.
          - Employee Portal: View assigned laptops, request laptops, and report issues.
  - Backend :
      - Built using Node.js with Express.js and MongoDB as the database.
      - Implements RESTful APIs for all functionalities.
      - Role-based authentication using JWT.
   
Database Schema :
  - Laptops:
      - Fields: id, brand, model, serialNumber, status, purchaseDate
      - Status: available, assigned, maintenance

  - Employees:
      - Fields: id, name, email, department

  - Assignments:
      - Fields: id, laptopId, employeeId, assignedAt, returnedAt

  - Maintenance Logs:
      - Fields: id, laptopId, description, status, cost, loggedAt

  - Issues:
      - Fields: id, laptopId, description, priority, status, reportedBy, reportedAt

Setup Instructions :
  - Backend Setup
      - Clone the repository:
          - git clone https://github.com/Sonu2210/Laptop-Management.git
          - cd Laptop-Management/backend

      - Install dependencies:
          - npm install

      - Configure the .env file with:
          - MongoDB connection string
          - JWT secret
      
      - Start the backend server:
          - npm start

  - Frontend Setup :
      - Navigate to the frontend directory:
          - cd ../frontend

      - Install dependencies:
          - npm install

      - Start the development server:
          - npm start



