# Useful links
* [Wirting on github](https://help.github.com/categories/writing-on-github/)
* [Basic formatting](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
* [Code blocks](https://help.github.com/articles/creating-and-highlighting-code-blocks/)
* [Tables](https://help.github.com/articles/organizing-information-with-tables/)
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

## JMS History
* JMS 1.02b (JSR 58) June 2001
* JMS 1.1 (JSR 914) March 2002 
* JMS 2.0 (JSR 343) May 2013

## Messaging model
* Point to point
  * Terminology
    * Queue
    * Sender
    * Receiver
  * (Sender vs Receiver) or (Producer,Publisher vs Consumer from JMS 1.1)
  * Message delivered to only one consumer
  * Fire-and-forget (Asynchronous)
  * Request-and-reply - need two queues (Synchronous, blocking)
  * Load balancing
  
![Point-to-point](https://github.com/slq/jms-wiki/blob/messaging-models/src/main/resources/point-to-point.PNG)

* Publish and Subscribe
  * Terminology
    * Queue -> Topic
    * Sender -> Publisher
    * Receiver -> Subscriber
  * Message delivered to each subscriber
  * Fire-and-forget broadcast
  * Load balancing of subscribers (JMS 2.0)
  * Subscriber is not known by publisher
  * Queue depth vs Topic depth - there is no topic depth, subscribers can have their own queues

![Publish-subscribe](https://github.com/slq/jms-wiki/blob/messaging-models/src/main/resources/publish-subscribe.PNG)
