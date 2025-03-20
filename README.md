# cilium-bgp-example
Example of a Cilium implementation connected to BGP router (frr on ubiquiti UDM)

The values.yaml is used to setup Cilium 1.17.2 in my setup.
You need to enable bgpControlPlane to use BGP

```
bgpControlPlane:
  enabled: true
```

For other options needed best check the official documentation.

This is a working example in my home lab.

