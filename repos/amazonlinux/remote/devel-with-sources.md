## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:344ff4b1f4393a196c004008cbf7a6382a0b1350926be200d8aa2af2f1312d00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:674bb59511e82c8a1c2d258fdcfc7a53a179669a9ebc795d480cb9a4bf8b6168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.0 MB (483963823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea24a33c3438f88cbb312990d340600fcc8d3cc9e09e8a6b1f4f4bfc3bc4a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Jun 2022 22:19:29 GMT
ADD file:3cc0d880def73a3d39f2ec8da9923e1d9311fbb286f57f0354ee67812655e9cc in / 
# Thu, 30 Jun 2022 22:19:30 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 22:19:52 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-ed69c9a13dd98aac57da3e991b6dba1e11b4436b0fb28daca9344392622a25bc.tar.gz"     && echo "a952c3af116216571c43cf213c443310c15a0687256336904b5d98f9d7fe393d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:67cf6ceed7a460575d469086894c81433cddb3fe8a258514d0619c8d7a1f1ec6`  
		Last Modified: Sat, 25 Jun 2022 04:14:50 GMT  
		Size: 68.8 MB (68790038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b5f39cc6d3846d4fd81cba740c98bef113e094ecb3de3798b0f03411997e2`  
		Last Modified: Thu, 30 Jun 2022 22:21:01 GMT  
		Size: 415.2 MB (415173785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:241d31e6ceef519880bcdd19a203c569b2ca35e95483660b6dcd8aa38e12b4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.0 MB (481983659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748231095de7ce3c656cfc5664207291ea55b54726e4d61a7baf421e018b8f0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2022 17:40:06 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ad9d68b91be6ac7e867c110accb52ae5eea9db45924a4ca3d4d32cde09c2f0a.tar.gz"     && echo "70a0d5140609568de4135eb7074409d868e13d33b0fceeca6e06ba401cf47f70  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ebb50bc68ff064c69dba9f8a55ddeace2ba2b508f32cf6727a987d16d4c479`  
		Last Modified: Mon, 18 Jul 2022 17:41:26 GMT  
		Size: 414.5 MB (414506463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
