JATA Scholar Portal

A Student Monitoring and Workforce Development Dashboard

Overview

JATA Scholar Portal is a lightweight, frontend-driven web application developed to support the Jigawa Agricultural Commercialization Workforce Scholarship Programme.

The portal enables the Jigawa Agricultural Transformation Agency (JATA) to:

Maintain a structured digital record of scholarship beneficiaries

Monitor academic progress and performance over time

Visualize programme statistics through dashboards and charts

Provide a scalable foundation for future backend integration

The system is intentionally designed to be simple, fast, and easy to deploy, using static files and JSON as a data source.

Key Features
1. Landing Page

Programme overview and objectives

Clear navigation to Dashboard, About, and Contact pages

Institutional branding aligned with JATA standards

2. Student Dashboard

Dynamic student listing populated from a JSON dataset

Search, filter, sort, and pagination controls

Performance indicators (GPA, attendance, research progress)

Interactive charts for:

Course distribution

Performance overview

3. Student Profile Modal

Full student biodata

Academic background and preferences

Current study details (university, degree level, course)

Performance metrics and notes

Linked student photograph

4. Responsive and Accessible Design

Built with Bootstrap 5

Fully responsive across desktop, tablet, and mobile

Accessible navigation and readable layout

Technology Stack
Layer	Technology
Frontend	HTML5, Bootstrap 5
Styling	Custom CSS
Icons	Bootstrap Icons
Animations	AOS (Animate on Scroll)
Charts	Chart.js
Data	JSON (static data source)
Hosting	GitHub Pages, Local Server, or any static host

No backend or database is required at this stage.

Project Structure
jigawa-scholarship-portal/
│
├── index.html              # Landing page
├── dashboard.html          # Student dashboard
├── about.html              # About the programme
├── contact.html            # Contact page
│
├── css/
│   └── style.css           # Global styles
│
├── js/
│   └── app.js              # (Optional) shared JS logic
│
├── data/
│   └── students.JSON       # Student dataset
│
├── images/
│   ├── logos/              # JATA logos
│   ├── students/           # Student photographs
│   └── placeholders/       # Fallback images
│
└── README.md               # Project documentation

Student Data Format (JSON)

Each student record follows a consistent structure to ensure compatibility with the dashboard:

{
  "sNo": "1",
  "employeeId": "JAGRO-2023010011",
  "fullName": "Hussaini Hashim",
  "photo": "images/students/JAGRO-2023010011",
  "gender": "Male",
  "dob": "1/1/94",
  "age": "31",
  "maritalStatus": "Married",
  "lga": "Auyo",
  "ward": "Kafur",
  "email": "example@email.com",
  "phone": "08000000000",
  "qualification": "B.Sc. Ed.",
  "areaStudy": "Agricultural Science",
  "yearGraduated": "2018",
  "preferredDegree": "Masters",
  "preferredCourse": "Agronomy and Crop Science",
  "course": "",
  "degreeLevel": "",
  "university": "",
  "gpa": "",
  "attendance": "",
  "research": "",
  "performance": "",
  "notes": ""
}

Student Photograph Rules

Store photos inside:
images/students/

Naming convention:

employeeId.jpg
employeeId.png


Example:

images/students/JAGRO-2023010011.jpg


The photo field in JSON should point to the image path without extension, allowing flexibility.