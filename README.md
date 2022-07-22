# Rancher and Private Registry Hands-on Workshop
This repository content provide the lab exercise guide for a hands-on workshop to help audience to understand and explore the open source technologies like Rancher and OPA in managing and securing containers on cloud based repositories like Azure Container Registry and/or private repositories such as Harbor.



## Open Source Technologies Used

| Software | Version         | Remarks                                                      |
| -------- | --------------- | ------------------------------------------------------------ |
| Rancher  | 2.6.6           | Enterprise-grade Kubernetes Management Platform              |
| RKE2     | v1.23.6+rke2r1  | Rancher Kubernetes Engine 2 - with Kubernetes version 1.23.6 |
| OPA      | 100.1.0+up3.7.1 | Open Policy Agent Gatekeeper: Policy and Governance for Kubernetes |
| Harbor   | v2.2.2-56d7937f | Project Harbor is an an open source trusted cloud native registry project that stores, signs, and scans content. |
| Trivy    | v0.16.0         | Aqua Trivy: Vulnerability and Misconfiguration Scanning      |



## Lab Exercises

* Access to the lab environment
* [Exercise-01-Deploy Monitoring and Istio onto RKE2 cluster](https://github.com/dsohk/rancher-istio-workshop/blob/main/docs/Exercise-01-DeployMonitoringandIstioonRKE2Cluster.md)
* [Exercise-02-Deploy Sample Bookinfo Microservices Application](https://github.com/dsohk/rancher-istio-workshop/blob/main/docs/Exercise-02-DeploySampleBookinfoMicroservicesApplication.md)
* [Exercise-03-Traffic Shaping with Service Mesh Canary Deployment](https://github.com/dsohk/rancher-istio-workshop/blob/main/docs/Exercise-03-Traffic-Shaping-with-ServiceMesh.md)
* [Exercise-04-Visualize Service Mesh with Kiali](https://github.com/dsohk/rancher-istio-workshop/blob/main/docs/Exercise-04-Visualize-ServiceMesh-with-Kiali.md)
* [Exercise-05-Explore Distributed Tracing with Jaeger](https://github.com/dsohk/rancher-istio-workshop/blob/main/docs/Exercise-05-ExploreDistributedTracingwithJaeger.md)
* [Exercise-06-Explore NeuVector and how it secure microserivces](https://github.com/dsohk/rancher-istio-workshop/blob/main/docs/Exercise-06-ExploreNeuVectorandhowitsecureMicroservices.md)

## References

* [Rancher Documentation](https://rancher.com/docs/rancher/v2.6/en/)
* [Istio Documentation](https://istio.io/latest/docs/)
* [NeuVector Documentation](https://open-docs.neuvector.com/)

