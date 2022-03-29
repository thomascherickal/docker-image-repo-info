## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:5734675e64c443882d799a2bb7cdaac67201fcb72fa4aa7a19642cddb05b3771
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
$ docker pull buildpack-deps@sha256:9e03562f59f09021b092b05b271489e61384d9c9d632b7b7a9c6f264ea5227df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81857215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15d0efa36888a8bb87f0a1c59e4d7eee3ba5effcb9bdacab8d701c5990f27d2f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:38:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:38:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 06:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ef3f2ac944896d21cb971be4b7ec028ac826242cd0451df060b0b4412b92f`  
		Last Modified: Fri, 18 Mar 2022 07:08:55 GMT  
		Size: 6.6 MB (6641832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f005ad8fda9d934f3bab809914d7cf447e57835543823c59da423475b8f58`  
		Last Modified: Fri, 18 Mar 2022 07:08:54 GMT  
		Size: 3.0 MB (3022305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bdf22b8f5807b9c0526a9d14e169c45fbf72a2cc495e590f2968bcf46aefce`  
		Last Modified: Fri, 18 Mar 2022 07:09:15 GMT  
		Size: 45.5 MB (45484444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:87d138b68073f7e0053757258680456bee34d1d04034145b587077630105a43a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71283242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2383927ac3825b3ef97589e9f216945f76f3f90b8af0a2f2cb0a199d8d2c5b02`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:07:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 03:08:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dd41a6c49eacf0df81b34978f371986d045163bc627fc8cc72de7188772b43`  
		Last Modified: Sat, 19 Mar 2022 03:40:45 GMT  
		Size: 5.7 MB (5712348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd796a264aa4c81e3c709b9f64a9058add3ff5a5d6182545c52efe99ffacdc7d`  
		Last Modified: Sat, 19 Mar 2022 03:40:42 GMT  
		Size: 2.6 MB (2584607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082f0bde1e152ac77e4ab26f624f3d2205c3ae15f1bbe59b9ee93647f4fd409f`  
		Last Modified: Sat, 19 Mar 2022 03:41:24 GMT  
		Size: 40.7 MB (40678154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:283b95931d38014c8def465bfc3c89c8ef08b18ea289f6d865fcf0c2ca22fb9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75663780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28f746734cef327170ff1bb22af4e8f324c49059161460ba322f0846fbff5b4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:14:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:14:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 15:14:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41286690e6e0880a7eedf7b719947899206ac7c646b802b51885491ddc2471`  
		Last Modified: Sat, 19 Mar 2022 15:23:19 GMT  
		Size: 6.1 MB (6082571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b6f7caed42996ec474afab3c51a3ef72660e3cbb42cb8c5865299122c0c109`  
		Last Modified: Sat, 19 Mar 2022 15:23:18 GMT  
		Size: 2.6 MB (2570252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bd0e9947f40049a8c9844722bfb13a9fb959b1afef96b347d61c7ca538b481`  
		Last Modified: Sat, 19 Mar 2022 15:23:38 GMT  
		Size: 43.3 MB (43281853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d15b6679b013e58d2403036d267ffbfe0b9138bb72ec2d93a3bad0017e3ce79b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84199825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c04f520e6ac601298f3863a7e9a37dd1f5343e60ca56ff3924b6619747ca4a4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 10:41:23 GMT
ADD file:72f05c1b10aca0acb5e79b003217b981354d67a2f72a45a5a48a74d5a22d8a52 in / 
# Fri, 18 Mar 2022 10:41:24 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:04:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:04:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 18:05:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ae2a3052b0bf32822826824df976f36386fcf8a79f3777f41da7a64101a1603`  
		Last Modified: Fri, 18 Mar 2022 10:42:30 GMT  
		Size: 27.2 MB (27162241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9e6babc5b42003a6314f5d85981704d30c95f5d0d1eba244b2a71f27519cfc`  
		Last Modified: Tue, 29 Mar 2022 18:19:50 GMT  
		Size: 6.9 MB (6929200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57500b148c0956371d20107dafed67b0fd92150bd4ed920637bf6ec22be1472`  
		Last Modified: Tue, 29 Mar 2022 18:19:49 GMT  
		Size: 3.0 MB (3038470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afffc1e0c6ca285038bbaaaf16b84b6ed72eefafedc19cccf36a5903cb61e4c4`  
		Last Modified: Tue, 29 Mar 2022 18:20:11 GMT  
		Size: 47.1 MB (47069914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:61439d2e2722da64a2a213ebedf250b8e729a0cbba1b3ffdfc7b00adf513ba7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94937852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2b4aa7891a9773811ad323563c75bb26e12994fca3c31bbdc078274bb38332b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:47:57 GMT
ADD file:512f577cb3b73f892801365276edc7835b0fbed63fe39c4e98c86264d363163b in / 
# Fri, 18 Mar 2022 00:48:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 06:09:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 06:10:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 06:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37a959c2edf986d1489b0000a2dbfecd72195cde6524f2a6545bf3c5d66f6bac`  
		Last Modified: Fri, 18 Mar 2022 00:50:57 GMT  
		Size: 30.4 MB (30438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1830b6c456b7475c45d963eda213b02483fc132dc1a3a8a912694395f1556c6`  
		Last Modified: Sat, 19 Mar 2022 06:49:09 GMT  
		Size: 7.1 MB (7056588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f35c7c52bcdc240668649aeed659e09476496c4c7a0fa05fcbdb7bed19e76d`  
		Last Modified: Sat, 19 Mar 2022 06:49:03 GMT  
		Size: 3.7 MB (3719308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ad29e0143d51c4eb9be5f7f43a5c00475708f80c406a070df25b58b889631`  
		Last Modified: Sat, 19 Mar 2022 06:50:04 GMT  
		Size: 53.7 MB (53723900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2e70581562c81e3a071d016b8532f1a13d916356c0b6387deedd902dae5829c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79687193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91d03b5446fc0504d625853bc76e8288f8cc121ca22ebf3556b4392a77d8834a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:37:02 GMT
ADD file:ca83c77547f5f41417a9bcad24827780f3cecda3aadc05e3ea075ef651e7a96c in / 
# Fri, 18 Mar 2022 00:37:05 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 17:05:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 17:05:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 17:06:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:19966aaba2fa737074d039f29b54f413d837daaa9d85f02bc54eddd7d645b73c`  
		Last Modified: Fri, 18 Mar 2022 00:38:33 GMT  
		Size: 25.4 MB (25365461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707de7995f967781fe849ea5a655fcb09a909fd6fb0b137984e23c20e247748`  
		Last Modified: Fri, 18 Mar 2022 17:14:33 GMT  
		Size: 6.3 MB (6332555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b377478018a8c1dec3ff1d3e1c0d8db2e042e1ab1fe80f7f615a0f777ad6d4`  
		Last Modified: Fri, 18 Mar 2022 17:14:32 GMT  
		Size: 3.0 MB (2974971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4c065ee36aeeb2fa0b5ab382cbd1b4d5f53998d5179b40d2de303ae6b25b24`  
		Last Modified: Fri, 18 Mar 2022 17:14:46 GMT  
		Size: 45.0 MB (45014206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
