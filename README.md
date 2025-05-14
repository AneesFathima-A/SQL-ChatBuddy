# SQL-ChatBuddy

This project is a rule-based and partially dynamic chatbot that maps natural language questions to SQL queries and retrieves data from a MySQL database. It features a simple GUI interface, making it user-friendly for querying structured data without needing to write SQL.

## Objective

The primary purpose of this project is to enable **effortless and intelligent data retrieval** for stakeholders such as **non-technical users, analysts, and managers**. By providing a natural language interface to structured data, the chatbot simplifies access to organizational information, eliminates dependency on technical teams for simple queries, and streamlines the decision-making process.

This system aims to:
- **Democratize data access** across departments
- **Reduce training overhead** by allowing users to "talk" to data
- **Save time and effort** by automating repetitive data inquiries
- Provide a **cost-effective alternative** to enterprise-grade chatbot solutions

## Features

- Rule-based chatbot using a **predefined dictionary of SQL queries**
- **Partially dynamic behavior** via Python’s `difflib` for fuzzy matching
- **Natural language to SQL mapping**
- Connects to a **MySQL database** using `mysql.connector`
- **Graphical User Interface (GUI)** for easy interaction
- Provides relevant responses by executing matched SQL queries

---

## How It Works

1. **User Input**: The user enters a natural language question through the GUI.
2. **Fuzzy Matching**: `difflib` compares the input with known question templates.
3. **Query Mapping**: If a match is found, the chatbot retrieves the corresponding SQL query from the dictionary.
4. **Database Interaction**: The SQL query is executed via `mysql.connector` to fetch the answer from the MySQL database.
5. **Response**: The chatbot displays the result in the GUI.
