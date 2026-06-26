# Smart Lender - Project Summary

This document provides a comprehensive overview of the **Smart Lender – Loan Eligibility Prediction System** project. It integrates the database design, project workflow phases, and technology stack.

---

## 🏗️ Project Architecture & Components

The system consists of several integrated components that process loan application data and predict loan eligibility.
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/07d0944d-cbe4-4af1-aa78-7e063f7fbf12" />

```mermaid
graph TD
    A[Loan Eligibility Dataset] --> B[Data Preprocessing]
    B --> C[Machine Learning Models]
    C --> D[Flask Web Application]
    D --> E[Prediction Results & Status]
```

### Key Subsystems

1. **Data Ingestion & Preprocessing**: Handles dataset collection, cleansing (missing values via mean/mode imputation), and scaling.
2. **Machine Learning Model Registry**: Compares models (Decision Tree, Random Forest, KNN, XGBoost) and exports the best-performing model.
3. **Flask Web Application API**: Provides a web-based prediction form for credit officers or applicants.

---

## 🗄️ Database Design (Entity-Relationship)

The system manages user profiles, credit history, loan applications, and ML predictions using the database structure visualized below.

### ER Diagram

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/49acb1b9-7c07-4366-a606-9969f07fc5b0" />


### Key Entities
* **USER**: System users (applicants or credit officers).
* **APPLICANT_PROFILE**: Personal details of applicants.
* **CREDIT_HISTORY**: Credit history and score records.
* **LOAN_APPLICATION**: Details of the submitted loan applications.
* **MODEL**: Information on the trained machine learning models.
* **PREDICTION_RESULT**: Model predictions matched to loan applications.

---

## 🔄 Machine Learning Workflow

The project is executed in five major epics following the standard Machine Learning lifecycle:

```mermaid
gantt
    title Project Workflow Timeline
    dateFormat  YYYY-MM-DD
    section Epic 1
    Data Collection & Arch Design :active, 2026-06-20, 3d
    section Epic 2
    EDA & Visualization           :active, 2026-06-23, 4d
    section Epic 3
    Data Preprocessing            :active, 2026-06-27, 3d
    section Epic 4
    Model Building & Evaluation   : 2026-06-30, 4d
    section Epic 5
    Flask App Integration         : 2026-07-04, 3d
```

### Workflow Diagram

![Smart Lender Project Workflow](C:/Users/ADMIN/.gemini/antigravity/brain/6bfe2cbb-178f-418e-8f7f-8bb132be1a93/images/Workflow_Diagram.png)

---

## 🛠️ Technology Stack

Below is the list of tools and libraries used in this project:

| Technology | Purpose | Documentation / Link |
| :--- | :--- | :--- |
| **Anaconda Navigator** | Environment & Package Management | [anaconda.com](https://www.anaconda.com/download) |
| **PyCharm** | Python Integrated Development Environment (IDE) | [jetbrains.com](https://www.jetbrains.com/pycharm/) |
| **NumPy** | Numerical Operations & Multidimensional Arrays | [numpy.org](https://numpy.org/doc/stable/) |
| **Pandas** | Data Processing & Table Manipulations | [pandas.pydata.org](https://pandas.pydata.org/docs/) |
| **Scikit-learn** | Machine Learning Training & Evaluation | [scikit-learn.org](https://scikit-learn.org/stable/) |
| **Matplotlib** | Core Visualization & Graph Plotting | [matplotlib.org](https://matplotlib.org/stable/) |
| **Seaborn** | Advanced Statistical Data Visualizations | [seaborn.pydata.org](https://seaborn.pydata.org/) |
| **Flask** | Lightweight Web Application Server | [flask.palletsprojects.com](https://flask.palletsprojects.com/) |

---

## 📂 Source Files

You can inspect the original source files in the project workspace:
- [software_and_tools.md](file:///C:/Users/ADMIN/.gemini/antigravity/scratch/smart-lender-erd/software_and_tools.md)
- [project_links.md](file:///C:/Users/ADMIN/.gemini/antigravity/scratch/smart-lender-erd/project_links.md)
- [project_workflow.md](file:///C:/Users/ADMIN/.gemini/antigravity/scratch/smart-lender-erd/project_workflow.md)
- [README.md](file:///C:/Users/ADMIN/.gemini/antigravity/scratch/smart-lender-erd/README.md)
