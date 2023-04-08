## arn

- uniquely identify resource in aws

## iam policy

- json doc that defines permission
- user/group - identity policy

## permission boundaries

- delegate admin to other users
- prevent privilege esacaltion
- control max permissions an IAM policy can grant
- uses - developers creating roles for lambda functions
- - app ownners crreating roles for ec2
- - admins creating ad hoc users

> not explicity allowed = implicityly senied
>
> explicit deny > everything else
>
> only attached policies have effect
>
> aws joins all applicable policies
>
> aws managed policies vs customer managed policices