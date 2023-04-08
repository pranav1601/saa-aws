## SQS

* messaging queue that allows asynchronous processing of work
* one resource writes a message to SQS queue and another message will retrieve from SQS queue
* asnchronous -> no direct communication

## poll based messaging

* whever resource requires he can access the message

## settings
* delivery delay -> default 0 mins upto 15 mins
* message to the SQS will be visible after the deliver delay
* why delay messages? front end info passed to backend for payment -> delay the confirmation message until confirmed
* Message size -> upto 256 kb
* Encryption -> encrypted at transit, not encrypted at rest by default
* message retention -> between 1 minute and 14 days
* long polling vs short polling -> short polling default -> backend instance connects -> checks if work is there -> keeps reconnecting to check -> many api calls and CPU util -> long polling -> connects and hangs around to check -> long polling should be default
* queue depth -> trigger for autoscaling

> user -> EC2(frontend) -> SQS <- EC2(backend)

* visibility timeout -> default 30 seconds -> remains in the queue for instance in queue to utilise the message in the queue -> message reappears in the queue; if message is utilised then message is deleted

> know all settings
>
> message can live for 14 days max
>
> need to pinpont issues
>
> difference between long polling and short polling
>
> 256 kb of text in any format
>
> can dupliate mesages (if happens consistently check for visibility timeout of failing to delete he message)
>
> not biderectional
>
> know the deaults
>
> if order imnportant - fifo
