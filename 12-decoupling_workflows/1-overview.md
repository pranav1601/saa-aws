## tight coupling

* user -> frontend(EC2) -> backend(EC2)
* one instance talking directly to another instance

## loose coupling

* user -> ELB -> frontend(multiple instances) -> ELB -> backend(multiple instances)
* frontend and backend not talking to eachother
* scalable and highly available
  
## service that help in this

* SQS -> message queueing service
* SNS -> messaging service for Application to application and application to person
* API gateway -> publish APIs at scale
  
> Never tightly couple
>
> No EC2 talking to another EC2 directly
>
> every level of application should loosely coupled
>
> > syncrhronous or asynchronous
>
> what type of decoupling
>
> order of mesages
>
> type off appication load