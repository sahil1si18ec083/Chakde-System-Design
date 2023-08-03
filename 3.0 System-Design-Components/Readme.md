# MONOLITHIC FRONTEND vs MICRO-FRONTEND
When it comes to structuring and developing frontend web applications, there are two main approaches: monolithic and micro-frontend. 
A monolithic frontend application is built as a single, large codebase where all the application code is contained in one place.
A micro-frontend application, on the other hand, is composed of several independent micro-applications or microservices that can be developed,
deployed, and scaled independently.

![image](https://github.com/sahil1si18ec083/Chakde-System-Design/assets/103936307/75ad59cc-378c-4d21-9b43-ed0d13a7c41e)

## Differences between Monolithic and Micro-frontends
![image](https://github.com/sahil1si18ec083/Chakde-System-Design/assets/103936307/274c11f9-a4e7-45e3-97b0-f2000634eaeb)

### Reference:
 https://xhulqornayn.hashnode.dev/monolithic-frontend-vs-micro-frontend-application-differences-pros-and-cons

# **Communication Protococols**
There are three ways of Communication Protococols
1. Normal HTTP Requests
2. Long Polling
3. Web Socket
4. Server Sent Event

### HTTP request
This is a one time connection between client and server. Everytime there is a service call, a new handshake is made
Then, the server does its work and sends the response back to the client using that already opened connection.
And then finally the connection gets closed. That's it.
One of the use-cases of the HTTP requests is: Fetching the profile information in Facebook applications.
### Long Polling
In Long Polling a bi-directional connection is established between client and server but the api calls are made at regular intervals of time 
Suppose we keep the interval time 3000ms. So after every 3000ms , client will try to fetch the response from the server 
One of the best useCases is our Cricbuzz.com where there is running commentary and score gets updated after every 5000ms 
Why we are taking 5000ms as polling time because approx after every 5000ms, ball is bowled in cricket and score board gets updated.
### Web Socket
In case of web socket, there is a permanent connection established between client and server.
And client is doing live retrival of data from server.
one best use case is Zerodha where live data is gets fetched from server and there cannot be delay of even a small interval

### Server Sent Event
Here server only notifies the client that there is some update and it needs to be updated on client.
One of the best use Case is Notification Feature on Instagram

# Availability
When the server is down, the user should be kept engaged by showing some static web till the server is up
# Accesibility
User should be able to access application in diffrent languages so that it can be accesssible by all sections of society
Enable screen readers
# Consistency
Diffrent browsers should have consistency with the application.
Like in diffrent browsers, application should behave and look in a same way
By putting some efforts, we are able to make our application Consistent
# Credibility & Trust
SEO
1. ON-Page
   -- title
   --description
   --performance
   
2. Off-Page
   --Advertisements
By these two types of techniques, we can establish  Credibility & Trust in our Application

# Logging & Monitoring
Error logging is important, should show message toasts that there is a particular error
Understanding the user is very important, what type of users are using our Application

# Databases & Caching
We need a  database in order to be stored in DB and we can fetch the data from the server.
Catching is we are storing data in client side only and we can use it anytime 
Catching is like database of client side
Local storage, cookies,  redux all comes under Catching

# Security
Authentication and Authorization of users is very important
Authenication means I am authenicated to youtube.com after my mail id is verified through Gmail
But authorization means me as a user has access to watch only videos on youtube but I am not authorized to access the creator page which only the youtube creators can have access.
So in a way Youtube creators are authorized to creator page but I am not.
But we both are authenicated on youtube.com

_When we are designing an application , we need to have proper Authentication and Authorization so that there will not be any security issue_

# Performance & Optimization
1. Use cdn links for images
2. Lazy Loading
3. Memoization

# Testing
1. Unit testing: How small componets are individually working
2. Integration Testing: How combined components are working
3. End to End testing: Testing the entire Flow




   



