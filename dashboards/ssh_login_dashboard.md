# Search visualisation

Here I used the data visualisation tool to turn my search into something more user friendly. 

This was achieved by piping the results of "Failed password" NOT "Invalid user" to "stats count", then piped again to "table count".

I formatted the colour settings to change the background of the text from green, to orange, to red based on the value present.

![Screenshot of Splunk data visualiser screen](https://github.com/user-attachments/assets/56c86e7a-aa26-47c1-a4f2-686f0f2cd41e)

# SSH login dashboard

This dashboard contains the data visualation from above, as well as a pie chart which illustrates the amount of failed and successful logins (this is based on the custom field extraction search from [searches/ssh_search.md](https://github.com/adamdelane/SplunkSIEMlab/edit/main/dashboards/ssh_login_dashboard.md))

![Screenshot of Splunk dashboard editor](https://github.com/user-attachments/assets/43f8f698-c165-4bb1-b89e-6dede21dff47)

# SSH failed login colour change

Once the data passes a certain value, the background colour changes 

<img width="1689" height="639" alt="shh fail colour change example" src="https://github.com/user-attachments/assets/f67451d5-cd7a-4f6f-b7bc-313e1d260a03" />


