# Virtual-Smart-Library-System-VSLS
A digital library system that lets users search, borrow, and manage books online. It features smart catalog search, automated borrow/return tracking, and personalized recommendations. Developed for the VITyarthi BYOP with full documentation, diagrams, and report.
Virtual Smart Library System (VSLS)

The platform enables users to perform online book searches and borrowing operations and manage their library collections through a digital interface. The system enables users to search books through its smart catalog function while tracking borrowings and returns automatically and offering individualized book suggestions. The system exists as a part of the VITyarthi Build Your Own Project evaluation process.

🚀 Features

The system enables users to search books through title or author or genre or keyword search. The system enables users to manage their book borrowing and returning activities through automated tracking. The system generates book recommendations through an algorithm that considers user preferences. The system enables users to create accounts which support both student and administrative access. The system provides users with access to statistical data and library operational reports through its dashboard interface. The system follows a modular design structure which provides both scalability and extendability and maintains a clean system architecture.

🛠️ Technologies Used

The system uses HTML and CSS and JavaScript for its frontend development while offering React as an optional choice. The system uses Python through Flask or Django for backend development and Node.js as an alternative. The system uses MySQL and MongoDB as its database management systems. The system uses Git and GitHub for version control operations. The system uses UML and ER Modeling and Architecture Diagrams as its development tools.

📥 Installation & Setup

Users can access the repository through the following command:

git clone https://github.com/your-username/Virtual-Smart-Library-System-VSLS.git

Users need to access the project directory through their system command. The system requires users to access the Virtual-Smart-Library-System-VSLS directory.

The system requires users to run the following command to install all necessary dependencies.

The system requires users to execute the application through the command python app.py. Users can access the system through their web browser by entering http://localhost:5000 into the address bar.

⚙️ Setup Instructions

1️⃣ Prerequisites

Ensure you have installed:

Python 3.9+

pip

MySQL / MongoDB

Git

2️⃣ Clone the Repository
git clone https://github.com/your-username/Virtual-Smart-Library-System-VSLS.git
cd Virtual-Smart-Library-System-VSLS

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Configure the Database
Example MySQL Setup:
CREATE DATABASE vsls;


Update your database config in:

app/config.py


Sample:

DB_HOST = "localhost"
DB_USER = "root"
DB_PASS = "password"
DB_NAME = "vsls"

5️⃣ Run Database Migrations (if provided)
python migrate.py

6️⃣ Start the Server
python app.py

code:
import java.time.LocalDate;
private final String isbn;
private final LocalDate borrowDate;
private LocalDate dueDate;
private LocalDate returnDate;


public BorrowRecord(String recordId, String memberId, String isbn, LocalDate borrowDate, LocalDate dueDate) {
this.recordId = recordId;
this.memberId = memberId;
this.isbn = isbn;
this.borrowDate = borrowDate;
this.dueDate = dueDate;
}


public String getRecordId() { return recordId; }
public String getMemberId() { return memberId; }
public String getIsbn() { return isbn; }
public LocalDate getBorrowDate() { return borrowDate; }
public LocalDate getDueDate() { return dueDate; }
public LocalDate getReturnDate() { return returnDate; }


public boolean isReturned() { return returnDate != null; }


public void markReturned(LocalDate date) {
this.returnDate = date;
}


public boolean isOverdue() {
return !isReturned() && LocalDate.now().isAfter(dueDate);
}


@Override
public String toString() {
return String.format("Record[%s] Member:%s ISBN:%s Borrowed:%s Due:%s Returned:%s",
recordId, memberId, isbn, borrowDate, dueDate, returnDate == null ? "(not yet)" : returnDate.toString());
}
}


Open in browser:

http://localhost:5000

🧪 Testing

Run unit tests:

pytest


Tests include:

Login validation

Book CRUD tests

Borrow/return flow

Search engine tests

📂 Project Structure
VSLS/
│── README.md
│── statement.md
│── requirements.txt
│── app/
│   ├── models/
│   ├── routes/
│   ├── templates/
│   └── static/
│── docs/
│   ├── UML/
│   ├── ERDiagram.png
│   ├── ArchitectureDiagram.png
│   └── WorkflowDiagram.png
│── tests/
│── report/
│   └── VSLS_Project_Report.pdf

The system includes all necessary documentation for users to access.

Problem Statement

Functional & Non-Functional Requirements

System Architecture Diagram

Workflow Diagram

Use Case Diagram

Class/Component Diagram

Sequence Diagram

ER Diagram

Implementation Details

Testing Approach

Future Enhancements

Complete Project Report (PDF)

🔮 Future Enhancements

The system will implement AI-based semantic book search functionality. The system will implement a chatbot function to serve as a library assistant. The system will receive a mobile application version. The system will implement OTP-based authentication for user login. The system will connect to external eBook APIs for additional functionality.
