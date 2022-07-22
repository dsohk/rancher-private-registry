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

This lab is consiting of 3 exercises 

* Exercise-01
  * [A-Scanning container image for vulnerabilities through Trivy on Harbor](https://github.com/dsohk/rancher-private-registry-workshop/blob/main/docs/Exercise-01A-ScanContainerImages.md)
  * [B-Setting up Harbor as a proxy to Azure Container Registry (ACR) and replicating images to ACR](https://github.com/dsohk/rancher-private-registry-workshop/blob/main/docs/Exercise-01B-SetupHarborProxyReplicateACR.md)
* Exercise-02
  * [A-Integrate Harbor with Rancher](https://github.com/dsohk/rancher-private-registry-workshop/blob/main/docs/Exercise-02A-IntegrateHarborRancher.md)
  * [B-Deploy sample application rancher/hello-word from Harbor onto RKE2 cluster ](https://github.com/dsohk/rancher-private-registry-workshop/blob/main/docs/Exercise-02B-DeploySampleApplication.md)
* Exercise-03
  * [A-Installing OPA on RKE2 cluster](https://github.com/dsohk/rancher-private-registry-workshop/blob/main/docs/Exercise-03A-InstallOPA.md)
  * [B-Setting up OPA constraint for registry access](https://github.com/dsohk/rancher-private-registry-workshop/blob/main/docs/Exercise-03B-SetupOPAConstraint.md)

## References

* [Rancher Documentation](https://rancher.com/docs/rancher/v2.6/en/)
* [Harbor Documentation](https://goharbor.io/docs/2.2.0/)
* [OPA Documentation](https://www.openpolicyagent.org/docs/latest/)

