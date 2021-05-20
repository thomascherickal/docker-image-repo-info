## `buildpack-deps:groovy-curl`

```console
$ docker pull buildpack-deps@sha256:a314bcaf71ba75d93d6976d83345d99568e54603af07bf5a37210e2c700a204d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:799ffbefab58874603085a760eea6774ee932ee57877b87132a2930b980001d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40397051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:379b6f8a6b2e2c6ae0648ddd6ca87572218dbb9c26b78a0cf293c04a0e1a0700`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 19:44:47 GMT
ADD file:50e56682329ac9b5b81321252a40154457a3f54c6972fce6c9755e513b4c8955 in / 
# Wed, 19 May 2021 19:44:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:49 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:50 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 20:21:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 20:21:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:abbb6e7817965b3a1b696d2d3393724dcba223f50e3be0fae33410c50a67db78`  
		Last Modified: Wed, 19 May 2021 19:46:05 GMT  
		Size: 31.3 MB (31328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ac6b0850ddfacd14d25844827637a38cf1bc3b9350ded94f9f6c7533765c73`  
		Last Modified: Wed, 19 May 2021 19:46:01 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666bf17853adc7e13292d64bed15e1e5c32888a27d3853b99a65b822a1bf62b`  
		Last Modified: Wed, 19 May 2021 19:46:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c133b90612991538174a3f5a9d68ab55070778b50695679d5af1df29556f8096`  
		Last Modified: Wed, 19 May 2021 20:32:51 GMT  
		Size: 5.4 MB (5404400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c19d37f0d899bed474caf69a57883dc48195c5f968fb420eafdf5c272738c3`  
		Last Modified: Wed, 19 May 2021 20:32:51 GMT  
		Size: 3.7 MB (3663496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:33775486d3a5718b7933408f00f1327697c79461ffe7d7b5b27859a9e9941d98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34283179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78e5543d54be9b1a75b3cda5bdc0e40fc0953fc474094e6a067ec74e15f693f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 May 2021 20:22:24 GMT
ADD file:acda6861dee730077731d36484af6c3fa51a7ea2bcdbab39a88f53cb3276509e in / 
# Wed, 19 May 2021 20:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 20:22:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 20:22:32 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:24:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 21:24:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ec376efdd72c4146827ffa866153a4452541beae9106def5a3afb4e858023939`  
		Last Modified: Wed, 19 May 2021 20:24:15 GMT  
		Size: 26.3 MB (26301801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065457da20bed844ec32f63c2c352d39da0d9cf58fd9fcdd710a8c2fe01e0ec`  
		Last Modified: Wed, 19 May 2021 20:24:08 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acffea83b1b3aaf9f535176139002bf18809b84cc711fddf2a83206c09194c8c`  
		Last Modified: Wed, 19 May 2021 20:24:08 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79506122a3d0c6d63e1d7f71ccc97b810db680e7216ace4caefdb03fbf36cd72`  
		Last Modified: Wed, 19 May 2021 21:33:12 GMT  
		Size: 4.8 MB (4840236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50daac1ff3d8fede9e0c5af53d483d76ae250d8cd081ebc17c9ab2330a2bfad`  
		Last Modified: Wed, 19 May 2021 21:33:11 GMT  
		Size: 3.1 MB (3140106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f75586cae2b63636f9418b5d68c1aa278aeae5075ddafe8fc768ebcd6584dc73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38866123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01d22bf091b8ce5301231cb686d4bb5fd2efffcdcc04c92c13cafdfe5fb1efb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:48:13 GMT
ADD file:3b909e405de304d3529a43650aa6812b726dbfe24e2f2a9c163818ab5c206cf1 in / 
# Fri, 23 Apr 2021 22:48:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:48:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:48:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:48:21 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:56:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:56:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0312c280f333ebad21d92c6554a1f0b81a5d7de275f2f1fe29c960721e40cb28`  
		Last Modified: Fri, 23 Apr 2021 22:50:26 GMT  
		Size: 29.9 MB (29858157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fedfba085a0c1226682c17f7966295deb654a557860da25aedabd09c96edf6`  
		Last Modified: Fri, 23 Apr 2021 22:50:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d5a4de4889c6c2db1938b8170a1a427483a6b6ab113ceeae3e4b02819d54cf`  
		Last Modified: Fri, 23 Apr 2021 22:50:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad193c7d2fd3d7abe2b82c37995e2605da385f11ca2f06dc30d5f5dc345c65f`  
		Last Modified: Sat, 24 Apr 2021 00:09:06 GMT  
		Size: 5.4 MB (5372256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af75efe104a171231aa661eca3858d14899f05643299dbe97ba30db9017801e6`  
		Last Modified: Sat, 24 Apr 2021 00:09:04 GMT  
		Size: 3.6 MB (3634669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1f9b0267834d6e8d2312ebf0fcb89dd211e08e22b953bf40ec2e57e7e2c26802
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47090157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e7cbfd92f984d3814783fb1e3f316897adfe393e9aca35a282c94b52e4d92c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 22:32:56 GMT
ADD file:9b647581492e8a9debf7c9a73eef985aebb7072321f5d8fa8c472b53fabafb28 in / 
# Fri, 23 Apr 2021 22:33:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:33:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:33:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:32:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:33:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d6ce6d3be4f5eb39a61ba05bb53c38219cd1113199e7fc30c6cd2cee4c5fb5d6`  
		Last Modified: Fri, 23 Apr 2021 22:37:33 GMT  
		Size: 36.5 MB (36527808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade482f405991ee00e6a2b07829b6997544361111bef88921c675886395fb6c9`  
		Last Modified: Fri, 23 Apr 2021 22:37:26 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc274e55013ed26baec88baa6993c5b544fbe9cb3ea899c2064ded5c32994964`  
		Last Modified: Fri, 23 Apr 2021 22:37:26 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174c6f22368d4cac81dbee4c63df9b2b4ad7bbac04afe87a1a68395d1ab9bbdd`  
		Last Modified: Sat, 24 Apr 2021 01:13:04 GMT  
		Size: 6.0 MB (6040163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913583832c077e8640bc72ca4391f09993d0ad7f9251c0ed5fd6c169766f8997`  
		Last Modified: Sat, 24 Apr 2021 01:13:03 GMT  
		Size: 4.5 MB (4521148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8bbb24c114be873946d24c309d5fe19e1993e8b6cba79ff6b6f4517e8e000428
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41336069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e6a73130cede03827f5c6767335c4bb827be1442352185bf6c2b762e0531a3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:41 GMT
ADD file:e6865857806d2adcd065b953497329982bba48a3a6eddfa285bdea7e0935c6f5 in / 
# Fri, 23 Apr 2021 21:45:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:50 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:39:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:39:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9dbc4da983b078d09d29988b8fc29124d77343f51e37478aa7c739723643a81f`  
		Last Modified: Fri, 23 Apr 2021 21:47:28 GMT  
		Size: 31.5 MB (31549443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7549c1649fc091c9984e5c7ddd083a6be49bf4b45230ac596a40f0930a011ff`  
		Last Modified: Fri, 23 Apr 2021 21:47:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b497247d2426717163cda90b8a84237dc66047912b51fe973a412dd0aa0cc0`  
		Last Modified: Fri, 23 Apr 2021 21:47:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533386638b5e92cc76ca1e9a92de024ff9eb4686940fd0e0484c67cba2d5faf9`  
		Last Modified: Fri, 23 Apr 2021 22:49:48 GMT  
		Size: 5.6 MB (5629335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff2bfb0558738f5fe21e9c857cd3f7086fa08bf5ba0f7eac1e63972758d04d5`  
		Last Modified: Fri, 23 Apr 2021 22:49:49 GMT  
		Size: 4.2 MB (4156254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
