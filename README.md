Basic Firewall Management – Internship Task
This README documents the process and outcomes of configuring firewall rules to block and allow specific network traffic.
The exercise demonstrates practical skills with Windows Firewall and UFW (Uncomplicated Firewall) on Linux.

Task Objective
Configure, apply, and test rules to block and allow inbound traffic using a system firewall.
Understand how firewall rules filter network traffic and improve system security.

Steps Performed
Opened Firewall Tool

Windows: Open "Windows Defender Firewall" via Control Panel.

Linux: Started a terminal and ensured UFW is installed (sudo apt install ufw).

Listed Current Rules

Windows: Viewed settings in “Inbound Rules”.

Linux: Ran
sudo ufw status

Blocked Inbound Traffic (Port 23 - Telnet)

Windows: Created a new inbound rule to block TCP port 23.

Linux: Used
sudo ufw deny 23

Tested Blocking Rule

Attempted to connect to port 23 via Telnet (local or remote). Connection was blocked.

Allowed SSH (Port 22) on Linux

Ran
sudo ufw allow 22

Removed Test Rule

Windows: Deleted the corresponding inbound rule for port 23.

Linux: Used
sudo ufw delete deny 23

Documented Commands & Steps

Listed all commands and major GUI actions for reference.

Example Linux commands:

text
sudo ufw status
sudo ufw deny 23
sudo ufw allow 22
sudo ufw delete deny 23
How Firewalls Filter Traffic
Firewalls enforce rules that permit or block traffic based on criteria like IP address, port, and protocol.
By controlling inbound/outbound connections, they help prevent unauthorized access, mitigate attacks, and secure network boundaries.
Stateful firewalls track connection state, while stateless firewalls filter each packet independently.

Outcome

Demonstrated basic firewall rule management.
Practiced blocking and unblocking ports.
Improved understanding of network traffic filtering.
Documented process for professional reporting.

Conclusion

Firewall management is essential for protecting systems from unauthorized access.
This hands-on exercise provided skills applicable in cybersecurity operations and technical interviews
