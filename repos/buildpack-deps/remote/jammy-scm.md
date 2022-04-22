## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:ec9171dd7323fffd3879f6b494586adf72364529a87826b368d9736f739f40a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:79911f86b093554149716965c98e60817c7a964ae1c7c603276081ea4330c9ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77139517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b00539a0650dc66565fd45bfee596c715db723a3622f940392aa2776c723897`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:26 GMT
ADD file:76dd6cab5732b31272279bb8868954cbbecf591f596f0c318524454e95eabfb9 in / 
# Thu, 21 Apr 2022 23:00:26 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:38:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:38:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:38:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8527c5f86ecc162d68a9d38c8f4c6a6443158c67417e8bc2c3cea9f3868394eb`  
		Last Modified: Thu, 21 Apr 2022 23:02:00 GMT  
		Size: 30.4 MB (30421209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267116e5ed7e25114cae791a2211cd6d54e09ed17d486b053ee196b0ab35247a`  
		Last Modified: Fri, 22 Apr 2022 01:46:56 GMT  
		Size: 3.8 MB (3818107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca1d741d4fb6f7e87293ff74efc9ba1e21413c3597973e423b994995c11f2a1`  
		Last Modified: Fri, 22 Apr 2022 01:46:56 GMT  
		Size: 3.6 MB (3559200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05ba7d442ad3cfbb5c41d47b05e77368b09b61a52a921d94eda03ff638919da`  
		Last Modified: Fri, 22 Apr 2022 01:47:12 GMT  
		Size: 39.3 MB (39341001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ed16de4c61260207029b60a5e82083b0fd32e35e4963fca16b943a536b8cbf15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76547370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4686c81acb2dd3833b4fe0069fb08266a5a74f30cda5ba3bb03a17f91331de`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:26:50 GMT
ADD file:95fa9814c92c68f6ebb968c026d5dc32392b2d7bf63598bd9c94956e439de1a2 in / 
# Wed, 06 Apr 2022 03:26:51 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:14:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Apr 2022 05:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:baabe2d26ef2a12fec9a57ed43158809666a1abdf64bf549d076889bd1044f2e`  
		Last Modified: Tue, 05 Apr 2022 13:24:57 GMT  
		Size: 27.0 MB (27039821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9878dc19e3020210f7d655fdac19d0a7fa3c3c2c573bea20a0dfcbb4d2c4354c`  
		Last Modified: Wed, 06 Apr 2022 05:32:31 GMT  
		Size: 3.6 MB (3569089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df52222cce1438f8ef50179567991c9b454b8309aaf7036e0a978cd45124fc57`  
		Last Modified: Wed, 06 Apr 2022 05:32:31 GMT  
		Size: 3.7 MB (3712445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c2a68bbf06b56fcee764ca520807cd1dc3ae61c5581f74832c7612ea0576b`  
		Last Modified: Wed, 06 Apr 2022 05:33:12 GMT  
		Size: 42.2 MB (42226015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:989c836346a891eb53d21cc46f7e5161df15ae3639913004891bda905bb43df8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75106143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8059e23943aed00a19ba1c651e8d59e0383014804240aeab99d86d2a874657`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:19 GMT
ADD file:49571aac1d9686cc3e1be327834e8e0a9d0cdef8501fe221dfa628689bd7459a in / 
# Tue, 05 Apr 2022 22:41:20 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:10:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:10:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:11:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b267b9306c29bd8ae0bcc24ca28ea93e4424c701b94c4c0390bed799035db1c2`  
		Last Modified: Tue, 05 Apr 2022 13:24:30 GMT  
		Size: 28.4 MB (28399696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ebe8351a60fd8356b722173592beda77dcf8c69e0d490eace665f5653e6d42`  
		Last Modified: Tue, 05 Apr 2022 23:18:17 GMT  
		Size: 3.8 MB (3792418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e15399f06b734423260659df4dddbe3348365b046d4083c19ff5a3e30bf590`  
		Last Modified: Tue, 05 Apr 2022 23:18:17 GMT  
		Size: 3.3 MB (3319632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127a3e2fd930b70ae5dff71a4674a1b08883b753958a066ed29b68b88b875bc`  
		Last Modified: Tue, 05 Apr 2022 23:18:34 GMT  
		Size: 39.6 MB (39594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0798e8b3a31e9d526779d9c9ec8ef7c4764137a26a239b2d40c6a0444f2b3906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77233334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85037418c7faa59b7c753f2a24054ba86204fd78bf08cf4915f7833d076a1c37`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:18:39 GMT
ADD file:75794a810468b5240ea932e78dd71b552e395323c6ec0cc79d804146f90ee444 in / 
# Thu, 21 Apr 2022 23:18:40 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:24:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:24:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 00:28:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e4d3d9efc57e0160a4c8fd76a93cec2e8274d4660b25de44af6a0831c87634b`  
		Last Modified: Thu, 21 Apr 2022 23:36:51 GMT  
		Size: 27.7 MB (27745140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15eaec18e9fe1aa3ca23012ccd477dfb97162ef7d1cc1ff10a7f15de84b624fb`  
		Last Modified: Fri, 22 Apr 2022 01:01:34 GMT  
		Size: 3.6 MB (3612933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e7dfd819c86c7572101432d76daed4fc4e538bae377fee2c79ebfef409c812`  
		Last Modified: Fri, 22 Apr 2022 01:01:32 GMT  
		Size: 3.8 MB (3776427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f258cff627ce7b638521230e6201bef2042483928396ed5686b88d205fc12`  
		Last Modified: Fri, 22 Apr 2022 01:03:46 GMT  
		Size: 42.1 MB (42098834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:11524bedf291207fe5d82b7eddc6e87525b31b7ab4fcffc45f7339dc0c34a5e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75192696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94747795364cc2670f94f2faa6ae836efdbb1ff9b0b26fa70c0546d745a76e34`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:40:09 GMT
ADD file:f5c8ee58aa674a88e8267835525f464ce4e6ee2c7a4506c9eff01d29081398de in / 
# Fri, 22 Apr 2022 00:40:14 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:43:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:44:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ffa6b3b756915b08f6495cf57b768499d1d1fd3a7f46ab94bd8044af9a08994`  
		Last Modified: Fri, 22 Apr 2022 00:41:47 GMT  
		Size: 28.6 MB (28637170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47d7fdbcbc80f5dc0de3bdf9e8bed5ceae6257cdff80136ee423cf776bacca7`  
		Last Modified: Fri, 22 Apr 2022 01:53:40 GMT  
		Size: 3.8 MB (3820151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71a168d4d5e4858b693200251b235dc42f9148db3c17780717ea5b3b510bd99`  
		Last Modified: Fri, 22 Apr 2022 01:53:40 GMT  
		Size: 3.5 MB (3470573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90b0629fe2365968f74a4355899f4cde325e48153a40dafcbc1349dbee99a76`  
		Last Modified: Fri, 22 Apr 2022 01:53:56 GMT  
		Size: 39.3 MB (39264802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
