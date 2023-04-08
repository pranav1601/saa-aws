## ecr

* aws manageed
* container image registry
* private container eimage repos
* supports open container initiative images, docker images, oci artifacts

## components to know

- registry - private registry for each aws account
- auth token - for pushing and pullin
- repo - contains docker images, oci image, oci artifacts
- repo policy - control all access
- image -container images that get pushed to and pulled from your repository
- ecr public - used  for public images

## lifecycle policies

- helps in management
- rules for cleanin up unused images
- ability to test your rules before applying them

## image scanning

- help identify software vulnerabilities in container images
- can be set to scan on push
- retrieve results of scan for each image

##  sharing

- cross region support
- cross account support
- configured per repository and per region

## cache rules

- cache public repos privately
- periodically reaches out to check current caching status

## tag mutability

- prevents image tags from being overwritten
- configured per repo

## integrations

- still use images within your own container infra
- ecs
- eks
- amazon linuz container can be used locally for your software development

> container image storage - aws managed
>
> keywords - manageed image registry, oci repos, images integration with ecs and ek