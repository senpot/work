# How to Deploy AWS Loadbalancer Controller for EKS Private Cluster

## Reference
* https://docs.aws.amazon.com/ja_jp/eks/latest/userguide/aws-load-balancer-controller.html

## Issue
* AWS Loadbalancer Controller attempt to connect to WAF Endpoint by default settings. So we could not deploy ALB Ingress Controller in EKS Private Cluster.

## Solution

### Added some args in Deployment
* EKS Private Cluster can't connect to WAF Endpoint, So I added some args to Deployment.

```yaml
apiVersion: apps/v1
kind: Deployment
(snip)
spec:
  template:
    spec:
      containers:
      - args:
        - --enable-shield=false
        - --enable-waf=false
        - --enable-wafv2=false
(snip)
```
