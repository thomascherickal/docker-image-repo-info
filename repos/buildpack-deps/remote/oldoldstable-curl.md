## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:d256f20730b7c16fc0ce58a3474655955a2b4ac252d27b3d382247107e633c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2300cfa42872270c1cfdebe01b3801ef884a8bdee78fdfa6b699ef92b528f01a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71936669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f24b7e1b7e6a5232315d05c509f9251f5e4e5838dad44ab08814d9ba689e08`
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

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e591d51d474fdccd32d8f3e001c2f206028eb0cf0a1ca0d80cb6fad4f25e02a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69618650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69c4c2cb4a7ef2cd19fd0753c8c1d06881822b6fcb66f4d6e95bbdd835331e7`
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

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f31c39b5fd7515bf0db51301f4f19eb199fe1bec9afe07fe7d75ad0e0fb38079
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67027664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da1b237044f964087658b9d80398029330908ef6d82ebddc93f9777eaf2bd4c`
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

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:23d6474aa06fbe8fc38ea9c4349fd4184e8cde5a2355023a520848948363d326
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74463694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6ce21730f6557207d3c258ab45ab1ae3f3d9323d72971589f13392980d2e5a`
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
