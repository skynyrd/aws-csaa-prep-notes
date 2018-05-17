* Simple query service
* Distributed Message Queue
* Messages can contain up to 256KB in any format
* Amazon SQS API
* Pull based (data pushed into the queue by producers and pulled out of the queue by the consumers)
* Message in queue life 1 minute - 14 days
* Visibility Time Out is the amount of time that the message is invisible in the SQS after a reader picks up that message.
    * Max 12 hours
    * Timeout? SQS deletes the message.
    * Job not processed within that time? Message is visible again and another reader will process it.
    * This could result in the same message being delivered twice.
* SQS long polling is continuously asking "Do you have a new message?" to SQS.


* Standard Queues (default)
    * nearly unlimited number of transactions per second.
    * at least once is guaranteed.
    * more than one copy of a message might be delivered out of order.
* FIFO Queues
    * the order is strictly preserved.
    * message is delivered once
    * limited to 300 transactions per second, but have all the capabilities of standard queues