## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:f892875fea79052c1040f2d11cea7741e1ba393f2244461ca454437c27e4b73a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bf40faf1a0382a641adb6f2283e55f447ebb3f1c08a549e44605d73c273d873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81872567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b016e88894232f410e810df3f5be49026e4fa7b07bd71586291f883d8765965d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:03:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d3b7a8084f0f50ac1b09fe5b075dd39627cf2d5bf67659da7c41138cda7b67`  
		Last Modified: Tue, 07 Jun 2022 02:23:53 GMT  
		Size: 6.6 MB (6644325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd97ebd2067d1a4bead88f69c0cdcc55b5a30fce0416079338359fc29d2bb4a8`  
		Last Modified: Tue, 07 Jun 2022 02:23:52 GMT  
		Size: 3.0 MB (3026631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41735452950ad5e0d9fa366c8a9bffb525845e2594e2a650de86b24b125d7dae`  
		Last Modified: Tue, 07 Jun 2022 02:24:10 GMT  
		Size: 45.5 MB (45489985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6ea45fe8b9155b916f1a9f98e0191bff337683e724192b3cde269f098779507f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71290191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44369f2f504ae91e0fe1cea0e41d0ad97e845b3ee95bdf72a6ec9612dadb3400`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:25 GMT
ADD file:9604e3641a386ec134596dd717862c2386c1b90009c0646b1773930f98949d9c in / 
# Fri, 29 Apr 2022 22:58:26 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:23:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:24:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:24:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03ca5b55b2bdc3c68d23c18a88c099e2015c6bdcef6e3c43ca0bfb6aea0b032a`  
		Last Modified: Fri, 29 Apr 2022 23:02:31 GMT  
		Size: 22.3 MB (22300451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a73dc6c378126504521857c1f5b32849b1a6f778ad3be2ae05e85a203b1679b`  
		Last Modified: Fri, 29 Apr 2022 23:44:06 GMT  
		Size: 5.7 MB (5713646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882d05cf8d5563b9acf2592cd89c94aa437d95d40a15b9f67c62ac3754b6c395`  
		Last Modified: Fri, 29 Apr 2022 23:44:03 GMT  
		Size: 2.6 MB (2584817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d3bf1f68a620a53fd64d163d712d07fb918d0e130f47c4b6d7c88fd12ab8d9`  
		Last Modified: Fri, 29 Apr 2022 23:44:49 GMT  
		Size: 40.7 MB (40691277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a98e25d55904a28a4d21cdb10eb7be2b73f38afaba5918a87891d78d0072b905
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75679924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf8bb03cd2fe608dbf3393722f9e47a06ab462000a486ceacba9dfe4fa28460`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:14:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:14:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:15:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60798d5be0c4fe2a3b108def28399e64d3473055149c3b22fa62e931213239e4`  
		Last Modified: Fri, 29 Apr 2022 23:23:40 GMT  
		Size: 6.1 MB (6082989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbd896531eeca6d8cc62526013f972fbe235bd8cf006d5bc34901a7cfbb7ff8`  
		Last Modified: Fri, 29 Apr 2022 23:23:40 GMT  
		Size: 2.6 MB (2570403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1586d1e5563ecd2e705ff77d7fab291b0fff2765b68e0f69e0e1f9ead6e3a99`  
		Last Modified: Fri, 29 Apr 2022 23:23:58 GMT  
		Size: 43.3 MB (43291443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:793a6bc9985a95f4163013ec314faf81faa56dcd5f78788bf9e9b2e6193cbb76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84224105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a8688ce5e30326b8459606b191a11c50042c71428bb87b48145b29f294f42b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 21:18:54 GMT
ADD file:c1118975f50d6835777043d4b807b4fcf30db0151d1e7659e077e9e33c4ea7c7 in / 
# Mon, 06 Jun 2022 21:18:54 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 21:45:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 21:45:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jun 2022 21:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1408ae6e2634d0ef0a2f110363deef0fdf35ee2958852f9d20b92b57495a9fb7`  
		Last Modified: Mon, 06 Jun 2022 21:19:41 GMT  
		Size: 27.2 MB (27165461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9997a51874c52f806343d9609c83d010ef99ca07d34fe33a866c72416728b1`  
		Last Modified: Mon, 06 Jun 2022 21:51:19 GMT  
		Size: 6.9 MB (6931382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5698bd6c395573f235a617e94df59b4d8e7c54b59065059267f6aa81e685a7ea`  
		Last Modified: Mon, 06 Jun 2022 21:51:17 GMT  
		Size: 3.0 MB (3041855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6196e18ef02eb07ef39a9b49d2c47f9c40556ac3696ef8742efa88473ed99eca`  
		Last Modified: Mon, 06 Jun 2022 21:51:36 GMT  
		Size: 47.1 MB (47085407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dbb3e2b7c29fc797c7c1e85d4180c1488bd27054bed04a935a05acba182ae930
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94961964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bcd5673d99377e620b31f265e1d645b9f67f8c2c542b09bcbf0eb1b5addb8b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:55:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:56:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d7ea724107cf3fb9dca027e66737cbba5da37d5b111c18bcbb1bc195ac8a17`  
		Last Modified: Sat, 30 Apr 2022 00:24:56 GMT  
		Size: 7.1 MB (7057904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328e725fac94afb6fc3c04f131827c3480065a1100acf76b2a2fd9c38ec61bba`  
		Last Modified: Sat, 30 Apr 2022 00:24:55 GMT  
		Size: 3.7 MB (3719532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55476303bf21961b37a56b5ff8894215db5d4c0794c3d68bdb6f6227eab57df2`  
		Last Modified: Sat, 30 Apr 2022 00:25:19 GMT  
		Size: 53.7 MB (53741345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9354c20468051c74cedb8b7bec1260fc31b926db368407685c214e2c05efceb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79711977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d13883041199e66098589606325a450c451cd74dccd4bc955f57d79a0e131f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:09:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:09:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad71b6aca98ce06e987b76f0d613b62e64dffb408abae9b95415af2f7416c46`  
		Last Modified: Fri, 29 Apr 2022 23:18:34 GMT  
		Size: 6.3 MB (6333148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f9a7ec2a119d06fe06667d3a801ec5234c7611b1d83200aa930c8c69fc614`  
		Last Modified: Fri, 29 Apr 2022 23:18:34 GMT  
		Size: 3.0 MB (2975210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa5c603c5ee07210bbaee5eff68c14fb9b0a6d3e78d239fff4de9d445cd34a4`  
		Last Modified: Fri, 29 Apr 2022 23:18:48 GMT  
		Size: 45.0 MB (45037791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
