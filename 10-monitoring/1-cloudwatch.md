## monitoring

* checks to catch any faults before catastrophe stikes

## cloudwatch

* monitoring and observability platform gives insight to architectures
* monitor mulitple levels and identify potential issues

## features

1. system metrics - cpu high, memory high. etc
2. application metrics - install CW agent inside ec2 - is apache server working, what is going inside the application
3. alarms - alert when something goes wrong

## metrics

1. default - no additional config - generally data that aws can see
2. custom - provided by using the CW agent installed on the host

> monitor - cloudwatch
>
> know the basic checks
>
> alarms - no default, must be created
>
> deafult vs custom - aws cant see past the hypervisor level
>
> managed service - more manged - more checks out of the box
>
> standard vs detailed - standard is 5 - minute intervals, detail is 1 minute
>
> real time - kinesis