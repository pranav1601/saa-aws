## service catalog

- allows orgs to create and manage catalogs of approved IT services
- list things like ami, server, sw, db, preconfigure components
- centrally manage it services and maintain compliance
- end users can be allowed to easily deploy preapproved catalog items within an org
- catalog templates are written and listed using cloudformation templates

## uses

- standsardize - restrict launching products to a specific list of preapproved soltuions
- end users can browse profucts and deploy approved services on their own
- access control - add constraints and grant access to products using aws IAM
- versioning - update products to new version and prpagate changes automatically

## aws proton

- creates and manages infra and deployment tooling for users as well as serverless and container based applications
- IAC-automate infra as code prvisioining and deployments
- define standardized infra for you serverless and container based apps
- use templates to define and manage app stacks that contai all components
- prvisions resources, configures CI/CD and deploys the code
- supports cft and terraform IAC

> enable developers to move faster with a self service toll to provision infra and manage code deploymenets     