## s3 object lock

* store objects with WORM model -> write once, read many times
* prevents objects from being deleted or modified for a fixed amount of time 

## governance mode

* cant overwrite or delete an object version or alter its setting unless they have special permissions
* give some users permission to alter the retention settings or delete

## compliance mode

* cant be overwritten or deleted by any user including the root user

## retention periods

* protects object version for a fixed amount of time
* after retention period expires the object version can be rewritten or deleted unless legal hold is present

## legal hold

* protects an object version from being overwritten or deleted
* does not have a retention period
* can be placed and removed by any user who has s3:putobjectlegalhold permission
  
## glacier vault lock policy

* implement worm model to glacier
* easily deploy and enforce compliance
* once locked, policy cannot be changed

> worm -> s3 object lock
> 
> individual object or whole bucket
> 
> governance mode or compliance mode
> 