## inspector

- automated security assessment service
- inspect netork and ec2 instances for vulnerabilities
- ports that are open
- provides detailed list of security findings prioritized y level of severity
- reviewed directly via inspector console or api

## types off assemessment

1. netork - network config analysiis. agent not required
2. host assessments - vulnerable software, hardeinging, sec best practces. inspector agent installed

## work

1. create assessment target
2. install agents on ec2 instances - automatically install the agent for instances that allow systems manager run command
3. create assessment template
4. perform assessment run
5. review findings against rules

> perform vulnerability scans on ec2- host assessment and vpc-network assessments
>
> run once or weekly
>
> vulnerability scans - inspector