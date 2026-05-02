# IT3040_Assignment_IT23662582

## Prerequisites (One-time Setup)

Before getting started, ensure you have the following installed on your system:

- **Python 3.11** or **Python 3.12**
- **Google Chrome** (recommended) or **Playwright Chromium** (Playwright will install it automatically)

## Project Setup

1. Extract the project folder to your desired location (e.g., `D:\` drive)
2. Open a **Command Prompt** or **PowerShell**
3. Navigate to the project directory by running:
   ```
   cd /d D:\test_automation
   ```
   *(Replace `D:\test_automation` with your actual extracted folder path)*

## Install Dependencies (One-time Setup)

From the project directory in Command Prompt/PowerShell, run the following commands:

```bash
pip install -U pip
pip install playwright openpyxl
playwright install
```

This will:
- Upgrade pip to the latest version
- Install Playwright (browser automation framework) and openpyxl (Excel handling library)
- Download and install Chromium browser for Playwright

## Running the Tests

From the project directory in Command Prompt/PowerShell, run:

```bash
python test_automation.py --excel "test_automation/Assignment 1 - Test cases IT23662582.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

### Command Parameters:
- `--excel`: Path to the test cases Excel file
- `--url`: Target website URL to test
- `--wait-ms`: Wait time in milliseconds between actions (5000ms = 5 seconds)
- `--type-delay-ms`: Delay between keystrokes (80ms)
- `--slow-mo-ms`: Slow motion delay (200ms)
- `--save-every`: Save screenshots every N test cases (1 = after each test)
- `--keep-open`: Keep the browser open after tests complete for inspection

## Project Structure

```
IT3040_Assignment_IT23662582/
├── README.md
├── test_automation/
│   ├── test_automation.py
│   └── Assignment 1 - Test cases IT23662582.xlsx
```