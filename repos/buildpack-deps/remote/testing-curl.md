## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:4f6f0ec702bb090de2b521849f99d085008716b4ee2f4251abc9c72fb07fdadc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:35e8f0e6033a01ce63f0c950d2b0fd73282a3f5843082d1909336c8482f90af9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70212190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbcf63b251394e7e435345f3714d2982e4ec6a9dceceaa1d5fd5a062eb08ac0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:19:50 GMT
ADD file:3785e6fc0adaed3cfee77ab7dd0756681492573e3553e88b5225fc14d56562d1 in / 
# Thu, 23 Apr 2020 00:19:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:48:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:48:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:91028a6d2ef79dd78d620852cfc6dcda63ffb7301b4a1e87108edd2e9e499625`  
		Last Modified: Thu, 23 Apr 2020 00:24:32 GMT  
		Size: 52.0 MB (51981200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831d9a74fb2992a6446c6eea6a71db00f998b765785b1f37a56464bd43408d09`  
		Last Modified: Thu, 23 Apr 2020 01:01:52 GMT  
		Size: 7.9 MB (7933113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f1160e3e672fe333aee8b37fb0e11661c02ab6ee62a7e276efe6b6f42271d9`  
		Last Modified: Thu, 23 Apr 2020 01:01:53 GMT  
		Size: 10.3 MB (10297877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f035169e1aa3075e61c54ab9eeec0ec229d13fdcadca1b86730a1fc22ef8b7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67459015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23ddb1f41691c7584d0bec633454faa35cdb0d5d334e34c9008d69039eae7494`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:06 GMT
ADD file:5be2178df3e21d9545818a91f7ad742ffb521f470db4ffb6f2b4b8e5381d0427 in / 
# Thu, 23 Apr 2020 00:51:09 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:21:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:21:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07d9742943d725059b0958dfff17760efe7b78df3e20635aab1c80cecf4d1375`  
		Last Modified: Thu, 23 Apr 2020 00:58:41 GMT  
		Size: 49.9 MB (49935576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6804de3a0793db8acc856e22cd4ad64c904053890cc2d87651cc6e49fe02b38`  
		Last Modified: Thu, 23 Apr 2020 01:47:02 GMT  
		Size: 7.5 MB (7514841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a05b6f98e0c3895a7e4e4a0bc79d3ae0e9198c978423547432797212d3c83`  
		Last Modified: Thu, 23 Apr 2020 01:47:01 GMT  
		Size: 10.0 MB (10008598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a2be7729ce0ac6f16827bb0570d09f80afa6f39e02005909027e6e6253f9766
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64574658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89dbeb4c8a3e30f92b7011abf39b3c47b1639796275a482139e7ef8abc11d2a6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:58:05 GMT
ADD file:353f89e64e5475f2d99be1c5e0eaa80d5aeb89e02c274ba507df4def8f7ccc8a in / 
# Thu, 16 Apr 2020 00:58:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:33:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a287a7fa81e293e147ba52c36ae34e643e975ef88ebe9a6f226a048dbb7ee9fa`  
		Last Modified: Thu, 16 Apr 2020 01:08:03 GMT  
		Size: 47.6 MB (47646389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47358f6975165f42a9cd9b867f0d03e95a00b52627d5e833781a9eb45eca84cc`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 7.3 MB (7255347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376a0294fac4492ac4a3da9b92cdf02ee87e6bfd519ee19fb996c5db96da33ae`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 9.7 MB (9672922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c95b0c0060cfebb357deb8bbc453c3c89a27c72df8c65ee14e22dd9347220b53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69003377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a31d465c7351837ff159573df28586e631e6b0deddb272161852a871c0de97`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:40:12 GMT
ADD file:27c25cdd69090f4b15f9f2f4a147879d1d7510b7b2f8c231a92fc74832325413 in / 
# Thu, 16 Apr 2020 02:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6c6bfde49c5261423574a9f9bc077a0cd0057775509f9d9e061556a16b84e1d7`  
		Last Modified: Thu, 16 Apr 2020 02:48:01 GMT  
		Size: 50.9 MB (50901465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c744c6854f291e264392cb87f79c4675b05d5383ca93df9f5b4be8f447aba3a7`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 7.8 MB (7807688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0a53c53b80bd91c029938e07ae8fb49e75ae1d45620212fa6fc041e97f5750`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 10.3 MB (10294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b46cf626b828ef9baff3f7897729f4256351086e25dd7282aacd0b6ed7c518f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71892709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:381908f07281083e4b4bf39628b55a05ff23c53221c1461df5bd8d60900eba72`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:38:53 GMT
ADD file:8842691c10d9cacf5f52fd9fdb3b0f3a9a5ed4212d9f2ab558d17e5efd9a758f in / 
# Thu, 23 Apr 2020 00:38:53 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:39:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:39:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0bf245c0cdf57ebbfbaf49d796259272bf11094420c0537965c4d322d66b4e55`  
		Last Modified: Thu, 23 Apr 2020 00:43:49 GMT  
		Size: 53.1 MB (53124775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3766da29a92d4e7819901f2cd3fd92af428a41fa1efecc94dadb17f8bd6e6d`  
		Last Modified: Thu, 23 Apr 2020 01:58:36 GMT  
		Size: 8.1 MB (8110585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6891810791eccf312b55bd366b84147115acf3dc533fd07cc22ed2ce3dd771b1`  
		Last Modified: Thu, 23 Apr 2020 01:58:36 GMT  
		Size: 10.7 MB (10657349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0746af610bd122b56a89c0777a7e10784799b828900c81e323c0f7b22fdf49c5
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68479319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347c5de411e59953b80101fda57965d324b57e7ca2c3c48f8bb8bbdb492ecb78`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:08:38 GMT
ADD file:01a8dba65674c16c3bae58d6e4cf7693a0616ee5efc5495e513ba4454fdaa97b in / 
# Thu, 23 Apr 2020 00:08:39 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:46:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:47:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1ccb563ff5d3d7b0b42a931c0aef1761ab04927c47d729b21ae98a7788ef6af2`  
		Last Modified: Thu, 23 Apr 2020 00:15:41 GMT  
		Size: 50.7 MB (50694211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc1749bc72a1c4ea633b9f43ee46469e3c9b9fca82f799a577fbddf0a0295d`  
		Last Modified: Thu, 23 Apr 2020 01:06:10 GMT  
		Size: 7.5 MB (7460628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed375c9815816af90643e25af4799e3d5c112ac07bc80b13cc5976a394275f53`  
		Last Modified: Thu, 23 Apr 2020 01:06:11 GMT  
		Size: 10.3 MB (10324480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:62dfd15aed39d27f89557842e3827bdaeff71805c588dad9ee2eef3412c7d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75187683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd193e42bc6cd241e977a911250256e07831d41e980728374a718edbdc34d450`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:32:36 GMT
ADD file:93aa541f8747875de57b6848e6e2df3b2ae7cdc03dcee5489fcfc1bbf45c4920 in / 
# Thu, 23 Apr 2020 00:32:41 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:40:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:23044bc1c77de90086fe2791c49374dbad1ff9af6b3b4dde5f4d46fc92e6a936`  
		Last Modified: Thu, 23 Apr 2020 00:48:13 GMT  
		Size: 55.9 MB (55855771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b244e406f7e60e72181a1fc05e23631e55e349385a03256c692ed685e75d61`  
		Last Modified: Thu, 23 Apr 2020 02:21:35 GMT  
		Size: 8.4 MB (8356173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bb62044b675b46ae88158a62f5e93b36bed0459b07a8e50881cd48a7d4070e`  
		Last Modified: Thu, 23 Apr 2020 02:21:35 GMT  
		Size: 11.0 MB (10975739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a13ddb649bf77f0944b0f7589c1e08b71402abe6597a3e6ee9cadd5883289a0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68364633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1769068678f5a7c2f3373dcb187e43c21cb1543b67fb768cc22855d98d835f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:50:53 GMT
ADD file:f056a549a046e95dc913639e6f66f03822a0253c29e80ca83bfec0ad17ce61a0 in / 
# Thu, 23 Apr 2020 00:50:56 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:52:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:52:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dea34220fb3629088500931b5a9b5f42e8310437035ae5d967501a1b59801c6b`  
		Last Modified: Thu, 23 Apr 2020 00:55:22 GMT  
		Size: 50.6 MB (50579994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a059087ed5236381609d7860683f56075adbd498ce096fd21827cb24329124a7`  
		Last Modified: Thu, 23 Apr 2020 02:06:32 GMT  
		Size: 7.6 MB (7600648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb9b52f51c99a0897c6de164eb2fea990a9c6433eb44a6d979eed78270fb2b7`  
		Last Modified: Thu, 23 Apr 2020 02:06:33 GMT  
		Size: 10.2 MB (10183991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
