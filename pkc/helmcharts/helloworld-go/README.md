# Helloworld go application

Helloworld-go is a web application written in GO and delivered as an helm chart by CSF.
it's a simple application that could retun a message to the user like "Hello world!" on different languages.
The language of helloworld is set by configuring "language" value in values yaml file of the chart


## Installation via Helm
Installation is done by running helm install command like in the following example :
- helm3 install myhelloworld mychart --namespace myns


## k8s ressources

### Rollback/backup

Helloworld use cbur asset to backup/restore k8s ressources, volumes and cluster data for a specific release.
By default the brpolicy value is false, to activate the backup & restore utility, user should set the values "cbur.enabled=true and pvc.enabled=true" 


## NOTE: 
If cbur is not installed with NCS , user could install it manually by using helm command


### Ingress

HTTP/TCP Trafic is controlled by kubernetes Ingress and byt API Gatway, to have access to helloworld for an esternal user, Ingress ressource would be activated but setting the values "ingress.enabled=true,ingress.tls.enabled=true"

