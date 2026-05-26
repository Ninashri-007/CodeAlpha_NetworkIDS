# CodeAlpha_NetworkIDS
# Network Intrusion Detection System (NIDS)

## Project Overview
This project demonstrates a simple Network Intrusion Detection System (NIDS) using Suricata and Wireshark on Kali Linux.

The IDS monitors network traffic and generates alerts for suspicious activities such as:
- ICMP Ping Detection
- HTTP Traffic Detection
- TCP SYN Scan Detection
- SSH Connection Attempts
- DNS Traffic Monitoring

## Tools Used
- Kali Linux
- Suricata
- Wireshark
- Nmap
- Curl

## Features
- Real-time packet monitoring
- Custom Suricata rules
- Alert generation and logging
- Traffic analysis using Wireshark

## Project Structure
- `custom.rules` → Custom Suricata detection rules
- `logs/` → Sample generated alerts
- `screenshots/` → Project screenshots

## Commands Used

### Start Suricata
```bash
sudo suricata -c /etc/suricata/suricata.yaml -i eth0
```

### Generate Traffic
```bash
ping google.com
curl http://example.com
nmap localhost
```

### View Alerts
```bash
sudo tail -f /var/log/suricata/fast.log
```

## Output
The IDS successfully detected:
- Ping traffic
- HTTP traffic
- SYN scans

##Author
Nina Sree Adari

## Author
NinaSree Adaru
