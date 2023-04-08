## relational db

* data organized into tables
* data itmes - rows
* fields- columns
* sql server, postgresql, oracle, mariadb, mysql, amazon aurora
* up and running in minutes
* rds- ec2 instance with only access to db
* multi az
* automatic failure capability
* automated backups
* db in own data center takes 8 days or longer

## when to use rds

* oltp - online transaction processing - rds
* oltp - rpocesses data from transactions in real time
* * all about data processing and completing large numbers of small transactions in real time
* olap - online analytical processing - processes complex queries to analyze historical data - redshift
* * data analysis using large amoutns of data as well as complex queries that take a long time to complete

## multi az rds

* creates exact copy of rds in a different az for automatic failover
* sql server, mysql, mariadb, oracle, postgre sql - not aurora in single az
* it is for disaaster recovery, not to improve performance

> rds is for oltp  -small transcations
>
> not suitable for olap