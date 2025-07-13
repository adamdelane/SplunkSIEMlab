# "Invalid user" ssh search

Creating "Invalid user" log data on my Ubuntu VM

![Screenshot of Ubuntu CLI](https://github.com/user-attachments/assets/e5bc150a-cdbe-4453-acd4-181759bd8400)

Searching inside the "network" index, within the ubuntu log file, for any messages that contain the phrase "authentication failure" or "invalid user".

![Screenshot of Splunk search screen](https://github.com/user-attachments/assets/139127f7-ca14-4519-bf39-c610bc7a9550)

# ssh login results search

Here I created an example user called "user1" and give it a password. This would allow me to SSH in to the user and create some successful and unsuccessful login attempts.

![Screenshot of Ubuntu CLI](https://github.com/user-attachments/assets/a59b56ec-c8cc-48e1-840e-cdbdae561dcb)

I attempted to SSH into the user multiple times, giving an incorrect password each time. I then searched for log entries which contained "Failed password" and didn't contain "Invalid user". This is because I only wanted to see log entries for failed login attempts of legitmate users.

![Screenshot of Splunk search screen](https://github.com/user-attachments/assets/620f52c1-9915-4d97-a307-07b4302c07dd)

I also generated some successful login data. I created a search which showcased both successful and unsuccessful logins for legitimate user accounts.

![Screenshot of Splunk search screen](https://github.com/user-attachments/assets/6b86f260-7445-4439-a5b9-e3bc796c2282)

