## caching

- external - cache data that will be returned to users
- internal - cache queires to speed up data bases

## otpions

1. cloudfront - cdn, external
2. elasticache -internal, infront of db
3. DAX - ddb accelarotr
4. global accelarator

> pick a solution that includes caching
>
> spped - decreases latency
>
> can it be cahched?
>
> what kind of cache to be used
>
> how does content get updated? (ttl)
>
> does it add anything beside speeds? (cf helps with security, gloabal ax solves problemebm of chaning ip)