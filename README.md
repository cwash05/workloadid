# workloadid
script for creating aks cluster with 
- workload identity
* api vnet integration
node and pod subnets
azure network plugin
azure network policy
azure defender
azure keyvault secrets provider
kubelet identity
running on Mariner/W2022 node pools

A keyvault is setup with a secret 'Secret1'.
A workload(managaed) identity is setup ${aksPrefix}-workid.
A service accoount {aksPrefix}-sa is created in namespace {aksPrefix}-ns.
A federated account is seteup ${aksPrefix}-fed.
A quick-start pod is createed using the service account and pulls the secret from the keyvault

You can get the logs for the quick-start pod to verify workload identity. 
   
**kubectl logs quick-start**

```script
I1013 22:49:29.872708       1 main.go:30] "successfully got secret" secret="Hello!"
```
