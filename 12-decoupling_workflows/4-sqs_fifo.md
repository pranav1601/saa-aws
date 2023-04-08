## sqs message ordering

* guarantees ordering and no duplicate messages
* 300 message per second only compared to unlimited
* name ends with .fifo
* message belongs to a specific group
* deduplication id given so that in a set interval there is no deduplication

> FIFO the only option when it comes to message ordering
>
> lower on performance -> only 300 ps
>
> user can do it on their end to use SQS standard by message id as message
>
> message group id process one by one
>
> cost is more