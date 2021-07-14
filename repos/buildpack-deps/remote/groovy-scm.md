## `buildpack-deps:groovy-scm`

```console
$ docker pull buildpack-deps@sha256:61892ea350994f807083c75321a15c1bdde4335e7b0cc58de81e684f633bfa80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:def105177e3e1a7bdfa9835074c343e7301f94b4fcc412dfbee0450a25e956bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95887159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b43365edd2e72fd33c666112ac758c6ce72234e04e30e41069863743617920`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:31:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a187db8c68613bb56c28a4f1c711d24248f3be342e2b2e98c6d162d37b9286c2`  
		Last Modified: Tue, 13 Jul 2021 23:46:40 GMT  
		Size: 5.4 MB (5404370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd548091a4b68a282f178caf8f237861b35ad281d3b8408ad339223262a181`  
		Last Modified: Tue, 13 Jul 2021 23:46:39 GMT  
		Size: 3.7 MB (3663412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9b58b1633551f88d8de925d153919fb1ff355ddf5ec050f245a0bb38d85093`  
		Last Modified: Tue, 13 Jul 2021 23:47:00 GMT  
		Size: 55.5 MB (55477811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e8b412072b1e627f2baa5a6472b1cff517a4826df277dd2c0ea9c8f31b013920
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84595342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a09d99d4493d757bafb5ca8aa3bc8862809476fb2879ccef64e8788f65852a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:33 GMT
ADD file:80b5f21ffac906a8416f39204cb526afaf64f15559123cb3a8fb311e312a703f in / 
# Tue, 13 Jul 2021 23:21:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:55:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 01:56:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ad80ac50e31c20115b0366841c81a92d1916a7f2113255fe1125324250475e7`  
		Last Modified: Tue, 13 Jul 2021 23:26:54 GMT  
		Size: 26.3 MB (26312397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87836ed84bb5f0e1d7b61439e8458826efce0a52158d32f928c2efc41367ac4`  
		Last Modified: Wed, 14 Jul 2021 02:19:01 GMT  
		Size: 4.8 MB (4840704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a0657bf22de96a1925b7c31d415ed9eff49f3b00971444459ee9b696832ef`  
		Last Modified: Wed, 14 Jul 2021 02:18:59 GMT  
		Size: 3.1 MB (3140633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e419af2ccab0c7223c92ce4cd8deaa2cdea7e08e02b9636ce5f7193b06162f6d`  
		Last Modified: Wed, 14 Jul 2021 02:19:51 GMT  
		Size: 50.3 MB (50301608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5be35c06c05733c4335bd77739c96f0be701494ccd458d039e05270857f07ed3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94356279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:605327ad5caa5567c7450f6c9f7013e80cbace8ffe58e1a3a1869cffa29d6c5f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:34 GMT
ADD file:8fe3c90118921d388c31ca28a21ff713dd718197e04654c6e0b7a09435f5287d in / 
# Tue, 13 Jul 2021 23:01:35 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:53:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:53:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3da8512ba050381848a454507530b9a467063e06b22a25eddc01311dbdf35301`  
		Last Modified: Tue, 13 Jul 2021 23:03:58 GMT  
		Size: 29.9 MB (29877377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055ca1e90e094916911d8a92553fa0422dd53e6e43fed33614623edae8ca22c9`  
		Last Modified: Wed, 14 Jul 2021 00:02:57 GMT  
		Size: 5.4 MB (5372770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955901556b2298b0b4c51d2c60f4312309d050d4152c6e9cbf8a27cc02b9357d`  
		Last Modified: Wed, 14 Jul 2021 00:02:57 GMT  
		Size: 3.6 MB (3635077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45f76631624206ef01b5b63f98f3e506bcaedcefd4804326ee884f3b4dcb53`  
		Last Modified: Wed, 14 Jul 2021 00:03:19 GMT  
		Size: 55.5 MB (55471055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f0fe9add7985d92c6808484c0efde2028bb6d2cd5ba709fcc78782419790e4c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110865638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99fe74ca30bda86d174201abfcea257f1b7eb65bc2052b87edbc744789da97a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:32 GMT
ADD file:5b3e0dae91824102eb438ea2d8c1f1190ffcaa623f93c4e0e96004e1098cacb7 in / 
# Thu, 17 Jun 2021 23:25:40 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 00:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 00:55:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 26 Jun 2021 01:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f3c6e346cb79378eaa11a81268da2aa9fb480ab376c060d5cb48380f3754b37`  
		Last Modified: Thu, 17 Jun 2021 23:29:02 GMT  
		Size: 36.6 MB (36561549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf3088338753aedc77d485ca99aac63dc4bc2bb88f766d066e9a92385a5ce31`  
		Last Modified: Sat, 26 Jun 2021 02:18:29 GMT  
		Size: 6.0 MB (6040721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432b10ec98757d1b5f49aeaf3288c25955f16a32ac6a74b66cd627510ceb29c6`  
		Last Modified: Sat, 26 Jun 2021 02:18:24 GMT  
		Size: 4.5 MB (4521737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e5cbe30721952aa4eba97d67389e491f056e856cefb4754ddb778c7d02cd3b`  
		Last Modified: Sat, 26 Jun 2021 02:20:04 GMT  
		Size: 63.7 MB (63741631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5e5824836a5642631bf4014253baa2dfde359925a2e4906bda482838652a92f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (102031129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21a628785ee3c037f3cddb4f549a156c7b315aaf4a700e8d07cf8af662dfdd64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:46 GMT
ADD file:02a1c687ec9417cdf601518590b3a21fe31a0ebd2cdeb9bc63792512b95de989 in / 
# Tue, 13 Jul 2021 22:53:49 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:44:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:412af85569a706b682c00eeeaf32aeacbe1a5df158e5b67ddff07842b7ba3080`  
		Last Modified: Tue, 13 Jul 2021 22:56:02 GMT  
		Size: 31.6 MB (31577497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ed9de239c255124abaa7cd10a81a3e295829e47c8f990a740c9de4638d328e`  
		Last Modified: Tue, 13 Jul 2021 23:52:18 GMT  
		Size: 5.6 MB (5629821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612d9fc542d056eb20ee90480c45cf9b38afd821365ceecc6ce517204872126`  
		Last Modified: Tue, 13 Jul 2021 23:52:17 GMT  
		Size: 4.2 MB (4156765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9768d4aa6766f231a99a9bffe76e6867dd9a5d208327f84e9e8997bf8989ad81`  
		Last Modified: Tue, 13 Jul 2021 23:52:34 GMT  
		Size: 60.7 MB (60667046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
