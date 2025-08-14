# ATM Security Monitoring Platform - Code Description
This is a client-side web application built with HTML, CSS, and JavaScript that allows financial institutions to monitor ATM security incidents. It provides role-based access control, data analysis, and reporting features.

##🔹 Key Features
### 1. Authentication & Role-Based Access
Two user roles:

Admin (CEO): Full access (upload data, view analytics, generate reports)

Analyst: Read-only access (dashboard & analytics only)

Session management (auto-logout after inactivity)

Hardcoded credentials (for demo purposes):

Admin: admin / admin123

Analyst: analyst / analyst123

### 2. Data Upload & Processing
CSV file upload (drag-and-drop or file browser)

Real-time validation (checks for required columns)

Data preview before processing

Stores data in browser memory (sessionStorage)

### 3. Dashboard & Analytics
Key Metrics:

Total losses

Incident count

Average loss per incident

Security risk level

Top Risk Indicators:

Highest-risk crew members

Most vulnerable machines

Riskiest districts

Trend Visualization (Chart.js)

### 4. Reporting
CSV Export (download transaction data)

PDF Reports (Executive Summary & Detailed Report)

Preview before download (demo version)

#🔹 Technical Implementation
### 📌 Frontend
Pure HTML/CSS/JS (no frameworks)

Responsive design (works on desktop & tablet)

Libraries Used:

PapaParse (CSV parsing)

Chart.js (data visualization)

jsPDF + html2canvas (PDF generation)

### 📌 Data Storage
Client-side only (no backend)

Uses sessionStorage (clears when browser closes)

No database required

### 📌 Security & IP Protection
All processing happens in the browser

No server-side code (protects intellectual property)

Confidential data is not stored permanently

#🔹 How It Works
User logs in (Admin or Analyst)

Admin uploads CSV data (ATM transaction records)

System processes & analyzes data:

Calculates total losses

Identifies high-risk incidents

Generates trends

User views dashboard & analytics

Generates reports (CSV/PDF)

#🔹 Limitations (MVP)
No permanent data storage (clears on refresh)

Demo credentials only (no real authentication)

Basic risk calculation (simple formula)

PDF export is a preview (full export requires backend)

#🔹 Future Enhancements
✅ Add a real backend (Node.js, Firebase, or AWS)
✅ Database integration (PostgreSQL, MongoDB)
✅ Advanced risk-scoring algorithms
✅ Email/SMS alerts for high-risk incidents
✅ Multi-user collaboration

# 🚀 Ready to Deploy
This is a fully functional MVP that can be hosted on:

GitHub Pages

Netlify

Vercel

Any static web hosting
