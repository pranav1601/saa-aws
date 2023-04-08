## cloudwatch logs

* tool that allows to monuitor, store and access log files from different stories.
* query your logs to look for something specific

## log terms

1. log event - record of what happend. timestamp and data
2. log stream - collection of log events. coninuous logs from a single instance
3. log group - collection of log streams. group all your apache web server logs across hosts together

## features

1. filter patterns - look for specific errora
2. CW log insights - SQL like solution to query all logs
3. alarms - create alert on patterns

> logs to CW logs if need to be prcoessed otherwise s3
>
> favor CW logs unless exam asks for a real time soltion
>
> alarms - used to alert of filter patterns found
>
> agent must be installed and configured, not automatic
>
> SQL - think cloudwatch insights