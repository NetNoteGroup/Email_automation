# Email Automation Tool

A Python-based automated email dispatcher designed to securely broadcast daily updates and reports to multiple recipients. Built specifically for sending scheduled updates to the **TradeTribe** forex trading community.

##  Features

* **Multi-Recipient Support:** Loops through a distribution list to deliver personalized emails seamlessly.
* **Daily Rate Limiting:** Built-in safeguards (`DAILY_LIMIT = 500`) prevent account blocks by tracking daily outbound volume.
* **MIME Configuration:** Structured using `MIMEMultipart` and `MIMEText` for clean text delivery.
* **Scheduling Infrastructure:** Imports `schedule` and `time` dependencies to automate routines.

##  Getting Started

Follow these steps to set up the script on your local machine.

### Prerequisites

Ensure you have Python 3.x installed along with the required libraries. Install dependencies via pip:

```bash
pip install pandas schedule
```

###  Configuration & Running

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   ```

2. **Navigate into the directory:**
   ```bash
   cd Email_automation
   ```

3. **Configure Authentication:**
   Open the script file and ensure your host configuration (such as `smtplib.SMTP` settings and app-specific security passwords) are properly initialized to hook into your email service provider.

4. **Execute the script:**
   ```bash
   python daily_email_report.py
   ```

##  Built With

* **Python 3** - Core application logic.
* **smtplib & email** - Native Python modules for SMTP protocol routing and MIME generation.
* **Pandas** - Data manipulation framework.
* **Schedule** - Job scheduling engine for automation routines.


*Developed for TradeTribe Community Outbound Updates.*
