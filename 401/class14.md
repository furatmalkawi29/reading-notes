


## What’s the difference between a FIFO and a standard queue?

Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue

## How can the server be assured a message was properly received?

By adding a message queue into our server that will be listening to received event for example from the client side, and when that event emitted from the client it will delete the request from the queue in the server.

Message Queues are so useful to store the data and make sure nothing is lost in case any other server went down.

## What classic design pattern is best represented by event driven programming?

Behavioral (Observer) design pattern

## How do you test an event driven system?

Start the application under test.
Send some input events to the server.
in the server try to console log each event data.
Wait until the application has listened to the events been send.
Assert that the data is logged and as you want.


# terms 

## Fifo queue 

FIFO queues used in messaging between applications when the order  events is important, or where events duplicates cant be handled 

## Pub/sub

Publish/subscribe messaging , its  real-time communication used to publish and subscribe to asynchronous events.

![](https://d1.awsstatic.com/product-marketing/Messaging/sns_img_topic.e024462ec88e79ed63d690a2eed6e050e33fb36f.png)


<br><br>

# SNS vs SQS

- SNS is a distributed publish-subscribe service.
- SQS is distributed queuing service.

- You can have SNS send messages to email, sms or http end point apart from SQS. There are advantages to coupling SNS with SQS. You may not want an external service to make connections to your hosts (firewall may block all incoming connections to your host from outside).


- SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. 