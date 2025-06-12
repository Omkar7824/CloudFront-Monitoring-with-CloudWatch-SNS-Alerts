#  CloudFront Monitoring with CloudWatch & SNS Alerts

This project demonstrates how to monitor an AWS CloudFront distribution using Amazon CloudWatch and receive alerts via Amazon SNS (Simple Notification Service).

---

## 🛠️ Tools & Services Used
- **Amazon CloudFront**
- **Amazon CloudWatch**
- **Amazon SNS**
- **AWS Console**

---

## 📊 What This Setup Monitors

- ✅ `4xxErrorRate`: Tracks client-side errors (e.g., 404).
- ✅ `5xxErrorRate`: Tracks server-side errors (e.g., 502/503).
- ✅ SNS Alerts for critical error thresholds.
- ✅ Custom CloudWatch Dashboard.

---

## 📸 Screenshots

> Located in the `Screenshorts` folder.

- 📌 CloudWatch Metrics Graph
- 📌 Alarm Setup
- 📌 SNS Email Subscription Confirmation
- 📌 Real-time Alerts in Inbox

---

## 🚀 Steps to Reproduce

1. **Create a CloudFront Distribution** (or use an existing one).
2. Go to **CloudWatch > Metrics > CloudFront > Per-Distribution Metrics**.
3. Add `4xxErrorRate` and `5xxErrorRate` to the graph.
4. Create alarms:
   - For example, if `5xxErrorRate > 1` for 2 evaluation periods, trigger alarm.
5. Create an **SNS Topic** and subscribe your email.
6. Link the alarm to the SNS topic.
7. Confirm the email subscription to start receiving alerts.

---

## 📬 Alert Example

- You’ll receive an email.
- Alarm Name: CloudFront-High-5xx.
- State: ALARM.
- Description: 5xx error rate exceeded 1% in last 10 minutes.

---

## 💡 Use Case

Perfect for:
- Cloud Engineers
- DevOps Monitoring Setups
- Real-time Performance Alerts
- Disaster Response & Health Checks

---

## 🧑‍💻 Author

**Omkar Rawool**  
Cloud Engineering Enthusiast | AWS Projects  
📫 [Connect on LinkedIn](https://www.linkedin.com/in/omkar-cloud-engineer)

