# ExamForge 🚀

**ExamForge** is a modern, responsive, and lightweight Single-Page Application (SPA) designed for conducting online tests and assessments. Built with a stunning dark-mode UI, it features real-time cloud synchronization using the JSONBin.io REST API, removing the need for a traditional backend server.

Developed by **Azhar Khan** (Acropolis Institute of Technology and Research, Indore).

---

## ✨ Features

### 🎓 For Students
- **Dynamic Test Taking**: Beautiful, interactive UI with seamless question navigation.
- **Real-Time Timer**: Visual progress bar and countdown timer that automatically submits the test when time is up.
- **Anti-Cheat System**: Enforces fullscreen mode. Exiting fullscreen multiple times triggers an automatic submission flagged with a violation.
- **Instant Grading**: Immediate, detailed breakdown of correct, wrong, and skipped questions upon submission.
- **Data Export**: Options to copy results to the clipboard, save as PDF, or share via Email.

### 🛡️ For Administrators (Teachers)
- **Secure Dashboard**: Protected admin area for managing tests and viewing results.
- **Cloud Sync**: Tests uploaded as JSON instantly sync to all student devices via the cloud.
- **Results Tracking**: View real-time student scores, completion times, and submission reasons directly from the dashboard.
- **Easy Uploads**: Bulk upload test question banks via simple JSON files.

---

## 🛠️ Technologies Used

- **Frontend**: Vanilla HTML5, CSS3, and JavaScript (No heavy frameworks).
- **Backend / Database**: [JSONBin.io](https://jsonbin.io/) REST API for cloud storage (Serverless architecture).
- **Icons**: FontAwesome 6.
- **Fonts**: Google Fonts (Inter, Outfit).

---

## 🚀 How to Run Locally

Because ExamForge is entirely serverless, running it is incredibly simple:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/azharkhan924/ExamForge.git
   ```
2. **Open the file:**
   Simply double-click `index.html` to open it in any modern web browser. No local server, Node.js, or database setup is required!

---

## ☁️ Cloud Architecture & Deployment

ExamForge uses Bin IDs to ensure a seamless experience for both students and teachers across different devices. 

- **Tests Bin**: Stores the JSON array of available tests.
- **Results Bin**: Stores the submitted scores of all students.

## 📄 JSON Question Bank Format

To add tests via the Admin Dashboard, use the following JSON structure:

```json
[
  {
    "id": "sample_test_1",
    "title": "Computer Science - Data Structures",
    "duration": 1800,
    "questions": [
      {
        "question": "Which data structure uses LIFO?",
        "options": ["Queue", "Stack", "Tree", "Graph"],
        "correct": 1
      }
    ]
  }
]
```
*(Note: Duration is in seconds. The `correct` field is the 0-indexed correct option).*

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page on GitHub.

## 📜 License

This project is open-source and available under the MIT License.
