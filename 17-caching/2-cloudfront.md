## cloudfront

- fast cdn - content delivery network
- delivers data, videos, apps, apis to customers to edge locations - decreases laency
- security - defaults to hhtps connectin, allows custom ssl certificate
- cant pick specifi countries, just general areas of the globe
- can be used to front endpoints along tiwth non aws apps
- set a ttl for the content to cache
- can addd temporary access points

>> CF fixes all connection issues

> performance issue can used by puttting CF
>
> slow connectivity - CF
>
> loading takes time -  CF
>
> can be used to block invidivual countries, but WAF is a better tool
>
> cannot pick specific esdge locations for your distributions
>
> only option to add https to a static website being hosted in s3 bucket
>
> in memory db - redis and ddb. favour ddb more
