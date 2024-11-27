# README: Automated Mango Call Center in Mali

This project demonstrates how to build an automated call center system for collecting and processing data about mango production in Mali. The system addresses challenges such as language translation, fraud detection, emergency call routing, and misdirected calls.

---

## Features

### 1. **Language Translation**
- **Input Language:** Bambara (spoken by most farmers in Mali).
- **Intermediate Translation:** French (for system compatibility).
- **Output Language:** English (for non-French-speaking stakeholders like the boss).
- Utilizes a two-step translation process:
  - Bambara → French → English.

### 2. **Fraud Detection**
- Identifies suspicious reports of mango yield and price:
  - Normal yield range: **5 - 15 tons.**
  - Reasonable price range: **$10 - $100 per ton.**
- Flags data exceeding expected ranges to detect potential underreporting or overreporting.

### 3. **Emergency Call Handling**
- Detects phrases indicating emergencies (e.g., infant health-related calls).
- Redirects such calls to appropriate services to ensure safety.

### 4. **Misdirected Calls**
- Detects calls meant for "Mango Mali," a music production company.
- Provides polite redirection for music-related queries.

### 5. **Data Collection**
- Captures and stores relevant data in a CSV file:
  - Caller phone number.
  - Translated input in English.
  - Fraud detection status.

---

## Installation

### Prerequisites
- **Python 3.6+**
- Required libraries:
  - `deep-translator`
  - `csv`
  - `re`
  - `string`

### Setup
1. Clone or download the project repository.
2. Install required Python libraries:
   ```bash
   pip install deep-translator
