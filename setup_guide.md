# Setup Guide

## Step 1: Update System
```bash
sudo apt update && sudo apt upgrade -y
```

## Step 2: Install Required Tools
```bash
sudo apt install suricata wireshark nmap curl net-tools -y
```

## Step 3: Create Custom Rules
```bash
sudo nano /etc/suricata/rules/custom.rules
```

## Step 4: Configure Suricata
Edit:
```bash
sudo nano /etc/suricata/suricata.yaml
```

Add:
```yaml
rule-files:
  - custom.rules
```

## Step 5: Start Suricata
```bash
sudo suricata -c /etc/suricata/suricata.yaml -i eth0
```

## Step 6: Generate Traffic
```bash
ping google.com
curl http://example.com
nmap localhost
```

## Step 7: View Alerts
```bash
sudo tail -f /var/log/suricata/fast.log
```
