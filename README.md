# Project-3
# Defensive Security Project

## Contributors
- **Wahid Sherzad**: Worked on Windows Logs Analysis
- **Horya Sediqi**: Worked on Apache Logs Analysis

## Project Overview
This project aims to analyze and enhance the security of Virtual Space Industries (VSI) by monitoring and analyzing various logs to detect suspicious activities and potential threats. We used Splunk to monitor and analyze the logs from both Windows and Apache servers.

## Windows Logs Analysis
**Contributor: Wahid Sherzad**

The Windows logs analysis focused on identifying and mitigating suspicious activities such as failed logins, successful logins, and account deletions. Key findings included:

- **Failed Logins**: Detected 35 failed login events on March 25, 2020, at 8:00 a.m., exceeding the alert threshold.
- **Successful Logins**: Identified 196 successful login events by user_j on March 25, 2020, at 11:00 a.m., surpassing the threshold.
- **Deleted Accounts**: No suspicious volume of deleted accounts was found. Key signatures included "A user account was locked out" and "An attempt was made to reset an account's password."

## Apache Logs Analysis
**Contributor: Horya Sediqi**

The Apache logs analysis aimed to identify abnormal HTTP methods, referrer domains, and response codes. Key findings included:

- **HTTP Methods**: Significant increase in POST methods during the attack period.
- **HTTP Response Codes**: Notable jump in 404 errors from 2% to 15%, indicating potential probing for vulnerabilities.
- **International Activity**: Detected a suspicious volume of HTTP POST activity, peaking at 1,296 events, and unusual international access patterns from cities such as Kiev and Kharkiv.

## Recommendations
To enhance VSI's security posture, we recommend the following mitigations:

1. **Strengthen Server Security**: Implement stronger access controls and robust password policies.
2. **Deploy Intrusion Detection Systems (IDS)**: Monitor and alert on unusual activities.
3. **Regular Security Reviews**: Update security configurations and conduct regular audits.
4. **Security Awareness Training**: Educate employees to prevent social engineering attacks.
5. **Encrypt Sensitive Data**: Protect intellectual property on the Windows Server.
6. **Web Application Firewall (WAF)**: Protect the Apache Server against web-based attacks.
7. **Software Updates**: Ensure all software and servers are updated with the latest patches.
8. **Incident Response Plan**: Develop and maintain a plan to address future incidents.
9. **Continuous Monitoring**: Analyze logs and network traffic for anomalies.
10. **Threshold Fine-Tuning**: Adjust alert thresholds to balance detection and reduce false positives.
11. **Geographic Blocking**: Prevent access from regions with no legitimate business needs.

By implementing these measures, VSI can better protect against potential cyber threats and enhance overall security resilience.
