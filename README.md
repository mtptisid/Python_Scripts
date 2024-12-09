#  **NMON ANALYSER FOR LINUX MACHINE WITH PYTHON**


This project automates the process of collecting, analyzing, and reporting system performance data from remote servers using NMON files. The tool performs the following tasks:

- Connects to remote hosts via SSH to fetch NMON files for specified dates.
- Analyzes the data to generate insights and plots for key system metrics.
- Creates a detailed report in `.docx` format for each host and date combination.
- Sends email notifications with the generated reports as attachments.

---

## Table of Contents

1. [Features](#features)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Configuration](#configuration)
6. [Output](#output)
7. [Email Integration](#email-integration)
8. [License](#license)

---

## Features

- Fetch NMON files for specific hosts and dates via SSH.
- Analyze system performance metrics, including:
  - CPU Usage
  - Memory Usage
  - Network I/O
  - Disk I/O and File Systems
- Generate detailed `.docx` reports with visual graphs.
- Automatically email generated reports for all hosts.

---

## Prerequisites

Ensure the following tools and libraries are installed:

1. **Python 3.6+**
2. **Required Python Libraries**: 
   - `paramiko`
   - `matplotlib`
   - `pandas`
   - `docx` (via `python-docx`)
   - `argparse`
3. **Sendmail Service** for SMTP configuration (no authentication required).

Ensure the Sendmail service is properly configured on your system.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/mtptisid/NMON_Analyser_with_Python.git
   cd NMON_Analyser_with_Python
    ```
2.	Install required Python libraries:
    ```
    pip install -r requirements.txt
    ```

## Usage

Run the script with the required arguments for hosts and dates. The script supports analyzing multiple hosts and dates by iterating through the inputs.

## Command
  ```
  python nmon_analysis.py --host <host1,host2,...> --date <date1,date2,...>
  ```

## Example
  ```
  python nmon_analysis.py --host my_host_001,my_host_002 --date 2024-11-21,2024-11-22
  ```


## Snapshots
![image](https://github.com/user-attachments/assets/1fcf31d6-b6a7-4e41-aa7b-b6a71c9c9677)

![image](https://github.com/user-attachments/assets/0fd92fdd-61b2-4094-826f-a0885c8c8bac)

![image](https://github.com/user-attachments/assets/29db0e50-3e1d-4ea2-8289-41edb92abb61)

![image](https://github.com/user-attachments/assets/865f966e-add2-4efb-838a-e23f07e7b424)

![image](https://github.com/user-attachments/assets/8659c9ef-569b-40dc-9f81-f64fe4aa2718)

![image](https://github.com/user-attachments/assets/ab12d46c-f7f0-4580-a8cd-b53208fa3400)






