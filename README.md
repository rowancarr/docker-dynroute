docker-dynroute
===============
Basic docker containers using the [dynroute](https://www.npmjs.org/package/dynroute) npm packge to update your aws route53 domains for dynamic ip address's

## Usage

Dynroute requires you load your aws creds into a .awsrc file, i have this on my host machines and load it up via the command line. 

### Standalone
```
docker run --rm -v /root/.awsrc:/root/.awsrc --name dynroute rowancarr/docker-dynroute dynroute -d os1.devopsbeards.com 
```

### Coreos/Fleetctl

```
fleetctl start dynroute.service
```




