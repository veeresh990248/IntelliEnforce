🚔 IntelliEnforce – Smart Traffic Enforcement System

An intelligent, data-driven traffic enforcement system built using Django that automates vehicle verification, fine calculation, and officer monitoring with anomaly detection.

🚨 Problem

Traditional traffic enforcement systems face serious issues:

Manual fine calculation → error-prone
Lack of transparency → corruption risk
No real-time monitoring → inefficiency
No behavioral analysis → no accountability
Example 1

Officer manually issues fines → inconsistent amounts → no audit trail.

Example 2

Repeated suspicious fines by same officer → no system to detect pattern.

💡 Solution

IntelliEnforce digitizes and automates the entire process:

Automated vehicle verification
Rule-based fine calculation
Centralized violation tracking
Officer performance monitoring
Anomaly detection for suspicious activity
⚙️ Core Features
🚗 Vehicle Verification
Enter vehicle number
Fetch and validate details
Check compliance

Example:

KA25MA1234 → Valid → No fine
KA09XX9999 → Expired documents → Fine generated

💰 Automatic Fine Calculation
Based on rule violations
Eliminates manual errors

Example:

No helmet → ₹500
Expired insurance → ₹1000
👮 Officer Dashboard
Total cases handled
Total fine collected
Recent violations list

Example:

Officer A → 20 cases → ₹10,000
Officer B → 5 cases → ₹2,000

📊 Violation Tracking
Stores all violations in database
Tracks vehicle + officer + time
⚠️ Anomaly Detection (Key Feature)

Detects suspicious enforcement behavior.

Example 1:
Officer suddenly issues 50 fines in 1 hour → flagged 🚨

Example 2:
Unusually high fines compared to others → flagged 🚨

🧠 Anomaly Detection Logic

(Current version uses statistical approach)

Calculates average fine behavior
Detects deviations beyond threshold
Flags abnormal activity

Future upgrade → ML-based prediction

🔄 System Workflow
User logs in
Officer enters vehicle number
System verifies vehicle details
Fine is calculated automatically
Violation is stored in database
Dashboard updates in real-time
Anomaly detection runs in background
🛠 Tech Stack
Backend: Django (Python)
Frontend: HTML, CSS📸 Screenshots
🔐 Login Page

📊 Dashboard

🚗 Vehicle Check

⚠️ Anomaly Detection

Database: SQLite
Authentication: Django Auth
Logic Layer: Custom Python services

