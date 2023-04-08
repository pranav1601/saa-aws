## DLQ

* sideline messages
* after specific number of retires, the problematic messages will move to DLQ
* link to a SQS

> problem with SQS? think about DLQs and visibility timeout
> 
> setup CW alarm to monitor queue depth
>
> just SQS that receive the reject message
>
> same retention window of 14 days
>
> you can use it for SNS