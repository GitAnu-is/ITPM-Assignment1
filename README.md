# IT3040 ITPM – Assignment 1 (Option 1)

## Singlish to Sinhala Transliteration Testing

This project contains automated test scripts to evaluate the accuracy of the **Chat Sinhala Transliteration** system available at:
https://www.pixelssuite.com/chat-translator

The focus is on identifying **incorrect transliterations (negative test cases)** using automation.

---

## ⚙️ Installation

Install required dependencies:

```bash
pip install -U pip
pip install playwright openpyxl
```

Install Playwright browser:

```bash
python -m playwright install chromium
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

### Covered Singlish Input Types:

* Question forms
* Commands
* Greetings
* Romanization variations
* English word insertions
* Emojis
* Numbers, dates, and time formats
* Mixed language inputs

---

## 📊 Results

The automation script performs the following:

* Inputs Singlish sentences
* Captures Sinhala transliteration output
* Compares with expected output
* Updates Excel file automatically

### Output Columns:

* **Actual Output** → System generated output
* **Status** → PASS / FAIL

---

## ⚠️ Important Notes

* Ensure the Excel file is **closed** before running the script
* Browser will open automatically during execution
* Results are saved after each test case
* The **browsers folder is excluded** from submission to reduce file size

---

## 📁 Submission Includes

* Playwright automation project
* Excel file with test cases and results
* README.md file
* GitHub repository (public access)

---

## 👨‍💻 Author

Registration Number: **IT23244320**

---

## 🔗 GitHub Repository

https://github.com/GitAnu-is/ITPM-Assignment1

---
