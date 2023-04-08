## x-ray

- collects app data for viewing , filteting and gaining sights about requests and responses
- downstream - view calls to downstream aws resources and other microservices/api or databases
- traces - receives traces from your apps for allowing insights
- mutlple options - intergrated services can add tracing headers, send trace data, or run the x-ray daemon

## concepts

- segments - data containing resource names, request details and other info
- subsegments - segments prvodigin more granular timing information and details
- service graph - graphucal representation of interacting services in requests
- traces - trace id tracks paths of requests and traces collect all segments ina request
- tracing header - extra http header containing sampling decisions and race id
- tracing header contianing added info is name x-amzn-trace-id

## x-ray daemon 
- aws software application that listens on udp port 2000. it collects raw segment data and sedns it to the aws x-ray api
- when the daemon is running it works along with the aws x-ray sdk

## integration

- ec2 - running agent
- ecs- within tasks
- lambnda - on/off toggle
- elastic beanstalk
-  api gateway
-  sns and sqs

> application insights - aws x ray
>
> viewing response times of downstream resources
>
> http resposne analysis
> 