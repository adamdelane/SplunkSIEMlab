# Opening port 514 in Windows Defender Firewall

This allows my Windows VM to receive the log files.

![Screenshot of Windows Defender Firewall config screen](https://github.com/user-attachments/assets/5ea5a0ac-d608-4861-9894-94f600776aba)


# Syslog Capture Folder

This is where syslogs are saved, ready to be ingested by Splunk.

![Screenshot of Windows 10 Explorer](https://github.com/user-attachments/assets/d5984108-c169-422c-8e50-4e0ed23adca5)

# Enable Syslog in Ubuntu

This enabled the Syslog forwarding service on my Ubuntu server VM.

![Screenshot of Ubuntu CLI](https://github.com/user-attachments/assets/a4469823-b267-47fd-bd99-d6561a7cd8ad)


# Configure Syslog reception / forwarding

This enables Syslog forwarding on UDP / TCP port 514.

![Screenshot of Ubuntu syslog forwarding config file](https://github.com/user-attachments/assets/2732c15b-7611-4243-86b1-c223d254e75e)

This dicates the IP address the syslogs are to be sent to, as well as whether they should be sent via TCP or UDP. The IP address shown in the screenshot is the IP address of my Windows 10 VM, and the "@@" means "TCP"

![Screenshot of Ubuntu syslog forwarding config file](https://github.com/user-attachments/assets/dbff0b9b-25b4-4a7f-9579-6805a5ca8923)

# Kiwi Syslog

Kiwi Syslog was used as a log receiver in place of Splunk Universal Forwarder as it is a lightweight, easy to set up solution for receiving logs send on Syslog protcol port 514. It allowed me to focus on log collection, parsing and visualtion without the added complexity of configuring individual log shippers or endpoint agents

![Screenshot of Kiwi Syslog Interface](https://github.com/user-attachments/assets/369cf24a-3a95-4a5f-84ca-e7f2a1b9dc0e)

Enabling of Kiwi Syslog recevier to receive syslog files on port 514.

![Screenshot of Kiwi Syslog settings screen](https://github.com/user-attachments/assets/1e746ace-9fc5-42d6-911c-96592643aed0)

Example of a test entry from the Ubuntu log file

![Screenshot of Kiwi Syslog receiving a log file](https://github.com/user-attachments/assets/1dd32e9b-77c4-4c06-803c-aac1aeedb477)

# Splunk config

Adding lo

<img width="1436" height="658" alt="adding log file" src="https://github.com/user-attachments/assets/d064048a-2d56-411e-8a6c-d85dbe7b58ef" />




