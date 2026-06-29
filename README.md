# CyberFace Guard - Desktop AI Security Attendance System

CyberFace Guard ek **desktop-based cybersecurity style face identification and attendance system** hai jo:

- login screen provide karta hai
- person add / update / delete karne deta hai
- manual information entry allow karta hai
- face image save karta hai
- live camera se face capture kar sakta hai
- photo se recognition kar sakta hai
- match hone par full information show karta hai
- mismatch hone par unknown batata hai
- attendance logs store karta hai
- dark cyber UI provide karta hai

## Features

1. Secure desktop login
2. Person management dashboard
3. Face embedding generation
4. Live webcam recognition
5. Photo-based recognition
6. Match / mismatch intelligence output
7. Attendance logging
8. SQLite local database
9. PySide6 professional desktop UI
10. VS Code friendly structure

## Tech Stack

- Python 3.14
- PySide6
- OpenCV Contrib
- SQLAlchemy
- SQLite
- bcrypt

## Folder Structure

```text
cyber_face_guard/
│   main.py
│   requirements.txt
│   README.md
│
├── app/
│   ├── bootstrap.py
│   ├── core/
│   │   ├── config.py
│   │   ├── database.py
│   │   └── models.py
│   ├── services/
│   │   ├── auth_service.py
│   │   ├── person_service.py
│   │   ├── attendance_service.py
│   │   └── face_engine.py
│   └── ui/
│       ├── login_window.py
│       ├── main_window.py
│       └── styles.py
├── data/
└── models/
```

## Step-by-Step Setup in VS Code

### 1) Project download / extract
- ZIP extract karein
- VS Code me folder open karein

### 2) Python 3.14 virtual environment banayein

### Windows PowerShell
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows CMD
```cmd
python -m venv .venv
.venv\Scripts\activate.bat
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## 3) App run karein
```bash
python main.py
```

## 4) Default login
- Username: `admin`
- Password: `Admin@123`

## 5) Person add karne ka process
1. People Management tab kholein
2. Employee code, name, address, role, department, joined date bharein
3. Face image select karein
4. Save button dabayein
5. Face embedding automatically generate hogi

## 6) Live camera recognition
1. AI Recognition tab kholein
2. Start Live Camera Recognition button dabayein
3. App camera se frame capture karega
4. Match hua to person info show hogi
5. Mismatch hua to unknown alert aur log create hoga

## 7) Photo recognition
1. AI Recognition tab kholein
2. Recognize from Photo button dabayein
3. Kisi person ki photo select karein
4. App result show karega

## 8) Delete person
- table me person select karein
- Delete Selected Person button dabayein

## Notes for Industry Upgrade
Ye bundle functional starter hai. Pure production deployment ke liye aap in improvements ko next phase me add kar sakte hain:

- role-based multi-user admin accounts
- audit trail export
- encrypted database fields
- liveness detection
- anti-spoofing
- camera stream thread optimization
- RTSP/IP camera support
- report export to PDF/Excel
- Docker / MSI packaging
- password reset flow
- event screenshots retention policy
- SOC monitoring panel

## Important
- First run me app OpenCV Zoo ke face models automatically download karega.
- Internet required ho sakta hai first launch ke time model download ke liye.
- Camera permission allow karna hoga.
- Better accuracy ke liye front-face, clear lighting wali employee image use karein.