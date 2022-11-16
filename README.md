# workloadid
script for creating aks cluster with workload identity, api vnet integration, node and pod subnets, azure network plugin, azure network policy, azure defender with kubelet identity running on Mariner/W2022 node pools

You can get the logs for the quick-start pod to verify workload identity. 
   
**kubectl logs quick-start**

```script
I1013 22:49:29.872708       1 main.go:30] "successfully got secret" secret="Hello!"
```
