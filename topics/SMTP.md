# SMTP 
An email protocol used for sending email messages from one email account to another via the internet.

### Email protocol
Sets of rules that define how email clients and accounts exchange information with one another.

### SMTP Server
Handles the sending, receiving and relaying of emails.

### How SMTP works
When a SMTP server is established, email accounts can connect and sent emails through this server. When the user 'sends' an email, the email client establishes a connection to the SMTP server.

When the email has arrived at the SMTP server, the client sends commands to tell the server what to do with the email and transfer data. The Mail Transfer Agent or Message Transfer Agent (MTA) checks to see if both email addresses are from the same email domain, such as gmail.com. If they are, it sends the email right away
If not, the server uses the Domain Name System (DNS) to identify the recipient’s domain and then send it to the right server.

### SMTP Commands
**HELO/EHLO (hello):** Email client identifies itself to a SMTP server. SMTP server sends back the command back with its domain name and IP address

**MAIL FROM**: sender shares code that specifies where the email is from. This outlines the email address and tell the SMTP server that a new transaction will occur from here. From here, the server resets everything and is ready to accept the email address. Once accepted, it will reply with a 250 OK reply code.

**DATA:** This triggers the transfer of data between the client and the server. All of the message contents will be moved to the SMTP server, which will respond with a 345 reply code. The contents of the messages are transferred to the server, where a single dot is sent in a line by itself to signal the end of the message. If accepted and ready for delivery, the server sends another 250 OK code. At this point, the message is on its way to the recipients.

**RCPT TO (recipient to):** The next command follows the 250 OK reply code identifying who the email is being sent to. Again, the SMTP server responds with the same code, at which point another RCPT TO command can be sent with a different recipient’s email address. This can go back and forth as many times as required depending on how many people will receive the email.

**QUIT**: When the email has been sent, the client sends the QUIT command to the server, severing the connection. If it has been successfully closed, the server will reply with a 221 code.

![SMTP commands](https://github.com/Danglevuminh/notes/blob/master/img/smtp%20commands.png)

### SMTP Error codes
**4.X.X Persistent Transient Failure:** Temporary failure with the mail server. Often used by the server to keep untrusted users at bay.

**5.X.X Permanent Error:** SMTP connection has dropped.
