## `buildpack-deps:hirsute-curl`

```console
$ docker pull buildpack-deps@sha256:970ab52135ff9f1b5ce05d7771d5c687dab481f22acaa813c955869ed88d38ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:hirsute-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9ba88bbe791266d9b7514667385cb7a341be4800ad96aec28131caa66c6280eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40930683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdd9ae90e2e06c1c083754ce29dc4d5cffbfc6fdb0d076fe7557e0ed87fc625c`
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

### `buildpack-deps:hirsute-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7f52e050098e2fc996ad7aca6a916939ad58cd412d57fca5945c913327f73571
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34843240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371b4fb133daa245c217bc1b96fa063e10141bc19630006e4bc28ab36fcacc42`
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

### `buildpack-deps:hirsute-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:16033a777bc573ecefdade14ace94433e13fb4a0b141dae67ae65df921c1fd2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39338025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8deffd88f3bcd7d3f6a975167178885e51cbfa3f49745847c080f9868ede9a48`
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

### `buildpack-deps:hirsute-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e796b8645b84771fbe12e09111c7cc34eb2b7caf137927b0c1f6431e53169c0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48002417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd340bdb564206dc12af6e641d54c3bdf26271d3ef6752f683507d38c067fb62`
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

### `buildpack-deps:hirsute-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a38dbf3f42d698f0ca17e73028a3dfd80e741ccc13bb933abf8d13c1c555bb6d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42685813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23110081a69b5d65ea81f1816558ddd575b9664d30730b257125d62e34dc2c6d`
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
