## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:4e0401bf1ba398dfbd820acc7da7a7b48bebe090d46f525f29b42f1e54334bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8c474a27635a29ce1f6daffda32528a0aa48b6f589ecf88490b158f33a571f15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82127733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b46a0d94344b399c5d7604309d08fcd4a61f68a8911fd92690bd5f4a46d9c8e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 05:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 05:37:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 05:37:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbd9104be902889dc21019a0f5023f798f3d4659871b7eff4e60ea6f1496df08`  
		Last Modified: Thu, 16 Mar 2023 05:45:13 GMT  
		Size: 27.5 MB (27533123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f926546ac77ef389dea10f2f48a9435499b9fd85ce007f054787873fba3ba820`  
		Last Modified: Thu, 16 Mar 2023 05:45:10 GMT  
		Size: 6.7 MB (6653872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e02fdac0efdc0f5d71c45d6ab71b8cf2421156adfbe3dd6673c198b60f5e696`  
		Last Modified: Thu, 16 Mar 2023 05:45:09 GMT  
		Size: 3.7 MB (3689653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57775961ac4b5f4df9ba21c9a454eec60eced52106a9c3c6480abe04fd31e975`  
		Last Modified: Thu, 16 Mar 2023 05:45:29 GMT  
		Size: 44.3 MB (44251085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6b08244e2bc4db9fd4a22095b42d9044de738c27f0c4f78a9fd1303fb5e9459e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83364676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad34d38cd21a977e6a4b1485518ff8873988b314b13cb4796e11b2ed4ec4d693`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:01:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:01:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:02:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2e2ff6a76c080ab34fadea2f47efdf4e1606b1482ed2e4597e51810a467b28a`  
		Last Modified: Thu, 16 Mar 2023 04:11:42 GMT  
		Size: 25.4 MB (25359548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003fc5922aae3f4274356fca42181568c983c95440b266598d0a8b3307f981b3`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 5.8 MB (5819049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f573392ff6ba3d538b9dd78eaac78c3a48a8719f2c3a366e5031c24433553af7`  
		Last Modified: Thu, 16 Mar 2023 04:11:39 GMT  
		Size: 3.9 MB (3850947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e5edf4553807d09a5e079189ad8abe94fa20ac8d3b91a1fdee74ffbbfc465a`  
		Last Modified: Thu, 16 Mar 2023 04:12:00 GMT  
		Size: 48.3 MB (48335132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7718090c669d397351860cb0345fd87226c3f44bfc63156d13b88ee8b6bb13c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81133371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794f72335c8bb0cbfaa191b6c8873dca8c9aeca030e74c1f1e6e88e9df6cfe91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:17:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 04:17:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bd94ab779df0c538759342d8eef230b315e98979bcac4604e94fb874397461b`  
		Last Modified: Thu, 16 Mar 2023 04:25:04 GMT  
		Size: 26.9 MB (26945660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8402fa00c99b6f8233d0c6452e59cfe2742b9b2c9f44a504aaa45a0516cd3`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 6.5 MB (6484575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa45039d5b2736a9624493cbbbf9200c134de7ddb8696ce87c68dad417e12f4`  
		Last Modified: Thu, 16 Mar 2023 04:25:01 GMT  
		Size: 3.6 MB (3648517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5195e2054b68f924f77b2db71706b518fdc87c9c6f3d900adad8e6eec601fb`  
		Last Modified: Thu, 16 Mar 2023 04:25:18 GMT  
		Size: 44.1 MB (44054619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:80776e57275eac4ab14959cc2eb0aa5c39dfbc1eac936218d2bd4714c32b6d34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92937683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86884dca514275133e923ec8f78e2785269d5ed21433f44077b1e44c33e5751b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 03:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c13086b2cdc797d6ae8ae49964c3990abf6b026e7f643db84a65b7f084366f08`  
		Last Modified: Thu, 16 Mar 2023 03:53:59 GMT  
		Size: 32.0 MB (31970021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb512502a00877ef190b1815b85439c23acfccd37a17990ec798b2bea4e21069`  
		Last Modified: Thu, 16 Mar 2023 03:53:49 GMT  
		Size: 7.6 MB (7632987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c926d392a0489ac95be096f121aa71205ac931a151fc7c4564fc57444078c1fd`  
		Last Modified: Thu, 16 Mar 2023 03:53:48 GMT  
		Size: 4.4 MB (4408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2857f7a011d6755514a89958db979d33059396ce8ea89c6552489bef9035282b`  
		Last Modified: Thu, 16 Mar 2023 03:54:23 GMT  
		Size: 48.9 MB (48926165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:be8e1571ea2945b768f155c85a9fc4d617a62103e27b12291a1b9e88c5ae2f53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80254144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad371214c349f4a458439e817f999971228fed0bcf6aceaccbb08508cf9c8a0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:56:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Mar 2023 01:56:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:413472b726c3207e3bafacfb65a3db7c0c8692445502e7d2ad70b1585e534841`  
		Last Modified: Thu, 16 Mar 2023 02:04:26 GMT  
		Size: 26.2 MB (26162786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef961f5d29313e42026cc5111865e26af7782293f64f5eca11172750d63f804`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 6.3 MB (6335431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b09797bd3d78e6694a4d023216c32e3665a913d5dcd639c47a00674aa9bd5f`  
		Last Modified: Thu, 16 Mar 2023 02:04:24 GMT  
		Size: 3.7 MB (3674242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac168459f3e70bf00dbc80bd6a3cca0005c0e36d3ecf7fd0ae2395921677c5`  
		Last Modified: Thu, 16 Mar 2023 02:04:40 GMT  
		Size: 44.1 MB (44081685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
