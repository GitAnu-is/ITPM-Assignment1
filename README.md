# IT3040 ITPM – Assignment 1 

## Singlish to Sinhala Transliteration Testing

This project contains automated test scripts developed to evaluate the accuracy of the **Chat Sinhala Transliteration** feature available at:
https://www.pixelssuite.com/chat-translator

The testing focuses on identifying incorrect transliterations of Singlish inputs into Sinhala using automated testing with Playwright.

---

## 📌 Prerequisites

* Python 3.11 or higher (used: Python 3.13.3)
* Google Chrome (or Playwright Chromium)
* Internet connection

---

## ⚙️ Installation Steps

Run the following commands in terminal:

```bash
pip install -U pip
pip install playwright openpyxl
python -m playwright install chromium
```

---

## 📂 Project Structure

```
ITPM Assignment1
│
├── browsers
│
├── test_automation
│     ├── test_automation.py
│     ├── IT23244320_Assignment 1 - Test cases.xlsx
│
└── README.md
```

---

## ▶️ Running the Automation

Navigate to the automation folder:

```bash
cd "D:\ITPM Assignment1\test_automation"
```

Run the test script:

```bash
python test_automation.py --excel "IT23244320_Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

---

## 🧪 Test Case Details

* Total Test Cases: **50 (Negative test cases)**
* Focus: **Failure scenarios in transliteration**
* Covers multiple Singlish input types such as:

  * Question forms
  * Commands
  * Greetings
  * Romanization variants
  * English word insertions
  * Emojis
  * Numbers, dates, and more

---

## 📊 Results

* The script automatically:

  * Inputs Singlish sentences
  * Captures Sinhala output
  * Compares with expected output
  * Updates Excel file

### Output Columns:

* **Actual Output** → System generated output
* **Status** → PASS / FAIL

---

## ⚠️ Important Notes

* Ensure the Excel file is **closed** before running the script
* Browser will open automatically during execution
* Results are saved after each test case

---

## 📁 Submission Includes

* Playwright automation project
* Excel file with test cases and results
* README.md file
* Git repository (public access)

---

## 👨‍💻 Author

Registration Number: **IT23244320**

---
