## kms

- key management service
- create and control encryption keys to encrypt data
- ebs, s3 rds
- centralized control
- control who can manage kets separately from who can use them

## cmk

- customer master key
- logical master ke
- metadata such as key id, creation data, descrption and key state
- contains key material used to encrypt and decrypt data

- request creeation of cmk
- control lifecycle of cmk and management

## hsm

- hardware securtiy module
- physical computing device that safeguards and manages digital keys and perform encryption and decryption
- contains one or more secure cryptoprocessor chips

## 3 ways to generate cmk

1. aws creates. generated within HSM
2. import key material from own key management infra and associate with a cmk
3. have key material generated and used in cloudhsm cluster as part of custom key store feature in aws kms

## key rotation

- choose kms to auto rotate cmk every year provided that the keys were generated within aws kms hsm
- not supported for imported, ayssmetric or keys generated in aws cloudhsm cluster using the aws kms customer key stpre featre

## policies

- primary way to manage cmk
- attach resource basedd policies to cmk, called key policies
- all msk cmk have a key policy

## control permission

1. use key policy
2. use iam policy with key polucy
3. use grants in combination with key policy - allow users to delegate access

## cloudhsm

- cloud based hsm that generated own encryption keys on cloud
- physical device entriel dedicated to you that can be deployed in highly available fashion

![kms vs cloudhsm](../images/kmsvscloudhsm.png)