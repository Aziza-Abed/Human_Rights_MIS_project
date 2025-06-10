# Human Rights Monitor MIS

A web-based Management Information System (MIS) built with FastAPI, MongoDB, and Streamlit. It helps document, manage, and analyze human rights violations with tools for reporting, case tracking, and data visualization.

---

## Features

- Incident reporting for public users, NGOs, and legal teams
- Case management with evidence uploads and status tracking
- Analytics dashboard showing violation trends, timelines, and maps
- Interactive maps to visualize incident locations
- Role-based access system for different user types
- Export options for downloading reports and cases as CSV or PDF

---

## Technologies Used

Backend: FastAPI (Python)  
Frontend: Streamlit  
Database: MongoDB Atlas  
Visualization: Plotly and Folium  
Export: FPDF, CSV, base64 encoding

---

## How to Set Up

1. Clone the repository

```
git clone https://github.com/your-username/human-rights-mis.git
cd human-rights-mis
```

2. Create and activate a virtual environment

```
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

3. Install dependencies

```
pip install -r requirements.txt
```

4. Set your MongoDB URI in the `db.py` file

5. Run the system

```
python run_all.py
```

The backend will run on http://localhost:8000  
The frontend will run on http://localhost:8501

---

## MongoDB Collections

- cases  
- case_status_history  
- incident_reports  
- report_evidence

---

## Access Roles

Public users can submit incident reports  
NGO Workers can submit and view reports  
Lawyers can view and submit both reports and cases (access code: LEGAL123)  
Admins have full access to all system features (access code: ADMIN123)

---

## Export Options

Reports and cases can be exported in CSV and PDF formats from the following locations:
- Incident Reporting → View Reports
- Case Management → View Cases
