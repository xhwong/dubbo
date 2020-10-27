## 负载均衡

> 下文将重点解析负载均衡部分

#### 概述
+ 对于dubbo的负载均衡，更偏向于调用方的限制，在调用服务提供者之前辨别服务提供者的能力来进行调用。
+ 目前最新的分别提供了5种负载均衡算法，分别是:

```
random=org.apache.dubbo.rpc.cluster.loadbalance.RandomLoadBalance
roundrobin=org.apache.dubbo.rpc.cluster.loadbalance.RoundRobinLoadBalance
leastactive=org.apache.dubbo.rpc.cluster.loadbalance.LeastActiveLoadBalance
consistenthash=org.apache.dubbo.rpc.cluster.loadbalance.ConsistentHashLoadBalance
shortestresponse=org.apache.dubbo.rpc.cluster.loadbalance.ShortestResponseLoadBalance
```



#### 源码