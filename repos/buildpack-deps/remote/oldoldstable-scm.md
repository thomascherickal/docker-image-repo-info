## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:466de73a8908d5c8a0d5c0b90fb16f9bedd0cca685a7b3c9d0f16c57e8898bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a2126d54b9400cf310087de8f68f54f5c3a1d93cd1af58727afed59d7aad6828
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115271458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d781dd9c1478a52511916e446959fd6856ae8fa6fd1888cef508c095663c1e07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:20:54 GMT
ADD file:63fdbdcc45a46a993700d252a6f9652db8ab25688daa8bbceaed90b73b2654cf in / 
# Wed, 13 May 2020 21:20:55 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:31:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:31:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc53e9ecf017dd9c8c8ba0c497d08e2d7c04f4a57dfce491d755cb37613f58a`  
		Last Modified: Wed, 13 May 2020 21:26:59 GMT  
		Size: 54.4 MB (54390659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cedf82ca715cf8b41a88bfb26ad7225ae77537b5999a2f9a3ed1c430b19bc98d`  
		Last Modified: Wed, 13 May 2020 22:46:29 GMT  
		Size: 17.5 MB (17546015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb3decbe8c76a4818f476de7732333bc00cdb7c3a75887374dd6d6450202e76`  
		Last Modified: Wed, 13 May 2020 22:46:46 GMT  
		Size: 43.3 MB (43334784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fdfee46caba135a7b1f90ba1986cf02df8382623cdaff16cbc5eef874632b619
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110774823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9463c382fbaa33cebca4cd4667da087e96ec4801cd4ee36e892af53b338a3a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:50:39 GMT
ADD file:621441e8cf0bd677ecfb646d7c54417894fedb89b8b03295c25a4ea0ebefbaf3 in / 
# Wed, 13 May 2020 21:50:42 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:37:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:37:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:39:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:535d6dc5159c1d8f20f2d1a86a8433d89941a1933de7a6930246eef7811be611`  
		Last Modified: Wed, 13 May 2020 21:59:45 GMT  
		Size: 52.6 MB (52581076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73189ba1a9ac8eb7f3c4a34630c9eacf6ef34fde77675eed4b21857d50d7a3e`  
		Last Modified: Wed, 13 May 2020 22:56:53 GMT  
		Size: 17.0 MB (17037185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7802ce38e2c324b7cc2c2773a4bdda1c88367f6d1823d6807df3c2d00a9ce`  
		Last Modified: Wed, 13 May 2020 22:57:15 GMT  
		Size: 41.2 MB (41156562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9358379376f157069fe774887f60e8122c24838705c5b643871b05a182297893
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106806991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23357c3adba65571c436c71aec05501e81ee4c08d002bea66729e03caa8716b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:14:33 GMT
ADD file:c27f6b9fb44500f82ed124d104a7cab3fed859c9cca4bbd0be2c77f3db082fa2 in / 
# Wed, 13 May 2020 21:14:36 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:01:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:02:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fb6d2bc03cec7adf4767dfcb7ac7a2740b65bd196c1071b809768619b12a0d4`  
		Last Modified: Wed, 13 May 2020 21:25:14 GMT  
		Size: 50.3 MB (50304251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32375e9074306a5d2a3cec4864995cabaaefd56b21eace9822bfed9dc2169d1`  
		Last Modified: Thu, 14 May 2020 00:21:41 GMT  
		Size: 16.7 MB (16723434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5c0933ac15f5a3d4ea8317d3ccec86327de17987d9262818b5c832440327fe`  
		Last Modified: Thu, 14 May 2020 00:22:01 GMT  
		Size: 39.8 MB (39779306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:332a5ff4fcc353cfde372bb4cbf030a946139f2b4187343429e6d437d80ba8ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118453620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0589ac2e3f89b9c02e6f258961ff40afe9b1c77296020cb6f456d0c6d81db4bc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:39:42 GMT
ADD file:c41a548ee5a118fc5c8efefd084aca1f4629d3f462ed9d1bc5ddc568db89b0d2 in / 
# Wed, 13 May 2020 21:39:43 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:46:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:46:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:49:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ecac86f3144ef4bfa8747d585400212884f0a7fb2a71c1eb54483af30ca0449`  
		Last Modified: Wed, 13 May 2020 21:46:50 GMT  
		Size: 54.6 MB (54607906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f067623bec4e0179ef9af3ffa91e7197a238ad23d31f534e3ee78a83f4547351`  
		Last Modified: Thu, 14 May 2020 00:03:33 GMT  
		Size: 19.9 MB (19855823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716e17289a4b0c8f800234eeecfdaac67fe336e111d4cfefafa845d074a0c65`  
		Last Modified: Thu, 14 May 2020 00:04:00 GMT  
		Size: 44.0 MB (43989891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
