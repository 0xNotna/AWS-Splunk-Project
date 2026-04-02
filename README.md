#  🧾 AWS Splunk & Alert automation Project


## 🎯 Objective 
To build and operate an AWS-hosted Splunk SOC lab that detects brute-force activity against a Linux EC2 instance and automates alert delivery through n8n and Slack. The project demonstrates cloud-based log monitoring, alert engineering, workflow automation, investigation, and incident reporting.

## 📊 What's Inside
- AWS-hosted Splunk deployment
- Linux authentication log ingestion into Splunk
- Brute force detection using SPL
- Tines alert automation and enrichment workflow
- Slack alert delivery
- Dashboard configurations for security monitoring
- Screenshots of SPL queries, Splunk alerts, AWS configurations, and workflow execution
- Incident Report
- Lessons learned
  
---------

## 🏗️ Architecture 
#### AWS/SPLUNK/TINES WORKFLOW
<img width="1498" height="886" alt="image" src="https://github.com/user-attachments/assets/22e8fc4e-e0ee-4676-9103-b1d52e594e69" />



### ♨️ Key Components

- EC2 Ubuntu victim machine: target host used to generate SSH brute-force telemetry.
- Splunk Forwarder: forwards /var/log/auth.log events from the EC2 instance to Splunk.
- Splunk Enterprise: ingests logs, runs detections, and triggers alerts.
- Tines: receives Splunk webhook alerts enriches and formats Slack notifications.
- Slack: receives the final alert for analyst visibility.
- Kali attacker workstation: generates controlled failed SSH attempts for the lab.

---------


## 🛠️ Technical Skills Demonstrated
- AWS EC2, IAM, Security Groups, and VPC fundamentals
- Splunk deployment and administration
- Brute-force detection using SPL
- Alert automation with Tines webhooks
- Slack-based security notification workflow
- Dashboard creation and log analysis
- Incident investigation and report
