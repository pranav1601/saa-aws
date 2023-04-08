## scaling options

* scaling is simplified in dynamodb - aws dows all heavy lifting
* provisioned - predicatable workloads, need to review past usage to set uppper and lower scaling bounds, most effective cost model
* on deman - sporadic workload, on deman, pay small amount for read and write, less cost effective

> keep cost in mind when scaling dynamodb - exam fenerally approach from a cost perspective
>
> predicatble - provisoned
>
>  sporadic - on demand
>
> access patterns - need to now if predicatable or unpredicatable
>
> design matters - avoiding hot keys will lead to better performance
>
> switching will only   happens once every 24 hrs