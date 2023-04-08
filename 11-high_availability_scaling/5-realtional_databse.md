## 4 ways to scale

1. vertical scaling - resiziing from one size to another can create greater performance
2. scaling storage - storage can be resiized, but it only goes up, not down
3. read replicas - creating read only copies of our data that can help spread out the workload
4. aurora serverless - offload scaling to AWS, better for unpredicatable workloads

> refactoring and chanign to dynmodb is a viable scaling choice
>
> wont work that easily in the real wrld but switching datatypes can solve the problem
>
> readd-heavy workloads - read replicas (need to update code)
>
> RDS only scales up, aurora scales automatically
>
> turn multi az on until it is a dev env
>
> use aurora if the situation calls for a relational databaase
>
> rds has most db scaling options
>
> horizonatal preferred over vertical (read replicas)
>
> dynamodb comes down to access patterns