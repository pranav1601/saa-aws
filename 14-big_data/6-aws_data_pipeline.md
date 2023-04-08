## aws data pipeline

- managed TL for automating movement and transformation of data
- data driven workflows - steps dependent on previous tasks
- define parametetrs for data transofrmations. data pipeling enforces the chosen logic
- hihgly available and distributed infra. fault tolerant
- autmaotically retriees failed activities. configure notifcation using sns
- integrates easily with ddb, rds, redshift, s3
- works with ec2 and emr for compute needs

## components

- pipeline definition - business logic of data management
- managed compute - create ec2 or use existing for your activities
- task runner - poll for different task and perform when found
- data nodes - define locations and types of data the will be input and output
- acitvites - pipleine compone nts that define the work to perform

## uses
- process data in emr using hadoop streaming
- import or export ddb data
- copy csv files or data between s3 buckets
- exporting rds data to s3
- copying data to reshift

![data pipeline](../images/data_pipeline.md.png)

> managed aws service for etl workflows
>
> managed etl service, automatic retries for data driven workflows - data pipeline