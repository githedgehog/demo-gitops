# Demo setup

- reset `demo.yaml` to `demo.reset.yaml` state
- make sure ArgoCD is synced and applied on switches
- make sure `server-1` and `server-4` got IPs from DHCP and can ping their gateways

```console
hhnet cleanup
hhnet bond 1101 enp2s1 enp2s2
ping 10.30.101.1

hhnet cleanup
hhnet bond 1102 enp2s1 enp2s2
ping 10.30.102.1
```