## push based messaging

* decided when the message is sent. delivers messages to the endpoint subscribed to it

## settings

* subscribers-> topic is published -> message sent to that topic -> resource is subscribed
* 256 kb of text in any format
* DLQ support
* fifo/standard -> fifo only supports SQS as subscriber
* encryption -> encrypted in transit but not add at-rest by default

> SNS used with SQS to fan out messages. Multiple messages might need to be sent to multiple groups that require the message/alert
>
> alerts=SNS
>
> push based notification
>
> CW needs SNS to alarm
>
> need to know all subsriber options
>
> SES is for marketing emails only
>
> email notification means SNS
>
> no retries other than HTTP