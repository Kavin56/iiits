# Hack The Threat - Cybersecurity & AI Hackathon

## Project Overview
This project is built as part of the "Hack The Threat" cybersecurity hackathon, focusing on AI-driven threat detection and security analysis. It consists of two main components:

1. **Demo Website (Testing Environment)**
   - Developed using HTML, CSS, JavaScript, and React.
   - Hosted on Netlify for easy deployment.
   - Used for testing various security vulnerabilities and resilience against cyber threats.

2. **Threat Classification System (Streamlit App)**
   - Built with Streamlit to analyze log files for security threats.
   - Implements Generative AI techniques to classify and visualize threats.
   - Allows users to upload log files for real-time analysis.

## Features
- **Honeypots:** Deceptive systems designed to lure and analyze potential attacks.
- **Threat Classification:** Uses AI to detect and classify security threats in log files.
- **Real-time Monitoring:** Tracks website uptime and potential security breaches.
- **Automated Testing & Analysis:** Utilizes various tools to assess security.

## Security Testing Frameworks Used

### 1. Locust (Load Testing)
- Locust is used to simulate multiple users accessing the website to test for performance and vulnerabilities under heavy traffic.
- **How to Run:**
  ```bash
  pip install locust
  locust -f locust.py --host https://taupe-tanuki-66c44a.netlify.app/
  ```
- **Sample Output:**
  _[Insert Screenshot of Locust Load Test Results]_  

### 2. Loguru (Logging & Monitoring)
- Loguru is used to log website activity, errors, and uptime monitoring.
- **How to Run:**
  ```bash
  python monitor.py
  ```
- **Sample Output:**
  _[Insert Screenshot of Loguru Logs]_  

### 3. Uptime Kuma (Website Monitoring)
- Uptime Kuma is a self-hosted monitoring tool that continuously tracks the availability and response time of the website.
- **How to Run:**
  ```bash
  docker run -d --restart always -p 3001:3001 louislam/uptime-kuma
  ```
- **Sample Output:**
  _[Insert Screenshot of Uptime Kuma Dashboard]_  

### 4. SQLMap (SQL Injection Testing)
- SQLMap automates the detection and exploitation of SQL injection vulnerabilities.
- **How to Run:**
  ```bash
  sqlmap -u "https://taupe-tanuki-66c44a.netlify.app/?id=1" --dbs
  ```
- **Sample Output:**
  _[Insert Screenshot of SQLMap Injection Results]_  

### 5. Pytest (Automated Security Testing)
- Pytest is used for automated functional and security test cases.
- **How to Run:**
  ```bash
  pytest test_security.py
  ```
- **Sample Output:**
  _[Insert Screenshot of Pytest Test Results]_  

## Setup and Deployment
### Prerequisites
- Python 3.8+
- Node.js (for frontend testing)
- Docker (for Uptime Kuma)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/hack-the-threat.git
   cd hack-the-threat
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit Threat Classification App:
   ```bash
   streamlit run app.py
   ```

## Future Enhancements
- Implement more AI models for threat detection.
- Integrate real-time alerts for detected threats.
- Expand honeypot functionalities to log attacker behavior in detail.

## Contributors
- **[Your Name]** - AI & Security Engineering
- **[Team Members]** - Development & Security Analysis

