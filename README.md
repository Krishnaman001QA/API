# Trello API Automation using Postman & Newman

## Project Overview

This project automates Trello REST APIs using Postman and Newman.

The collection covers end-to-end CRUD operations for:

- Board API
- Card API
- Checklist API
- Comment API

The project is integrated with Newman for command-line execution and can be executed through Jenkins CI.

---

## Technologies Used

- Postman
- Newman
- Node.js
- Git
- GitHub
- Jenkins

---

## Project Structure

```
Postman_API_Collection
│
├── Collections
├── Environments
├── Reports
├── README.md
├── package.json
├── .gitignore
└── Jenkinsfile
```

---

## APIs Covered

### Board API

- Get All Boards
- Get Specific Board
- Get Single Board

### Card API

- Create Card
- Get Card
- Update Card
- Delete Card

### Checklist API

- Create Checklist
- Delete Checklist

### Comment API

- Add Comment
- Delete Comment

---

## How to Run

Install Newman

```
npm install -g newman
```

Run Collection

```
newman run Collections/Trello_hindi.postman_collection.json ^
-e Environments/Stg_Trello_Hindi.postman_environment.json
```

---

## CI/CD

This project can be executed using Jenkins and generates HTML reports automatically.