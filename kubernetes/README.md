# Kubernetes

## Howtos
* [Generate Network Policy by sniffing network traffic](https://itnext.io/generating-kubernetes-network-policies-by-sniffing-network-traffic-6d5135fe77db)
* [Flatcar linux](https://www.rkatz.xyz/post/2020-09-13-flatcar/)
* [Kubernetes the hardway](https://github.com/kelseyhightower/kubernetes-the-hard-way) by Kelsey Hightower
* [k8s examples](https://github.com/knelasevero/kubernetes-examples)
* [k8s by example](https://kubebyexample.com/)
* [Cosigned](https://github.com/dlorenc/cosigned) Admission Control tool to check cointainer signatures
* [Security Checklist](https://github.com/Vinum-Security/kubernetes-security-checklist)
* [Access the API from a POD](https://kubernetes.io/docs/tasks/run-application/access-api-from-pod/)
* [How to view network namespaces](https://www.packetcoders.io/how-to-view-the-network-namespaces-in-kubernetes/)
* [How to configure security context for a pod](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/)
* [Seccomp and SELinux](https://jhrozek.wordpress.com/2021/05/25/prevent-cve-exploits-in-your-kubernetes-cluster-with-seccomp-and-selinux-profiles/amp/)
* [A guide to admission controllers](https://kubernetes.io/blog/2019/03/21/a-guide-to-kubernetes-admission-controllers/)
* [real world pentest for kubernetes](https://docs.google.com/presentation/d/1y6KGGT5Uw27cCgFMKiGv0NjRhq8YvjY_S9UG8s_TThg/edit#slide=id.g767a4f706d_0_116)
* [Network Policy Recipes](https://github.com/ahmetb/kubernetes-network-policy-recipes)
* [Kubernetes Operator 101](https://developers.redhat.com/articles/2021/06/11/kubernetes-operators-101-part-1-overview-and-key-features#operators_extend_kubernetes_to_automate_tasks)

## Bare Metal
* [Build Bare Metal with External Access & containerd](https://www.datapacket.com/blog/build-kubernetes-cluster)
* * [k8s on baremetal, flannel, metallb, coreos](https://www.marcolancini.it/2021/blog-kubernetes-lab-baremetal/)

## Post Exploit
* [C2](https://github.com/cyberark/kubesploit)
* [Post Initial access](https://medium.com/swlh/kubernetes-attack-path-part-2-post-initial-access-1e27aabda36d)
* [Cyberark guide](https://www.cyberark.com/resources/threat-research-blog/kubernetes-pentest-methodology-part-3)
* [Kubexploit](https://github.com/cyberark/kubesploit) Cyberark C2C tool


## Falco
* [Falco Project](https://falco.org/docs/)
* [Github](https://github.com/falcosecurity/falco)
* [Unveil malicious process with Falco](https://sysdig.com/blog/unveil-processes-falco-cloud/)
* [Using Falco to monitor outbound traffic for Pods in Kubernetes](https://www.rkatz.xyz/post/2021-04-16-falco-network-monitoring/)
* [Falco labs](https://falco.org/labs/)

## eBPF
* [Sidecarless Service Mesh](https://thenewstack.io/how-ebpf-streamlines-the-service-mesh/)
* [eBPF CO RE Reference Guide](https://nakryiko.com/posts/bpf-core-reference-guide/)

## Training
* [K8s simulator](https://github.com/kubernetes-simulator/simulator) runs k8s on aws and try different misconfiguration scenarios
* [K8s CTF](https://github.com/quarkslab/minik8s-ctf)
* [KubeCon 19 CTF](https://securekubernetes.com/)

## Helm
* [Exploring the security of Helm](https://engineering.bitnami.com/articles/helm-security.html)
## Etcd
* [How to modify etcd data directly](https://medium.com/flant-com/modifying-kubernetes-etcd-data-ed3d4bb42379)
* [Etcd security model](https://etcd.io/docs/v3.2/op-guide/security/)

## OPA
* [Top 5 k8s controls](https://blog.styra.com/blog/open-policy-agent-the-top-5-kubernetes-admission-control-policies)
* [Rego Unit Testing](https://blog.styra.com/blog/rego-unit-testing)
* [5 tips for the Rego language](https://www.fugue.co/blog/5-tips-for-using-the-rego-language-for-open-policy-agent-opa)
* [Kyverno](https://kyverno.io/)
* [Gatekeeper](https://github.com/open-policy-agent/gatekeeper)
* [CrossGuard - Pulumi's Policy as Code](https://www.pulumi.com/docs/guides/crossguard/)

## Multi-tenancy
* [MT with Hiearchical Namespaces](https://engineering.mercari.com/blog/entry/20210930-scaling-kubernetes-tenant-management-with-hierarchical-namespaces-controller/)
* [HNC](https://kubernetes.io/blog/2020/08/14/introducing-hierarchical-namespaces/)
* [MT workgroup presentation from KubeCon 19](https://static.sched.com/hosted_files/kccncna19/f7/kubecon-us-2019-mt-wg-deep-dive.pdf)


## tools
* [kubens kubectx](https://github.com/ahmetb/kubectx)
* [kubescape](https://github.com/armosec/kubescape)
Kubescape is the first open-source tool for testing if Kubernetes is deployed securely according to multiple frameworks: regulatory, customized company policies and DevSecOps best practices, such as the NSA-CISA and the MITRE ATT&CK® .
Kubescape scans K8s clusters, YAML files, and HELM charts, and detect misconfigurations and software vulnerabilities at early stages of the CI/CD pipeline and provides a risk score instantly and risk trends over time. Kubescape integrates natively with other DevOps tools, including Jenkins, CircleCI and Github workflows.
* [kubeaudit](https://github.com/Shopify/kubeaudit)


