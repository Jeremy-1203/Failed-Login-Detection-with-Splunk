# Failed Login Detection with Splunk

## Overview

This project demonstrates how to detect and investigate failed Windows login attempts using Splunk Enterprise. A Windows 11 virtual machine was deployed in VirtualBox, Windows Security Logs were collected, and failed authentication events were identified using Splunk.

## Objective

The goal of this project was to:

- Configure a Windows 11 virtual machine
- Install and configure Splunk Enterprise
- Collect Windows Security Event Logs
- Generate failed login attempts
- Detect failed authentication events using Event ID 4625
- Practice basic SIEM investigation techniques

## Lab Environment

- Splunk Enterprise
- Windows 11 Enterprise
- Oracle VirtualBox
- Windows Security Event Logs

## Detection Query

```spl
index=main EventCode=4625
```

## Investigation Steps

1. Created a Windows 11 virtual machine in VirtualBox.
2. Installed Splunk Enterprise.
3. Configured Splunk to ingest Windows Security Event Logs.
4. Attempted multiple logins using an incorrect password.
5. Searched Splunk for Event ID 4625.
6. Reviewed the generated failed authentication events.

## Findings

- Successfully collected Windows Security Logs.
- Generated multiple failed login attempts.
- Detected Event ID 4625 events in Splunk.
- Verified that failed authentication activity was properly logged and searchable.

## Skills Demonstrated

- SIEM Administration
- Security Monitoring
- Log Analysis
- Windows Event Log Collection
- Security Event Investigation
- Splunk Search Processing Language (SPL)
- Virtualization with VirtualBox

## Screenshots

See the screenshots included in this repository:

- Windows Login Screen
- Failed Login Attempt
- Splunk Event ID 4625 Detection Results

## Outcome

This project demonstrates the ability to deploy a SIEM platform, ingest Windows security logs, generate security events, and investigate failed login activity using Splunk Enterprise.
