#  Intrusion Detection Report (Simulated)

##  Summary
This report analyzes simulated web server logs using Splunk-like search techniques to identify intrusion patterns.

##  Key Observations
- IP `192.168.1.23` made 3 consecutive failed login attempts in 7 seconds.
- Unauthorized access attempt to `/admin` detected from IP `192.168.1.85`.
- IP `203.0.113.5` accessed the homepage with no suspicious behavior.

##  Potential Threats
- Brute-force login behavior from IP `192.168.1.23`
- Possible admin panel probing from `192.168.1.85`

##  Actions (Simulated)
- Alert configured to trigger if more than 5 failed logins from a single IP in 5 minutes.
- Malicious IPs would be blocklisted using a firewall or IDS.

##  Lessons Learned
Even basic logs can uncover potential threats. Tools like Splunk enhance this process with powerful search and alerting.
