# Docker Registry deployment instructions


## NOTICE ! 
- this is just a simple configuaration and it's not based on best practices.
- I would recommend to use Harbor docker registry on production. 
	- you can customize it's UI , use Volunrabality scanner , retention policy , CRD and ... .
- the repo has tested with Digital Ocean K8s.
- I have deployed NFS storage for ReadWriteMany file-system solution.
I have used DO blockstorage for redis. 


## Directories overview

- [htpasswd](htpasswd) 
  - secret for docker registry username and password.
- [redis](redis) 
  - simple redis instance for caching processes.
- [garbage](garbage) 
  - cronjob for garbage collection.
- [registry](registry) 
  - all needed yaml files to launch and expose docker registry.

