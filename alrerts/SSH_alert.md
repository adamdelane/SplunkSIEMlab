# SSH alert configuration

Here I created an alert that would trigger when there are too many failed SSH login attempts in a given time.

<img width="804" height="714" alt="ssh alert 1" src="https://github.com/user-attachments/assets/62a32f55-c223-4235-9599-746c1a28adf4" />

<img width="807" height="695" alt="ssh alrt 2" src="https://github.com/user-attachments/assets/7dbc4ca8-4455-4a00-a067-735f3601ae4e" />

It was set to run every 5 minutes, based on the data received in the last 5 minutes. It would expire in 1 hour to prevent too many alerts being sent.

When more than 10 results are detected, the alert is saved to splunk and emailed to a user.

"Scheduled" was selected over "Real Time" as in a real-life scenario, Real Time analysis would only be used on high risk alerts due to the amount of bandwidth used.

# Alert Summary 

<img width="1251" height="272" alt="alert summary" src="https://github.com/user-attachments/assets/ed143979-4459-4019-a731-fbbffd34374e" />

# Alert Triggering

<img width="1481" height="438" alt="ssh alert triggered" src="https://github.com/user-attachments/assets/838643c7-2dba-414f-b3e8-c5ac9578a8ca" />

<img width="630" height="356" alt="email alert" src="https://github.com/user-attachments/assets/4bcba02a-4da9-47b5-b480-86dc756f38c7" />
