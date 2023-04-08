## sticky sessions

* classic load balancer route each request to registered ec2 with the smallest load
* sticky sessions allow you to bind a users session to a specific ec2 instance
* ensures all requests from the user during the session are sent to the same instance

## scaling issues

* if we terminate an instance, still load balancer will send that ec2 which is terminated which wont work
* so disable sticky sessions

> users to stick to same ec2 instance
>
> disable sticky session to avoud load balancer sending user to same ec2