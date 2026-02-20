# Habit Tracker

## 1. Project Title and Summary

Habit Tracker is a web-based application designed to help users build, monitor, and maintain consistent daily habits. The system provides a structured and intuitive environment for tracking progress and analyzing performance over time.

The primary purpose of the system is to support personal productivity and self-improvement through reliable habit monitoring and statistical insights. It enables users to create structured routines, categorize habits, and evaluate their daily performance through a centralized dashboard.

### Target Users

- Individuals seeking to improve personal productivity  
- Users who want structured daily habit tracking  
- Professionals aiming to monitor long-term behavioral consistency  

---

## 2. Features

### User Authentication (JWT)
Secure authentication and authorization using JSON Web Tokens (JWT). The system ensures that only authenticated users can access and manage their personal habit data.

### Habit Creation and Management
Users can create, edit, update, and delete habits. Each habit is associated with a specific user and can be customized according to individual goals.

### Habit Categories
Habits can be organized into categories to improve structure and usability. This allows users to group habits such as Health, Study, Work, or Personal Development.

### Daily Habit Completion Tracking
Users can mark habits as completed on a daily basis. The system records completion history, enabling consistent monitoring over time.

### Dashboard with Statistics
A centralized dashboard provides visual and numerical summaries of habit performance, offering insights into daily completion rates and overall progress.

### Clean Architecture
The system follows clean architecture principles, separating concerns into distinct layers to ensure maintainability, scalability, and testability.

---

## 3. Technologies Used

### Front-end
- HTML  
- CSS  
- JavaScript  

### Back-end
- .NET Web API  
- Entity Framework Core  
- JWT Authentication  

### Database
- Relational database (SQL Server or PostgreSQL)  

---

## 4. System Architecture

The system follows a layered clean architecture approach. Responsibilities are separated into distinct layers to maintain a clear boundary between business logic, infrastructure, and presentation.

- The front-end communicates with the back-end through RESTful HTTP endpoints.  
- The back-end is implemented using .NET Web API.  
- Business rules are encapsulated within the application and domain layers.  
- Data persistence is handled using Entity Framework Core with a relational database.  

This architectural design improves maintainability, scalability, and long-term extensibility.

![ARQ DIAGRAM](https://github.com/user-attachments/assets/177bafbf-623f-4a49-9139-cd016edfed8d)

---

## 5. ERD (Entity Relationship Diagram)

The Entity Relationship Diagram (ERD) represents the structure of the relational database. It illustrates how core entities such as Users, Habits, Categories, and HabitRecords relate to each other.

The ERD ensures data normalization, consistency, and proper relational mapping between tables.

![CLASS DIAGRAM](https://github.com/user-attachments/assets/f4f5c7b4-7cf8-44ae-bc17-a2d257ac7956)


## 6. Use Case Diagram

The Use Case Diagram describes the main interactions between users and the system. It outlines authentication, habit management, category organization, and daily tracking operations.

![USE CASE](https://github.com/user-attachments/assets/fffc65a4-66e0-4fef-8cc5-472471a9d347)


---

## 7. Class Diagram

The Class Diagram illustrates the object-oriented structure of the system. It defines the primary domain entities, their attributes, and relationships within the application.

![CLASS DIAGRAM](https://github.com/user-attachments/assets/b2a289ba-d4eb-4cbd-8bf1-9d5ce6d94a5e)

---

## 8. Project Folder Structure

HabitTracker/
│
├── backend/
│   ├── HabitTracker.API/
│   ├── HabitTracker.Application/
│   ├── HabitTracker.Domain/
│   ├── HabitTracker.Infrastructure/
│   └── HabitTracker.Tests/
│
├── frontend/
│   ├── css/
│   ├── js/
│   ├── pages/
│   └── index.html
│
├── docs/
│   ├── diagramas/
│   │   ├── architecture.png
│   │   ├── erd.png
│   │   ├── casos_de_uso.png
│   │   └── diagrama_de_classes.png
│   │
│   └── README.md
│
└── README.md



---

## 9. How to Run the Project

### Back-end

1. Navigate to the backend directory:

cd backend


2. Configure the database connection string in the `appsettings.json` file.

3. Apply database migrations:

dotnet ef database update


4. Run the API:

dotnet run


5. The API will be available at:

https://localhost:5001


### Front-end

1. Navigate to the frontend directory:

cd frontend


2. Open `index.html` directly in a web browser  
or  

3. Run a local development server (recommended):

npx serve .


4. Ensure that the API base URL configured in the JavaScript files matches the back-end address.

---

## 10. Future Improvements

- Implementation of notification reminders  
- Habit streak tracking system  
- Mobile version of the application  
- Dark mode interface option  

---

## 11. License

This project is licensed under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANT
