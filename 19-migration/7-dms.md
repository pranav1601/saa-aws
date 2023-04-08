## dms

- migration of rlation db, warehouses, nosql, other daa stores
- migrate data between aws and on premise. both ways
- can be used as one time or continuous sync
- SCT - translate db schemas to new platforms


## works

- server running replication softweare
- create source and ttareget connection for loading from and to
- schdule tasks to run on the dm server to mvoe data
- aws creates the table and primary keys
- create your target tables before hand if desired
- leverage SCT fro creating som,e or all of your tables, indexes and more
- source and target data stores are referred to as endpoints

## concepts

- same engine - easily migrate between source and target endpoints with the same engine types eg - mmysql to mysql
- different enfines- migrate between source and target endpoints with diffferent engines - eg orace to postgresql
- must have one endpoint to live within an aws service
- cannot be useed exclusively outside of aws

## schema conversion tool SCT

- conver ecisting db schema from one engine to other
- converts many tpes of realtional db, including OLAP and OLTP. supports data warehouses
- converted schemas can be used for any supported rds engine tpe, aurora or redshift
- can use the converted schemas with db running on ec2 or data stored in s3

## migration type

1. full load - all existing data is moved from souces to targets in parallel
2. full load and change data capture cdc - full load plus cdc captures changes to source tables during migration - only one to guarantee transactionaly integrity of target db
3. cdc only - only replicate the data changes from the source db

## migrate large data stores with snowball

- problem - terabytes, bandwidth throttles
- leverage snoball edge devices and s3 with dms to migrate data setes quickly
- SCT - leverage sct to extract data into snowball devices then into s3
- load converted fata - can still load the extracted data from s3 and migrate to the chosen destination
- cdc compatible - leverage cdc for capturing changes when extracting data to store in s3

> easy db migrations
>
> 