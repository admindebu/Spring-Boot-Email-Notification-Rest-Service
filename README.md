# Spring-Boot-Email-Notification-Rest-Service
This POC is developed for send simple text email or attachment email to multiple user using Spring Boot Rest Service
# YouTube Video Explanation Step by Step : https://youtu.be/JsAoKViy3PY

# YouTUbe Video : org.springframework.mail.MailAuthenticationException: Authentication failed : Username and Password not accepted	
https://youtu.be/MHrKr2TFiMM

# Rest API URL
1. Send Simple text Email : http://localhost:8080/v1/notification/textemail  , method : POST , Mediatype : application/json
Body : 
{
	"sendTo" : "xyz@gmail.com,y@gmail.com",
	"subject" : "Test",
	"body" : "Hello"
}

2. Send Attachment Email : http://localhost:8080/v1/notification/attachemail , method : POST 
from-data:  key = file and value is the upload file
Body : 
{
	"sendTo" : "xyz@gmail.com,y@gmail.com",
	"subject" : "Test",
	"body" : "Hello"
}

Here we are giving receipant email address in the properties files in this configuration
email.address=xyz@gmail.com,y@gmail.com,etc...
