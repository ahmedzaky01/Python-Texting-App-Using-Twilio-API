# Python-Texting-App-Using-Twilio-API
 How to Create a Python Texting App Using Twilio API in 6 steps



Have you ever wanted to learn about API's (Application Programming Interfaces) and also build cool projects with them using Python? Well... we will get to do just that. We will create a basic app from scratch. You'll see why Twilio is so special. No previous knowledge required... Let's get started.

#### 1. Create a Twilio Account:

Go to Twilio's website: http://www.twilio.com
Once there you will click on the +SIGN UP button found in the upper right hand corner


Now that you have signed up for an account you will need to obtain a phone number to send messages from.

#### 2. Buy a text Capable Phone Number:

Go to the Buy a Number page (Dashboard Console > Phone Numbers > Buy a Number)

#### 3. Verify a Phone Number on Twilio https://www.twilio.com/console/phone-numbers/verified. That you would like to text.

#### 4. Get Twilio Credentials
 https://www.twilio.com/console
 
 Get Account SID
 
 Get Auth Token

#### 5. Put your twilio credentials and twilio phone numbers in credentials.py

#### 6. Open your terminal and pip install twilio.


```python
 from twilio.rest import Client


 #Your Account SID from twilio.com/console
 account_sid = "" #your account SID from twilio console

 #Your Auth Token from twilio.com/console
 auth_token  = "" #your auth token from twilio console

 client = Client(account_sid, auth_token)
 message = client.messages.create(
 to="your number",
 from_="your twilio number",
 body="message body")

 print(message.sid) #To print sid 
```

#### Congratulations!
 You just sent your first text through your Python Text App that uses the Twilio API.
