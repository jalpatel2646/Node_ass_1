# Student Collection API

A simple and efficient Node.js/Express API to manage student records, calculate academic metrics like average CGPAs, identify top performers, and filter students by branch.

## 🚀 Features

- **Full Student Registry**: Access a comprehensive list of all students.
- **Top Performer Analysis**: Quickly identify the student with the highest CGPA.
- **Academic Statistics**: Calculate the average CGPA across all students.
- **Branch Filtering**: Filter and view students based on their specific department or branch.
- **Status Monitoring**: Built-in health check endpoint to ensure server stability.

## 🛠️ Technology Stack

- **Node.js**: Runtime environment.
- **Express.js**: Fast, unopinionated, minimalist web framework.
- **CORS**: Middleware to enable Cross-Origin Resource Sharing.
- **Nodemon**: Utility that monitors for changes and automatically restarts the server.

## 🏁 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [npm](https://www.npmjs.com/) (installed with Node.js)

### Installation

1. Clone or download the repository.
2. Open your terminal and navigate to the project directory:
   ```bash
   cd node_ass-1
   ```
3. Install the required dependencies:
   ```bash
   npm install
   ```

### Running the Server

**For Production:**
```bash
npm start
```

**For Development (with Auto-Reload):**
```bash
npm run dev
```

The server will be available at `http://localhost:3000`.

## 📖 API Documentation

### Base URL
`http://localhost:3000`

### Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/` | Health check endpoint. Returns server status. |
| `GET` | `/students` | Retrieves a list of all students in the collection. |
| `GET` | `/students/:id` | Get details of a specific student by their `ID`. |
| `GET` | `/students/topper` | Returns the student object with the highest CGPA. |
| `GET` | `/students/average` | Returns the average CGPA of all students. |
| `GET` | `/students/count` | Returns the total count of students. |
| `GET` | `/students/branch/:branchName` | Retrieves all students belonging to a specific branch. |

### Data Model Example

```json
{
  "id": 1,
  "name": "Aarav Sharma",
  "branch": "CSE",
  "semester": 8,
  "cgpa": 9.3
}
```

---
Generated with ❤️ for the Node.js Assignment.