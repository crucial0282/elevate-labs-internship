# Firewall Configuration and Testing

## Overview
This report details the steps taken to configure and test the firewall on a Linux system using UFW (Uncomplicated Firewall). The goal was to manage inbound traffic by blocking unwanted ports (specifically Telnet on port 23) and allowing essential services (such as SSH on port 22). Logging was enabled to monitor firewall activity.
### 1. Checking Firewall Status
Initially, the firewall status was checked using:

    sudo ufw status verbose

Result: Firewall was inactive.


### 2. Enabling UFW
The firewall was enabled to start filtering traffic:

    sudo ufw enable

### 3. Adding Firewall Rules
Block Inbound Traffic on Port 23 (Telnet)
To enhance security by blocking the vulnerable Telnet service, the following rule was added:

    sudo ufw deny 23

This blocks all inbound connections to port 23.


Allow SSH (Port 22)
Since remote management via SSH is often necessary, the firewall was configured to allow inbound SSH connections:

    sudo ufw allow 22

### 4. Verifying Firewall Rules
The current active firewall rules were verified with:

    sudo ufw status numbered

The output confirmed:

    Port 23 is denied.

    Port 22 is allowed.

### 5. Testing the Rules
An attempt was made to connect to port 23 locally/remotely to verify the block:

    Telnet connection attempts to port 23 failed, confirming the rule is effective.

    SSH connections on port 22 worked as expected.
