## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:25aa1f87d4e3f7b1c571480c99eb63c5c26d413492d0fe3054a3758fde9ae480
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1b0d7f988e97e2c04a9b133c03a17318ba8d090665be0379dac37bb2584d09e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84691134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bbd40979908b65d5c3b61b2ef5869a7ce5f32ba07612078b7e85d2c1dd86aa2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:44 GMT
ADD file:60b287b09986a8e8c3d9cdca2ee7e42ccb5349cca29f8720b7269b258551be15 in / 
# Thu, 17 Jun 2021 23:31:44 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:44:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:44:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e2d1c03542857d58a3cae774cad57f863543c683f444da46126220e343c359f`  
		Last Modified: Thu, 17 Jun 2021 23:33:33 GMT  
		Size: 31.8 MB (31838498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a9990dd093d007a85113fba8fb76ca8b7a6d559abc0fa0e09888d1c681629e`  
		Last Modified: Fri, 25 Jun 2021 21:53:30 GMT  
		Size: 5.4 MB (5430714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1a386bb0a5ec44f2db7cf4b64016255a36837cdd1c6a2781e4770db48182a`  
		Last Modified: Fri, 25 Jun 2021 21:53:30 GMT  
		Size: 3.7 MB (3661471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c016cfed562ac5a356a0609ba1cbb3bec23f796dc2bd345839c34e81d3a658d2`  
		Last Modified: Fri, 25 Jun 2021 21:53:48 GMT  
		Size: 43.8 MB (43760451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6a8f926bade961b353bcb1697c78864c123d7dfb7e101a39ff67be67daacdf7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75003976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e3f4e6e696af528723ed802149e9e112fdad2c3b7751a55bfcc1583b7d432f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:30 GMT
ADD file:edf6d852373478f415087a473f977275a1cd2e0f2f2ea2914233dd9848300f32 in / 
# Thu, 17 Jun 2021 23:32:30 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:39:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:39:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:40:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e91134f25ff17dcefc1502cdfb0473acec980e15fd4018fbc611fdac57c53a4`  
		Last Modified: Thu, 17 Jun 2021 23:35:46 GMT  
		Size: 26.8 MB (26847070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e780f8e1bd2a3e00f282a61507aaeee0aaaedcce645f8cac36e21dee950830db`  
		Last Modified: Fri, 25 Jun 2021 21:52:06 GMT  
		Size: 4.9 MB (4858085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4762121ee64b6532d871aebaefa843c37f1f15334218b40ce6f652dd7d52b6a4`  
		Last Modified: Fri, 25 Jun 2021 21:52:04 GMT  
		Size: 3.1 MB (3138085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e36633ab4f0fe1c8a83c86ea2e9cf27a226c2dc5ce5c1de8d3feeb21ffef776`  
		Last Modified: Fri, 25 Jun 2021 21:52:51 GMT  
		Size: 40.2 MB (40160736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:565037abecead496bc2a2792340f4de17c1a935d746fb874394fc6e806125c6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83102855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1efcc52269e8fefb4a3d4c7b5d21720daafc86e7b03def0f68b3a71a0134a48f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:15 GMT
ADD file:14f2cfab8ca5ecbcf5781b131b4f4698cc89fe6c9885d37857eca6f4956223a1 in / 
# Thu, 17 Jun 2021 23:54:16 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 21:54:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 21:55:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 21:55:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:546693bd47c7a007f5d22f034279c659c2c0269da36d6a58641b3ebf416e3984`  
		Last Modified: Thu, 17 Jun 2021 23:56:46 GMT  
		Size: 30.3 MB (30297621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bfabf30a70ee3337e72e934e7bd51f7971eb3976016f69222f6ab6028d8e6a`  
		Last Modified: Fri, 25 Jun 2021 22:00:55 GMT  
		Size: 5.4 MB (5402846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ffba69d983f3ea04c4ae3aa81c9ff5c3f13aa311fb4011965ac687cec3ae7`  
		Last Modified: Fri, 25 Jun 2021 22:00:54 GMT  
		Size: 3.6 MB (3637558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d0fc593628bfd107b9a088fbddb06f197e8a907849b34016285f98b6265d9b`  
		Last Modified: Fri, 25 Jun 2021 22:01:14 GMT  
		Size: 43.8 MB (43764830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bd9d858b62c509ad77b643a6f06b4d9dff9d6422339437618e59e00e83cf658e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98047388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bbdeffc345b7f3b85dc299d030ad5e84e558bdd34cff9274273796ff304f03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 03:52:02 GMT
ADD file:3d7449eef944b930488986ed089606017a4392e5e8231031c80e680e31b4da77 in / 
# Thu, 21 Jan 2021 03:52:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:52:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:52:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:52:47 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 07:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:35:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Jan 2021 07:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55aebc4be35f4811f0c02de6f92178fd8f7b65e395e8cb03da193bac6fafea1d`  
		Last Modified: Thu, 21 Jan 2021 03:55:55 GMT  
		Size: 37.1 MB (37120027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4a190c1c2a83741c3769bb3ad14038be64a619a04aa712f80ce3a1f5218e5`  
		Last Modified: Thu, 21 Jan 2021 03:55:47 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009631d025b1b2b9e034f9fd76ed1e632a0dc6f0aeec51263339007901b56748`  
		Last Modified: Thu, 21 Jan 2021 03:55:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02946107bd138c77db9eab66487871adfba9c8b7b078d2990a469890389ec91`  
		Last Modified: Thu, 21 Jan 2021 08:10:57 GMT  
		Size: 6.1 MB (6054214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cd4a6aa56af3abb812e969114f97e4dc21f400bccfa57cd61e6a36d310c99d`  
		Last Modified: Thu, 21 Jan 2021 08:10:56 GMT  
		Size: 4.8 MB (4827138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be0c8d3e6c904e1ab054ea36644f54cd5145a5631456649af11bbbaba489e5f`  
		Last Modified: Thu, 21 Jan 2021 08:11:24 GMT  
		Size: 50.0 MB (50044971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bf8ff828a8c44bbab2367facb42dcde50721599bf5efa35a5643a8200479c90d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90749117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10390433921267d86fac2e3e998d424494e12fae0488134e025e29c223695d3e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 04:02:00 GMT
ADD file:8ec30abb851d24263f13b8ab93a9889626368053d325848b2f951e43ccac9a0c in / 
# Thu, 21 Jan 2021 04:02:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:02:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:02:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:02:12 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:25:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Jan 2021 05:25:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35d604bd00566c6cbc331e49db9228af41b973581b365975622efcddfda24580`  
		Last Modified: Thu, 21 Jan 2021 04:04:14 GMT  
		Size: 32.5 MB (32534356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8645fe124321a0a9ceca773d8bd654c8edfb63087f69654dc33b005cd936031`  
		Last Modified: Thu, 21 Jan 2021 04:04:09 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811acaaa59ef2c29c645ec90173a876498cec8129d2051e6826881ba068508fb`  
		Last Modified: Thu, 21 Jan 2021 04:04:09 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c0a035e1b4479247e30498cb38c95743838097221a8aafc70ede4da8e1b6bf`  
		Last Modified: Thu, 21 Jan 2021 05:34:30 GMT  
		Size: 5.7 MB (5691508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476bdd8305678676c465817a601000b79a702ef2feb7d9fc199dd171304f9712`  
		Last Modified: Thu, 21 Jan 2021 05:34:29 GMT  
		Size: 4.5 MB (4458912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9928f3c621a6ce2274dfc19b3cdbaa1fb5d4b0bb2c1e5b4e0a4bcd581247ff79`  
		Last Modified: Thu, 21 Jan 2021 05:34:47 GMT  
		Size: 48.1 MB (48063304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
