## guard duty

- uses ML to montior malicious behaviors
- unusual API calls from malicious IP
- attempts to disable cloudtrail loggin
- unauthorized deployments

## features

- alersts appearn in guardduty and CW events
- receives feeds from third parties like proofpoint, crowdstrike, AWS sec about malicious domains and iP addresses
- monitors cloudtrail logs, vpc flow logs ad DNS logs
- centeralize thread detection
- autmated response using CW events and lambda
- ML and anomaly detection

## threat detection with AI

- 7-14 days to set baseline
- once active, you will see findings on the guard duty console and in CW events 

## prciing

- 30 days free
- after that based on CT evenets
- volume of DNS and VPC flow logs data

> updates a db on know malicioud domains using external feeds from third parties
>
> CW events can be used to trigger lambda dunction to address a threat