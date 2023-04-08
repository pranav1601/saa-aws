## aws phd

- aws health
- visibility of resource perfrmance and availability of service/accounts
- how health events affect you and resources
- maintain timeliness and relevant infromation with events
- view upcoming maintennacnec tasks that affect accounts and resources
- near instant delivery of notifications and alertsd to speed up troubleshooting or prevention

## concepts

- aws health eveent - notifications sent on behalg of healt
- account specific event - event specigific to account or org
- public event - events reportd on services that are public, not specific to aaccounts
- dashboard - shpwogn account and public evets, shows service health as well
- event type code: include affected servies and sepcific type of event
- event type category - associated category- will be attached to every event
- evetn status - reorts if event is open, close or upcoming
- affected entities - which aws resources are or maybe affected by the event

![health](../images/health.png)

> reveive notifications and alerts for affected resources
>
> can automate actions using eventbridge
>
> alerts for service health and sutomating the reboot of ec2 instance for aws maintencance - phd