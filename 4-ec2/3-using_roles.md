## what is IAM role

* specific permissions
* aws identity in aws that has permissions
* designed to be consumed by someone who needs it
* role as temoprary
* when assume a role-> temporary crendetials given
* allow cross account access

## creating a role

* go to IAM
* then roles
* create role -> aws service or another aws account or web identity or saml
* choose a use case
* attach policy
* add tags
* add name

> preferred option from sec perspective
> 
> avoid hard coding credentials
> 
> policies control a roles permission
> 
> upate a policy attached to the role
> 
> attach and detach role to running ec2 instance siwthout stoppping them