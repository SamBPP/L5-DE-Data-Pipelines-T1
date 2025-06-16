# L5-DE-Data-Pipelines-T1

Welcome to the starter repository for designing and implementing a user data pipeline project. This project leverages SQLite and Python to simulate building a simple yet extensible data pipeline.

## 🚀 Project Overview

Your objective is to:

1. **Design a Database Schema**  
   Create a schema to receive user data from an existing software application. This will initially include 10 UK-based users and their associated login timestamps.

2. **Implement a Data Pipeline**  
   Develop a Python-based pipeline that:
   - Ingests raw test data
   - Cleans and validates inputs
   - Loads the transformed data into your SQLite schema

3. **Use Test Data**  
   Provided test data includes:
   - 10 fictional UK users
   - Login timestamps in raw CSV or JSON format (provided separately or created by you)

4. **Prepare for Future Phases**  
   Consider the flexibility of your schema and pipeline. Future phases will include:
   - Users from different countries
   - Diverse timestamp formats
   - Additional fields (e.g. activity logs, geolocation)

5. **Documentation**  
   Clear and comprehensive documentation is expected:
   - Describe your database schema (tables, relationships, constraints)
   - Outline your pipeline steps (cleaning logic, validation rules, loading process)
   - Include comments in your code and a summary in this README

**Note: Collaborate with Your Instructor**  
 Your instructor will act as the stakeholder and Subject Matter Expert (SME). They will provide clarification on:
   - Schema requirements
   - Business rules for validation
   - Future data sources

---

## 🛠️ Getting Started

1. **Open in your favoured environment**  
   Launch this project in VS Code, Anaconda, Jupyter. You can also download the whole repo!

2. **Install Requirements**  
   Installs Python packages listed in `requirements.txt` using `pip install -r requirements.txt.

3. **Initialise the Database**  
   On first launch, the `init_db.sql` script is there as a demo SQL script, and the `connect.py` script shows how to connect to a database.

---

## 📦 Repository Structure

```plaintext
├── .devcontainer/           # Codespaces config
│   ├── devcontainer.json
│   └── Dockerfile
├── data/                    # Sample data files
│   ├── UK User Data.csv
│   └── UK-User-LoginTS.csv
├── .gitignore               # Hiding files that will not be committed
├── connect.py               # Example Python script to query a database
├── init_db.sql              # Example SQL script for schema creation in SQLite
├── README.md                # Project instructions (this file)
└── requirements.txt         # Python package requirements
```

You also have `create_database.sql`, `explorer.ipynb` and `explorer.py` files. These are model answers to the project requirements, demonstrating how to create a database and explore it using Python and Jupyter Notebook.

---

## 📄 Next Steps

* Replace `init_db.sql` to reflect your custom schema.
* Build your data ingestion pipeline in a new script (e.g. `pipeline.py`).
* Document your changes and logic clearly in the documentation.
* Coordinate with your instructor as the SME to validate requirements and plan future enhancements.

---

## 🧠 Remember

This setup uses **SQLite** for simplicity and local prototyping, but the same schema and logic should be portable to PostgreSQL or another RDBMS in a production environment. Keep modularity and maintainability in mind.

Happy coding!