# cilium-bgp-example
Example of a Cilium implementation connected to BGP router (frr on ubiquiti UDM)

This enables me to advertise/anounce all pod IP and all Service IP of the kubernetes cluster to my main gateway/router.

Resulting in a setup where all devices in my (v)LAN(s) have a route available to the services and pods inside the kubernetes cluster.



The values.yaml is used to setup Cilium 1.17.2 in my setup.
You need to enable bgpControlPlane to use BGP

```
bgpControlPlane:
  enabled: true
```

For other options needed/used, best check the official documentation.

This is a working example in my home lab.
