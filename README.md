# Hospital Management System

Full-stack hospital automation platform built for a real healthcare client, handling appointment booking, patient records, prescriptions, pharmacy inventory, blood donation management, and AI-assisted clinical support.

## ✨ Features

- **Role-based access control** across 4+ user types — patients, doctors, admins, pharmacists — each with a dedicated, secure portal
- **Appointment booking** with real-time doctor availability
- **Patient record management** — structured workflows for patient data handling and contextual medical query support
- **Prescription tracking & pharmacy inventory** control
- **Blood donation management** module
- **AI-powered chatbot** for patient-facing queries ([see companion repo](https://github.com/Kiran301103/chatbot))
- **ML-based disease prediction** — heart disease, Parkinson's, and diabetes risk models ([see companion repo](https://github.com/Kiran301103/multiple_disease_prediction))
- Automation for appointment/service workflows, cutting admin processing time by ~40%

## 🛠️ Tech Stack

`HTML` · `CSS` · `PHP` · `JavaScript` · `Python` · `SQL` · AI/ML techniques for predictive modules

## Prerequisites
- PHP 7.4+ with the mysqli extension
- MySQL or MariaDB
- Composer (for PHPMailer, already vendored — only needed if you want to update dependencies)
- A local server stack: XAMPP/WAMP/MAMP, or PHP's built-in server
- Python 3.9+ and pip (only for the /chatbot module)
  
## 🏗️ Architecture

The system is organized into role-specific portals sitting on a shared PHP/MySQL backend, with Python-based ML services handling prediction and chatbot inference, integrated via API calls from the PHP layer.

## 🚀 Getting Started

```bash
git clone https://github.com/Kiran301103/hms.git
cd hms
# Import the SQL schema into your MySQL instance
# Configure DB credentials in config file
# Serve via PHP (e.g. XAMPP/WAMP or php -S localhost:8000)
```
BDMS/ and pharm/ are separate mini-apps with their own database and entry point — see the setup guide for exact database names, since the module READMEs and the actual PHP connection code don't fully agree (documented in docs/DATABASE_SCHEMA.md).

## 📌 Impact

Reduced admin processing time by ~40% while supporting secure, role-based access across the full patient care lifecycle.

## License

This project is licensed under the Apache License 2.0.

See the [LICENSE](./LICENSE) file for full details.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.

© 2026 Kiran M, Manoj Kumar K
