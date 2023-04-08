## acid

* atomic - all changes performed successful or notjing
* consistent - should be consistend
* isolated - no other process can cahnge when transaction running
* durability - the change should sustain
* dynamodb used for this transcations accross 1 or more tables in single AWS account and region

## uses

* financial transactions
* managing orders
* multiplayer game engines
* coordination actions across different services

## transcations

* multiple or notjing transactions
* financial transactions
* fulfilling orders
* 3 options for reads - eventual consistency, strong consistency and transactional
* 2 options for writes - standard and transactional
* up to 25 items or 4mb of data

> ACID requirement -> ddb transactions
>
> all or nothing transactions