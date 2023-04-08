## waf

- web application frewall that montors http/https that are forwearded to cloudfront or ALB
- lets you control access to your content
- what ip addresses allow to requests
- alb or cloudfront wil either allow this content or give http 403 status code
- layer 7
- sql injections, cross site scripting

## 3 behaviours

1. allow requests except ones you specify
2. block all requests except one you specify
3. count the requests that match the properties you specify

## conditions

- ip address origin
- country of requests
- value in headers
- presenec of sql code 
- presence of a script
- strings that appear in requests - specific strings 

> block sql injections, cross site scripting