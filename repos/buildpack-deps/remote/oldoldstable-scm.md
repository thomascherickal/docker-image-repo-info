## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:6029c1c3544280573274d9be6f9cdff5b647ac8d8dc86da8fb3140a965e748b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:17a261a61287529e5ed1936477a24c98c41119d5b65ca5c10a0689175da99677
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115274891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69d61fe47c32123a4844169e449808441f139cf10af1e504267931c4a7d60c6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:45 GMT
ADD file:545fa4a7e3efbc02fd93b103a922af1496dafa1358953302d1e9112772a46c6d in / 
# Thu, 23 Apr 2020 00:20:45 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:53:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:53:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 00:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4cbd35197708a9e2a08a980f6184996202108f81f5a0a2639bba1f4e070c56b`  
		Last Modified: Thu, 23 Apr 2020 00:25:23 GMT  
		Size: 54.4 MB (54390774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cc73abfb4303b455fc8d3efa21117aeacb8235e3eb27426aca3f86f2d09e6a`  
		Last Modified: Thu, 23 Apr 2020 01:03:49 GMT  
		Size: 17.5 MB (17545895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e28fdf8450ab7cca43fd94de3108f4c22436aca0ae9c3097446d26e5a88cd2`  
		Last Modified: Thu, 23 Apr 2020 01:04:01 GMT  
		Size: 43.3 MB (43338222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e5079aa0a6d416f9cdc7d3d6183cfdf4ed221b5f2d9f3bdf047488c265d9c7e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110779381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8919e595cbaf1940a317d1187e954b8355350638fb913d7984eb6a117a9a120c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:40 GMT
ADD file:ad74a04687587d6f1c99337a488cf1940e8c2858ba05d7333e41b00f97d7a9a9 in / 
# Thu, 23 Apr 2020 00:52:42 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:30:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:30:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 01:32:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:391f9df5907e432e21493cb2cf9b5973be82a7b817b5bf35de533d6058b40a88`  
		Last Modified: Thu, 23 Apr 2020 01:00:16 GMT  
		Size: 52.6 MB (52581465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b60d367079b97ebb9773382f8436388d39b7de3ad8462b27be00f053a25185`  
		Last Modified: Thu, 23 Apr 2020 01:50:32 GMT  
		Size: 17.0 MB (17037185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a739223f8202ea692eff094c0dbd380e1cca108fd824942669c6af574570ef9`  
		Last Modified: Thu, 23 Apr 2020 01:51:00 GMT  
		Size: 41.2 MB (41160731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:17718cb62a06b3a8f013c386540dea1a4d55e356ec4149367435890bba15476e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106805072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f62c28dae6bca9ce485c37d627d56ba163f19718af5d8cd9ef14fc3e9d7d375`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:00:13 GMT
ADD file:0b08b600835a16058b725946cb7ae338fea6a14cf6998584f9728d2c62324f1e in / 
# Thu, 16 Apr 2020 01:00:16 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:44:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc084eacfbe394e053f99559ca63f9d660d60dad0b70a31347e5088af534b2e9`  
		Last Modified: Thu, 16 Apr 2020 01:09:20 GMT  
		Size: 50.3 MB (50304312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2753eba5d276059ffd460d19c6e651040079c4a18c7d6a93682bef3e285c0b9`  
		Last Modified: Thu, 16 Apr 2020 01:58:21 GMT  
		Size: 16.7 MB (16723352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff41b20f0ffb69690b5b8efa517a6db82e30df6bbb8a1ba31dda7369f437c9a`  
		Last Modified: Thu, 16 Apr 2020 01:58:41 GMT  
		Size: 39.8 MB (39777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8a4a7f21e279f9807e3a7baa92b8ee0e531fb0097efe5cfc7457dcaf3c42f518
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118443623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aafb7ac93b8b8004b368dc52d2e8de68ef9d0054023a2e7c093ad6907e4fa22a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:50 GMT
ADD file:5a51343ededbfe4c380e189c99b1136cd1143a41ea66cee7cbdc3b9b523ac86a in / 
# Thu, 23 Apr 2020 00:39:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:46:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:46:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 01:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46bce17837ebb6f15aa73ef7b5c4ce1f32c9108c2dc291e4af9944c5bb7130e9`  
		Last Modified: Thu, 23 Apr 2020 00:44:51 GMT  
		Size: 54.6 MB (54607867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64d5974b96b34da72142a0155b10ccf50819700a2fd7d3faf98329ad3808cf`  
		Last Modified: Thu, 23 Apr 2020 02:01:40 GMT  
		Size: 19.9 MB (19855827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18254c800e99a51f674488ec0f9688b8f952adcf63222e9648847baefaef31cb`  
		Last Modified: Thu, 23 Apr 2020 02:01:59 GMT  
		Size: 44.0 MB (43979929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
