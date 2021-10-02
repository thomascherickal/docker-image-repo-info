<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:14.04`](#ubuntu1404)
-	[`ubuntu:16.04`](#ubuntu1604)
-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:21.04`](#ubuntu2104)
-	[`ubuntu:21.10`](#ubuntu2110)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20210930`](#ubuntubionic-20210930)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20210921`](#ubuntufocal-20210921)
-	[`ubuntu:hirsute`](#ubuntuhirsute)
-	[`ubuntu:hirsute-20210917`](#ubuntuhirsute-20210917)
-	[`ubuntu:impish`](#ubuntuimpish)
-	[`ubuntu:impish-20210928`](#ubuntuimpish-20210928)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:rolling`](#ubunturolling)
-	[`ubuntu:trusty`](#ubuntutrusty)
-	[`ubuntu:trusty-20191217`](#ubuntutrusty-20191217)
-	[`ubuntu:xenial`](#ubuntuxenial)
-	[`ubuntu:xenial-20210804`](#ubuntuxenial-20210804)

## `ubuntu:14.04`

```console
$ docker pull ubuntu@sha256:43cb19408de1e0ecf3ba5b5372ec98978963d6d0be42d0ad825e77a3bd16b5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:14.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:881afbae521c910f764f7187dbfbca3cc10c26f8bafa458c76dda009a901c29d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b66b487594a1f2b75396013bc05d29d9f527852d96c5577cc4f187559875d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:40 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 25 Mar 2021 22:33:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551a797c01db074ab0233ceb567e66b8ebdcb9de9a2e7baa36d57dfbca463a3`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 72.7 KB (72664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512123a864da5e2a62949e65b67106292c5c704eff90cac2b949fc8d7ac1e58e`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:534255069ef3adf1c7a555fd9f614845ab66c61ef9846e438d86e12ae8c89b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2cd03315989aa8326f2c276922d3969994c1304b1310d2e0d33a26d94dd68ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:23:03 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Tue, 13 Jul 2021 23:23:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:23:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 13 Jul 2021 23:23:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:23:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c5cd1be699257153c2a6de85968c2d9c413d87470dc4f540c5c3decbca8e47`  
		Last Modified: Tue, 13 Jul 2021 23:28:27 GMT  
		Size: 76.8 KB (76774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf1c32ebce749806713a088af6ff1cbf7c75a8132d310ff391948e3e611ef6`  
		Last Modified: Tue, 13 Jul 2021 23:28:26 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:0fe9a82e42e32a74cca83fc84d5ab80b2ef73b7b90b7bab661b00ef3d16bfad9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:423c4ed354ff1af8b464f13e25792ddb5e0a2c6baa22b5af909e68b557062eec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 May 2021 12:30:34 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Thu, 27 May 2021 12:30:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 27 May 2021 12:30:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 27 May 2021 12:30:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 27 May 2021 12:30:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e84a55d935eb29baa4a459e89f330e090e7f9db90fbdd96f6c47b89c614c671`  
		Last Modified: Thu, 27 May 2021 12:33:16 GMT  
		Size: 59.1 KB (59096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a9c88d39064b3377476bafe5b4a86f498750df033058cc4a61194f2ca5540b`  
		Last Modified: Thu, 27 May 2021 12:33:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; 386

```console
$ docker pull ubuntu@sha256:88152195106ff09bade23cb5aacfd26c381a8835c9d42124b4cba1dc3c2475e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ba408bae1426c4f394e045b16a140bc555e520d5eaacc97ac60ac5f298313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:57:06 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 25 Mar 2021 22:57:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:57:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea2d50b5278097c6d027fc9fc0caf006649fcd94f094dde6ce578abe865ff21`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:12d9fa858f255e4b70827aff83e8ce37b6fcaddaf6732276aa1f0763402f4fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02949c650aebaafb917ebe6bfd55a42505e22b38e8370878164051da4ae1bcc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:24:04 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Tue, 13 Jul 2021 23:24:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:24:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 13 Jul 2021 23:24:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:24:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aab203a69be44b1617f0da6b00b670e9016c3b00ab311b384ac3f859e86613`  
		Last Modified: Tue, 13 Jul 2021 23:29:07 GMT  
		Size: 63.4 KB (63430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1576c78d220b27404b5d0c3d635c36524229553e3ccf3b9a5ad4ca93c216c6c6`  
		Last Modified: Tue, 13 Jul 2021 23:29:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:16.04`

```console
$ docker pull ubuntu@sha256:454054f5bbd571b088db25b662099c6c7b3f0cb78536a2077d54adc48f00cd68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:16.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:a3785f78ab8547ae2710c89e627783cfa7ee7824d3468cae6835c9f4eae23ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46499103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f50765242581c887ff1acc2511fa2d885c52d8fb3ac8c4bba131fd86567f2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:b722e2654241f9681f4719dce7aa16a2f0c35769e17a636f5b39a33967d1aeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40313783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033c410d53efaab9e847168b94fea14d551788200a15f4d2424c84e4cd2ab8a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:11c7a73a8eb322a177481fdeafc34957200f2f0d1f2192044ad5262008d4bba9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6834beb45bf45c3a0423173bc99b6c7f1ae051b0187febdf9b9e780beac78af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; 386

```console
$ docker pull ubuntu@sha256:4a6759446930ee402a2091605c0911f237ad18b5c250a535d11563d9402eb15a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac20e7c3411697a4a85c1cb30850f77b8238e0a0ef0e176ca8f0e763066eed4b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cf25d111d193288d47d20a4e5d42a68dc2af24bb962853b067752eca3914355e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47523633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914466c340b7c02825333f4de2597bcd673f18eb0cec83840b13a3cc68338937`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:5fea5a070916f61785140faa8e16fa8bf7ca3f152ceed9c48154f8aca4c3667e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb8683432fbdd1ec03145305370c4ec7079b01e22fcc47dd4df1aa862463474`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:d501bde46939f19cb83d6fc604f8d0cda403683e8aa9765f5f0f271de3025279
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:18.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:fc0d6af5ab38dab33aa53643c4c4b312c6cd1f044c1a2229b2743b252b9689fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26705075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a214d77f5d747e6ed81632310baa6190301feeb875cf6bf9da560108fa09972`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3e30324cd69917410983687854bf0f31f03c9dd4ecdbd55f75068f989a318def
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22304304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20adc023075c337e050411d61c993daf3bf85180e287addf9b7a6bce6fa7b4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:4b114761663a63948fcd36ef36315b31370c52e59546cf32fee60a8fb16aeddf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23727476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6441fe3d04f510c10053f360ce7ab676bfb87f098a8cfb8ded445722fcb261`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:ca98d3a711fd16c1e7565be9d2668f90c3f5eba708cc538ac902bb2da269bdeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27158466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44056bbf2d5ce1042c35164084bcb51ba0c185a4033c2aad7417fdd8c6346cb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:450907f6c8be99db80d11bc3f6f34296fd79b08fd120edfaf904e94346e4d06e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30437758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab745013b69681e72ca8828de7f7a56a893838db3ad31280202d6365e10f46d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:66504687c64ca60db9f451c76c8306af50b276c28c614f18c4ae34007fa244ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25362918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75982df0039a45ad1d04b6976b7f279d80594692b7f8b14d2368bc2fe746062b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:44ab2c3b26363823dcb965498ab06abf74a1e6af20a732902250743df0d4172d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:20.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:3555f4996aea6be945ae1532fa377c88f4b3b9e6d93531f47af5d78a7d5e3761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28568914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597ce1600cf4ac5f449b66e75e840657bb53864434d6bd82f00b172544c32ee2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e1a690fbb7b7f117472061b2025132b04ed1a3bbe5e48a3831d4813be7b20223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b3ddfc9fc5db841245f00fbeb98755ae3ab6d49dcb603bd5544ef55e00f15d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2eedb44775176d77c25c9a69c948b871b67624881e9e46553379443ce788181f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27172405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daab1c66d4670806f6a1890857dc5554a8c5b423ef4399b3fbc5c16022aaef0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8f083e3e070591f3f70ec51abd83d0e6e8b5c92fe4bc79775f50d0a22b8b7021
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33291791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0501f0572349877e5332affe472977acd6e5d4fe071a1cafe69a95dbb9c2c1aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; riscv64

```console
$ docker pull ubuntu@sha256:db6aab4e73bc6b1b7e824b693073f79cd706b096e3375187d1395b7c8b37eed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24227267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba84824da1bda6352c1401ef9e4f830b57f4f922223903106db69023c442a94`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:14:48 GMT
ADD file:a8b9aeb23e8f47568ef8ea33a80fee0c676db7c4c9ec9210abf75217a8f329fb in / 
# Fri, 01 Oct 2021 01:14:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:91a226dd2b609e6bc3e70f7621380def71f05b74e75fa1a2f0421795a8904f10`  
		Last Modified: Fri, 01 Oct 2021 01:37:38 GMT  
		Size: 24.2 MB (24227267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4ddabbb8109f098e206abe5dfa64c5429f82353ee50dde5484a1a48c047eb32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27122910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8749b206ce00913c9a567a3f1de60a9462e3014ac383e4c497b5c4d88f475b23`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:21.04`

```console
$ docker pull ubuntu@sha256:44e4ce6defdd88435d6f724b4ed4bfa3dd7796c93012bbe1af16da4a7479a006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:21.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b19ac4988412eaf6ab191ab246d2e1bc9d792ce9a57ef3e97635b41118c4fe9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31704296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f83bfe0b632bd4a5018a57a9c0386564d6ece1645862388200d5a81dae9a7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:54337979c56cc50b52ae70e5531b904e7f34a5d8c383770c75b14f51e5cb26d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26859487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3522c2cf51bd9e4a0315265f0b071fd2fc962ab20f7eeefd29b86b4b79c2c808`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:eb35f49285e58e4baf77e7a5eedeac57f1fdfeb688126a1914e61cb5d19f1ae5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.2 MB (30174163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083fe054c6965dc373db8b9863e89c31abd56aae8ad716c3830e5856c320d9e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:60dfaddf644de61f02ac434ee607fc67123d8c9a6e0b84fcee59211e6cc1a469
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37185952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f685da69c67500e48dad075763bd1bb10bad221d50a72a86abddc20a7a1b4a9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.04` - linux; riscv64

```console
$ docker pull ubuntu@sha256:b2cf15cebd073c22821e0b735d9c70eb108458992f73b73c43f4d14ef3038f04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27141881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faaad95feb654da33d02ceb6c15a5b384f9b432ec1b39e849347675e59eeabc1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:7341458761704d75f1ed1d436f99ed4be4984e978101c7dcd0a70f93ddc14b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32505539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c69fe2db8ddbdeff2f993f21dc6898446721a1af23b3649ed1556ec1db116d3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:21.10`

```console
$ docker pull ubuntu@sha256:9a7b522028ebc43104df4b9d9e3e8b002f4dbe316d6f09464a58306baeed0423
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:21.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:b284173fbabcefd6cd4ef871e408d3252b24d762a997323377eaa208240fb72a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30399219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd54db809ce7c0c4a5519431f18e583fc4571e433345ca7deceaa5a1f9fb6ec`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:24:06 GMT
ADD file:14abde46780e9aa8c8c5c54d89baf3f1913aa6fef0d44ecc320cf962c4ba9e4d in / 
# Fri, 01 Oct 2021 02:24:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6122078cc60fecb720ddc58a9f5be50b4112ba9f366d21eccaf834489eafdda5`  
		Last Modified: Fri, 01 Oct 2021 02:25:54 GMT  
		Size: 30.4 MB (30399219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4f92d734b1b459411bf08e3d372425f9fe32778c5379be9b871dcb36445573c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26916992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce570a3a124ab71b3f2a4b517021b2537b380b0eb4cef867bb9d5db03478906f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:55bce25aa903e56698b8ab74c96a9d4de4b152254bf766d2be6f48a02cd886f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29047978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68655ee9aa431faa0081c84edc93a175c59b8f897440c69bd30e69087b91e9cc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8bc56b544223a2ecba0926e57b706514e73ae4ff5ddeab090faed9020d4aa94b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36055099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3e2cffe6f2afc5e5fac69b863b56f13414865b1209ab3f6cfb962f746266c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; riscv64

```console
$ docker pull ubuntu@sha256:6d43cbf9a191da6a33efc5bdc327185ea8363d0ead8a07fbe8590d5a3bdde25c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7f6a349055717cf10ba89991eeded03ccaf3a92888ca35b7a84f56a798688`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:8370ebd1ad75d56999ebb386c9a3c9f3bc52e3e38a6096566a867d92bb6ebdf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30770041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4811400563f83422d383472f6ce188a30359e1e4b9534306ebf243f461cd2df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:d501bde46939f19cb83d6fc604f8d0cda403683e8aa9765f5f0f271de3025279
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic` - linux; amd64

```console
$ docker pull ubuntu@sha256:fc0d6af5ab38dab33aa53643c4c4b312c6cd1f044c1a2229b2743b252b9689fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26705075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a214d77f5d747e6ed81632310baa6190301feeb875cf6bf9da560108fa09972`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3e30324cd69917410983687854bf0f31f03c9dd4ecdbd55f75068f989a318def
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22304304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20adc023075c337e050411d61c993daf3bf85180e287addf9b7a6bce6fa7b4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:4b114761663a63948fcd36ef36315b31370c52e59546cf32fee60a8fb16aeddf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23727476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6441fe3d04f510c10053f360ce7ab676bfb87f098a8cfb8ded445722fcb261`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:ca98d3a711fd16c1e7565be9d2668f90c3f5eba708cc538ac902bb2da269bdeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27158466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44056bbf2d5ce1042c35164084bcb51ba0c185a4033c2aad7417fdd8c6346cb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:450907f6c8be99db80d11bc3f6f34296fd79b08fd120edfaf904e94346e4d06e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30437758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab745013b69681e72ca8828de7f7a56a893838db3ad31280202d6365e10f46d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:11 GMT
ADD file:32c084b07cf88f4b46c2c94d6e8634a245a8ea46f4c166fe98b49a7e3d44a700 in / 
# Tue, 31 Aug 2021 02:10:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b66177991333478fe4de9a7fc6ee8c546debb78334473278e085735e8a88072d`  
		Last Modified: Tue, 31 Aug 2021 02:13:59 GMT  
		Size: 30.4 MB (30437758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:66504687c64ca60db9f451c76c8306af50b276c28c614f18c4ae34007fa244ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25362918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75982df0039a45ad1d04b6976b7f279d80594692b7f8b14d2368bc2fe746062b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic-20210930`

```console
$ docker pull ubuntu@sha256:9a22ac5930fdf81e1d0353a57075e0625622b037751171e8fb5a6b269678b7de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `ubuntu:bionic-20210930` - linux; amd64

```console
$ docker pull ubuntu@sha256:fc0d6af5ab38dab33aa53643c4c4b312c6cd1f044c1a2229b2743b252b9689fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26705075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a214d77f5d747e6ed81632310baa6190301feeb875cf6bf9da560108fa09972`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210930` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3e30324cd69917410983687854bf0f31f03c9dd4ecdbd55f75068f989a318def
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22304304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae20adc023075c337e050411d61c993daf3bf85180e287addf9b7a6bce6fa7b4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210930` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:4b114761663a63948fcd36ef36315b31370c52e59546cf32fee60a8fb16aeddf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23727476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6441fe3d04f510c10053f360ce7ab676bfb87f098a8cfb8ded445722fcb261`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210930` - linux; 386

```console
$ docker pull ubuntu@sha256:ca98d3a711fd16c1e7565be9d2668f90c3f5eba708cc538ac902bb2da269bdeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27158466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44056bbf2d5ce1042c35164084bcb51ba0c185a4033c2aad7417fdd8c6346cb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 03:46:35 GMT
ADD file:6718b956b86d332e4a53184568ac5205e92f9edeba804c64254e3b2da6e66c72 in / 
# Fri, 01 Oct 2021 03:46:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:96391085795d2daa9755c58002e78a76eecf7fd57a1d8a3778e87b0079ed47e9`  
		Last Modified: Fri, 01 Oct 2021 03:47:35 GMT  
		Size: 27.2 MB (27158466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20210930` - linux; s390x

```console
$ docker pull ubuntu@sha256:66504687c64ca60db9f451c76c8306af50b276c28c614f18c4ae34007fa244ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25362918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75982df0039a45ad1d04b6976b7f279d80594692b7f8b14d2368bc2fe746062b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:17 GMT
ADD file:d248d4b5739ee5d07e920ec481dc4af81b314aa52e64618322197a642394a41d in / 
# Fri, 01 Oct 2021 01:42:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:97372e5b313b6b8bab9913de546bc50f73818d8275c94fc6491993c97b9d8bad`  
		Last Modified: Fri, 01 Oct 2021 01:43:49 GMT  
		Size: 25.4 MB (25362918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:9a7b522028ebc43104df4b9d9e3e8b002f4dbe316d6f09464a58306baeed0423
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:b284173fbabcefd6cd4ef871e408d3252b24d762a997323377eaa208240fb72a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30399219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd54db809ce7c0c4a5519431f18e583fc4571e433345ca7deceaa5a1f9fb6ec`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:24:06 GMT
ADD file:14abde46780e9aa8c8c5c54d89baf3f1913aa6fef0d44ecc320cf962c4ba9e4d in / 
# Fri, 01 Oct 2021 02:24:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6122078cc60fecb720ddc58a9f5be50b4112ba9f366d21eccaf834489eafdda5`  
		Last Modified: Fri, 01 Oct 2021 02:25:54 GMT  
		Size: 30.4 MB (30399219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4f92d734b1b459411bf08e3d372425f9fe32778c5379be9b871dcb36445573c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26916992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce570a3a124ab71b3f2a4b517021b2537b380b0eb4cef867bb9d5db03478906f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:55bce25aa903e56698b8ab74c96a9d4de4b152254bf766d2be6f48a02cd886f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29047978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68655ee9aa431faa0081c84edc93a175c59b8f897440c69bd30e69087b91e9cc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8bc56b544223a2ecba0926e57b706514e73ae4ff5ddeab090faed9020d4aa94b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36055099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3e2cffe6f2afc5e5fac69b863b56f13414865b1209ab3f6cfb962f746266c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; riscv64

```console
$ docker pull ubuntu@sha256:6d43cbf9a191da6a33efc5bdc327185ea8363d0ead8a07fbe8590d5a3bdde25c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7f6a349055717cf10ba89991eeded03ccaf3a92888ca35b7a84f56a798688`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:8370ebd1ad75d56999ebb386c9a3c9f3bc52e3e38a6096566a867d92bb6ebdf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30770041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4811400563f83422d383472f6ce188a30359e1e4b9534306ebf243f461cd2df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:44ab2c3b26363823dcb965498ab06abf74a1e6af20a732902250743df0d4172d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:focal` - linux; amd64

```console
$ docker pull ubuntu@sha256:3555f4996aea6be945ae1532fa377c88f4b3b9e6d93531f47af5d78a7d5e3761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28568914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597ce1600cf4ac5f449b66e75e840657bb53864434d6bd82f00b172544c32ee2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e1a690fbb7b7f117472061b2025132b04ed1a3bbe5e48a3831d4813be7b20223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b3ddfc9fc5db841245f00fbeb98755ae3ab6d49dcb603bd5544ef55e00f15d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2eedb44775176d77c25c9a69c948b871b67624881e9e46553379443ce788181f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27172405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daab1c66d4670806f6a1890857dc5554a8c5b423ef4399b3fbc5c16022aaef0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8f083e3e070591f3f70ec51abd83d0e6e8b5c92fe4bc79775f50d0a22b8b7021
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33291791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0501f0572349877e5332affe472977acd6e5d4fe071a1cafe69a95dbb9c2c1aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; riscv64

```console
$ docker pull ubuntu@sha256:db6aab4e73bc6b1b7e824b693073f79cd706b096e3375187d1395b7c8b37eed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24227267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba84824da1bda6352c1401ef9e4f830b57f4f922223903106db69023c442a94`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:14:48 GMT
ADD file:a8b9aeb23e8f47568ef8ea33a80fee0c676db7c4c9ec9210abf75217a8f329fb in / 
# Fri, 01 Oct 2021 01:14:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:91a226dd2b609e6bc3e70f7621380def71f05b74e75fa1a2f0421795a8904f10`  
		Last Modified: Fri, 01 Oct 2021 01:37:38 GMT  
		Size: 24.2 MB (24227267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4ddabbb8109f098e206abe5dfa64c5429f82353ee50dde5484a1a48c047eb32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27122910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8749b206ce00913c9a567a3f1de60a9462e3014ac383e4c497b5c4d88f475b23`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal-20210921`

```console
$ docker pull ubuntu@sha256:0c00088c0d187ed09be5fe73629fab2387ae3d73d54ce82f9135d8c5e6c6aa52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:focal-20210921` - linux; amd64

```console
$ docker pull ubuntu@sha256:3555f4996aea6be945ae1532fa377c88f4b3b9e6d93531f47af5d78a7d5e3761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28568914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597ce1600cf4ac5f449b66e75e840657bb53864434d6bd82f00b172544c32ee2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210921` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e1a690fbb7b7f117472061b2025132b04ed1a3bbe5e48a3831d4813be7b20223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b3ddfc9fc5db841245f00fbeb98755ae3ab6d49dcb603bd5544ef55e00f15d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210921` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2eedb44775176d77c25c9a69c948b871b67624881e9e46553379443ce788181f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27172405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daab1c66d4670806f6a1890857dc5554a8c5b423ef4399b3fbc5c16022aaef0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210921` - linux; riscv64

```console
$ docker pull ubuntu@sha256:db6aab4e73bc6b1b7e824b693073f79cd706b096e3375187d1395b7c8b37eed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24227267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba84824da1bda6352c1401ef9e4f830b57f4f922223903106db69023c442a94`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:14:48 GMT
ADD file:a8b9aeb23e8f47568ef8ea33a80fee0c676db7c4c9ec9210abf75217a8f329fb in / 
# Fri, 01 Oct 2021 01:14:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:91a226dd2b609e6bc3e70f7621380def71f05b74e75fa1a2f0421795a8904f10`  
		Last Modified: Fri, 01 Oct 2021 01:37:38 GMT  
		Size: 24.2 MB (24227267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20210921` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4ddabbb8109f098e206abe5dfa64c5429f82353ee50dde5484a1a48c047eb32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27122910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8749b206ce00913c9a567a3f1de60a9462e3014ac383e4c497b5c4d88f475b23`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:hirsute`

```console
$ docker pull ubuntu@sha256:44e4ce6defdd88435d6f724b4ed4bfa3dd7796c93012bbe1af16da4a7479a006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:hirsute` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b19ac4988412eaf6ab191ab246d2e1bc9d792ce9a57ef3e97635b41118c4fe9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31704296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f83bfe0b632bd4a5018a57a9c0386564d6ece1645862388200d5a81dae9a7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:54337979c56cc50b52ae70e5531b904e7f34a5d8c383770c75b14f51e5cb26d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26859487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3522c2cf51bd9e4a0315265f0b071fd2fc962ab20f7eeefd29b86b4b79c2c808`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:eb35f49285e58e4baf77e7a5eedeac57f1fdfeb688126a1914e61cb5d19f1ae5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.2 MB (30174163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083fe054c6965dc373db8b9863e89c31abd56aae8ad716c3830e5856c320d9e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:60dfaddf644de61f02ac434ee607fc67123d8c9a6e0b84fcee59211e6cc1a469
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37185952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f685da69c67500e48dad075763bd1bb10bad221d50a72a86abddc20a7a1b4a9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; riscv64

```console
$ docker pull ubuntu@sha256:b2cf15cebd073c22821e0b735d9c70eb108458992f73b73c43f4d14ef3038f04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27141881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faaad95feb654da33d02ceb6c15a5b384f9b432ec1b39e849347675e59eeabc1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute` - linux; s390x

```console
$ docker pull ubuntu@sha256:7341458761704d75f1ed1d436f99ed4be4984e978101c7dcd0a70f93ddc14b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32505539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c69fe2db8ddbdeff2f993f21dc6898446721a1af23b3649ed1556ec1db116d3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:hirsute-20210917`

```console
$ docker pull ubuntu@sha256:ec5d259ccc2623529ef8dfb2db3d2f9106e02d30a713b720c099978bd1c77f7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:hirsute-20210917` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b19ac4988412eaf6ab191ab246d2e1bc9d792ce9a57ef3e97635b41118c4fe9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31704296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f83bfe0b632bd4a5018a57a9c0386564d6ece1645862388200d5a81dae9a7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute-20210917` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:54337979c56cc50b52ae70e5531b904e7f34a5d8c383770c75b14f51e5cb26d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26859487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3522c2cf51bd9e4a0315265f0b071fd2fc962ab20f7eeefd29b86b4b79c2c808`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute-20210917` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:eb35f49285e58e4baf77e7a5eedeac57f1fdfeb688126a1914e61cb5d19f1ae5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.2 MB (30174163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083fe054c6965dc373db8b9863e89c31abd56aae8ad716c3830e5856c320d9e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute-20210917` - linux; riscv64

```console
$ docker pull ubuntu@sha256:b2cf15cebd073c22821e0b735d9c70eb108458992f73b73c43f4d14ef3038f04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27141881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faaad95feb654da33d02ceb6c15a5b384f9b432ec1b39e849347675e59eeabc1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:hirsute-20210917` - linux; s390x

```console
$ docker pull ubuntu@sha256:7341458761704d75f1ed1d436f99ed4be4984e978101c7dcd0a70f93ddc14b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32505539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c69fe2db8ddbdeff2f993f21dc6898446721a1af23b3649ed1556ec1db116d3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:impish`

```console
$ docker pull ubuntu@sha256:9a7b522028ebc43104df4b9d9e3e8b002f4dbe316d6f09464a58306baeed0423
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:impish` - linux; amd64

```console
$ docker pull ubuntu@sha256:b284173fbabcefd6cd4ef871e408d3252b24d762a997323377eaa208240fb72a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30399219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd54db809ce7c0c4a5519431f18e583fc4571e433345ca7deceaa5a1f9fb6ec`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:24:06 GMT
ADD file:14abde46780e9aa8c8c5c54d89baf3f1913aa6fef0d44ecc320cf962c4ba9e4d in / 
# Fri, 01 Oct 2021 02:24:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6122078cc60fecb720ddc58a9f5be50b4112ba9f366d21eccaf834489eafdda5`  
		Last Modified: Fri, 01 Oct 2021 02:25:54 GMT  
		Size: 30.4 MB (30399219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4f92d734b1b459411bf08e3d372425f9fe32778c5379be9b871dcb36445573c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26916992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce570a3a124ab71b3f2a4b517021b2537b380b0eb4cef867bb9d5db03478906f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:55bce25aa903e56698b8ab74c96a9d4de4b152254bf766d2be6f48a02cd886f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29047978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68655ee9aa431faa0081c84edc93a175c59b8f897440c69bd30e69087b91e9cc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8bc56b544223a2ecba0926e57b706514e73ae4ff5ddeab090faed9020d4aa94b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36055099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3e2cffe6f2afc5e5fac69b863b56f13414865b1209ab3f6cfb962f746266c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:28 GMT
ADD file:776487dfd6a31c5a5d57d6924dd11136cb94d2e661eb085c76b14213c2220e3f in / 
# Tue, 31 Aug 2021 02:11:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:7f23233eca55841e558566a0a689d1261b17a023a5d0ed1e0ee267da33ff84a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:11 GMT  
		Size: 36.1 MB (36055099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; riscv64

```console
$ docker pull ubuntu@sha256:6d43cbf9a191da6a33efc5bdc327185ea8363d0ead8a07fbe8590d5a3bdde25c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7f6a349055717cf10ba89991eeded03ccaf3a92888ca35b7a84f56a798688`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; s390x

```console
$ docker pull ubuntu@sha256:8370ebd1ad75d56999ebb386c9a3c9f3bc52e3e38a6096566a867d92bb6ebdf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30770041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4811400563f83422d383472f6ce188a30359e1e4b9534306ebf243f461cd2df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:impish-20210928`

```console
$ docker pull ubuntu@sha256:afc78ed1447cf0a701750f6aee6b6bb98183fcdc0c1c8d002e4153f259dd96ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:impish-20210928` - linux; amd64

```console
$ docker pull ubuntu@sha256:b284173fbabcefd6cd4ef871e408d3252b24d762a997323377eaa208240fb72a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30399219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd54db809ce7c0c4a5519431f18e583fc4571e433345ca7deceaa5a1f9fb6ec`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:24:06 GMT
ADD file:14abde46780e9aa8c8c5c54d89baf3f1913aa6fef0d44ecc320cf962c4ba9e4d in / 
# Fri, 01 Oct 2021 02:24:06 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6122078cc60fecb720ddc58a9f5be50b4112ba9f366d21eccaf834489eafdda5`  
		Last Modified: Fri, 01 Oct 2021 02:25:54 GMT  
		Size: 30.4 MB (30399219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20210928` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4f92d734b1b459411bf08e3d372425f9fe32778c5379be9b871dcb36445573c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26916992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce570a3a124ab71b3f2a4b517021b2537b380b0eb4cef867bb9d5db03478906f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20210928` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:55bce25aa903e56698b8ab74c96a9d4de4b152254bf766d2be6f48a02cd886f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29047978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68655ee9aa431faa0081c84edc93a175c59b8f897440c69bd30e69087b91e9cc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20210928` - linux; riscv64

```console
$ docker pull ubuntu@sha256:6d43cbf9a191da6a33efc5bdc327185ea8363d0ead8a07fbe8590d5a3bdde25c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7f6a349055717cf10ba89991eeded03ccaf3a92888ca35b7a84f56a798688`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20210928` - linux; s390x

```console
$ docker pull ubuntu@sha256:8370ebd1ad75d56999ebb386c9a3c9f3bc52e3e38a6096566a867d92bb6ebdf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30770041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4811400563f83422d383472f6ce188a30359e1e4b9534306ebf243f461cd2df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:51 GMT
ADD file:d4436e6a424f51bbe486f3f4614b547c16e11f0b9e876ac7a4196bba85f65dff in / 
# Fri, 01 Oct 2021 01:42:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:51f9fa2a618c34c6f055c5337e5484b46ec926bf3b8ed93cbe89399bf17c4938`  
		Last Modified: Fri, 01 Oct 2021 01:44:30 GMT  
		Size: 30.8 MB (30770041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:44ab2c3b26363823dcb965498ab06abf74a1e6af20a732902250743df0d4172d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:latest` - linux; amd64

```console
$ docker pull ubuntu@sha256:3555f4996aea6be945ae1532fa377c88f4b3b9e6d93531f47af5d78a7d5e3761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28568914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:597ce1600cf4ac5f449b66e75e840657bb53864434d6bd82f00b172544c32ee2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e1a690fbb7b7f117472061b2025132b04ed1a3bbe5e48a3831d4813be7b20223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b3ddfc9fc5db841245f00fbeb98755ae3ab6d49dcb603bd5544ef55e00f15d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2eedb44775176d77c25c9a69c948b871b67624881e9e46553379443ce788181f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27172405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daab1c66d4670806f6a1890857dc5554a8c5b423ef4399b3fbc5c16022aaef0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8f083e3e070591f3f70ec51abd83d0e6e8b5c92fe4bc79775f50d0a22b8b7021
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33291791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0501f0572349877e5332affe472977acd6e5d4fe071a1cafe69a95dbb9c2c1aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; riscv64

```console
$ docker pull ubuntu@sha256:db6aab4e73bc6b1b7e824b693073f79cd706b096e3375187d1395b7c8b37eed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24227267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba84824da1bda6352c1401ef9e4f830b57f4f922223903106db69023c442a94`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:14:48 GMT
ADD file:a8b9aeb23e8f47568ef8ea33a80fee0c676db7c4c9ec9210abf75217a8f329fb in / 
# Fri, 01 Oct 2021 01:14:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:91a226dd2b609e6bc3e70f7621380def71f05b74e75fa1a2f0421795a8904f10`  
		Last Modified: Fri, 01 Oct 2021 01:37:38 GMT  
		Size: 24.2 MB (24227267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:d4ddabbb8109f098e206abe5dfa64c5429f82353ee50dde5484a1a48c047eb32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27122910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8749b206ce00913c9a567a3f1de60a9462e3014ac383e4c497b5c4d88f475b23`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:44e4ce6defdd88435d6f724b4ed4bfa3dd7796c93012bbe1af16da4a7479a006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b19ac4988412eaf6ab191ab246d2e1bc9d792ce9a57ef3e97635b41118c4fe9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31704296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f83bfe0b632bd4a5018a57a9c0386564d6ece1645862388200d5a81dae9a7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:53 GMT
ADD file:3a18768000089a105cd4f288985d6249e8aee2c742a055a892a47aab413f25c0 in / 
# Fri, 01 Oct 2021 02:23:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:80d63867ecd7f5e4a966c8400729828e902773a9f03109a2ec69605ddc8045a9`  
		Last Modified: Fri, 01 Oct 2021 02:25:36 GMT  
		Size: 31.7 MB (31704296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:54337979c56cc50b52ae70e5531b904e7f34a5d8c383770c75b14f51e5cb26d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26859487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3522c2cf51bd9e4a0315265f0b071fd2fc962ab20f7eeefd29b86b4b79c2c808`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:26 GMT
ADD file:0ecbd9f51121128f5d6ca097a4f697705e11f91abe0a7f83083e18bceeeddfef in / 
# Sat, 02 Oct 2021 05:59:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:615bdbfbc600b147544d8c25eedf00ddb7eebaf2e9005c1da9f5885a6bbc6c1d`  
		Last Modified: Sat, 02 Oct 2021 06:03:33 GMT  
		Size: 26.9 MB (26859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:eb35f49285e58e4baf77e7a5eedeac57f1fdfeb688126a1914e61cb5d19f1ae5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.2 MB (30174163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083fe054c6965dc373db8b9863e89c31abd56aae8ad716c3830e5856c320d9e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:04 GMT
ADD file:36081e580b6851b0f8a1176a307b99a673510dc87809a726cad514bd7f56d620 in / 
# Fri, 01 Oct 2021 02:44:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e61beefb4313333ca27a602845cbf2a6f7cba9c176bb999f14a4bdcfb6a54148`  
		Last Modified: Fri, 01 Oct 2021 02:46:09 GMT  
		Size: 30.2 MB (30174163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:60dfaddf644de61f02ac434ee607fc67123d8c9a6e0b84fcee59211e6cc1a469
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37185952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f685da69c67500e48dad075763bd1bb10bad221d50a72a86abddc20a7a1b4a9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:11:01 GMT
ADD file:28ec82d5664675df3fbd80ea2405c9f6441adb338e5969157339ef7d3b9cb690 in / 
# Tue, 31 Aug 2021 02:11:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:76dbcd36047f3dda1663b45891fb64b9bb6c0ef0e5611c1f8280ac85e57cc7af`  
		Last Modified: Tue, 31 Aug 2021 02:14:46 GMT  
		Size: 37.2 MB (37185952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; riscv64

```console
$ docker pull ubuntu@sha256:b2cf15cebd073c22821e0b735d9c70eb108458992f73b73c43f4d14ef3038f04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27141881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faaad95feb654da33d02ceb6c15a5b384f9b432ec1b39e849347675e59eeabc1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:16:46 GMT
ADD file:3e74b3f99e917f6242f9460c55d6b1ed2c4e243bb9deeef85c260be1e6c3b3b7 in / 
# Fri, 01 Oct 2021 01:16:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cfe1f0adec8bd7640ec8d5467a7a5553e6d58e6cb80adbbc101495501625dca9`  
		Last Modified: Fri, 01 Oct 2021 01:40:30 GMT  
		Size: 27.1 MB (27141881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:7341458761704d75f1ed1d436f99ed4be4984e978101c7dcd0a70f93ddc14b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32505539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c69fe2db8ddbdeff2f993f21dc6898446721a1af23b3649ed1556ec1db116d3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:40 GMT
ADD file:fcf310d9f4d95ff5ed13b1e66aa2a62f163b9bcfc9e9fdbae5af11f19dd0bd85 in / 
# Fri, 01 Oct 2021 01:42:42 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9e74faf81dfb98c642fd37930279e8a6538c4ce035807bab59ed0f1d0a0eb627`  
		Last Modified: Fri, 01 Oct 2021 01:44:16 GMT  
		Size: 32.5 MB (32505539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty`

```console
$ docker pull ubuntu@sha256:43cb19408de1e0ecf3ba5b5372ec98978963d6d0be42d0ad825e77a3bd16b5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:trusty` - linux; amd64

```console
$ docker pull ubuntu@sha256:881afbae521c910f764f7187dbfbca3cc10c26f8bafa458c76dda009a901c29d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b66b487594a1f2b75396013bc05d29d9f527852d96c5577cc4f187559875d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:40 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 25 Mar 2021 22:33:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551a797c01db074ab0233ceb567e66b8ebdcb9de9a2e7baa36d57dfbca463a3`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 72.7 KB (72664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512123a864da5e2a62949e65b67106292c5c704eff90cac2b949fc8d7ac1e58e`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:534255069ef3adf1c7a555fd9f614845ab66c61ef9846e438d86e12ae8c89b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2cd03315989aa8326f2c276922d3969994c1304b1310d2e0d33a26d94dd68ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:23:03 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Tue, 13 Jul 2021 23:23:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:23:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 13 Jul 2021 23:23:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:23:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c5cd1be699257153c2a6de85968c2d9c413d87470dc4f540c5c3decbca8e47`  
		Last Modified: Tue, 13 Jul 2021 23:28:27 GMT  
		Size: 76.8 KB (76774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf1c32ebce749806713a088af6ff1cbf7c75a8132d310ff391948e3e611ef6`  
		Last Modified: Tue, 13 Jul 2021 23:28:26 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:0fe9a82e42e32a74cca83fc84d5ab80b2ef73b7b90b7bab661b00ef3d16bfad9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:423c4ed354ff1af8b464f13e25792ddb5e0a2c6baa22b5af909e68b557062eec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 May 2021 12:30:34 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Thu, 27 May 2021 12:30:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 27 May 2021 12:30:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 27 May 2021 12:30:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 27 May 2021 12:30:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e84a55d935eb29baa4a459e89f330e090e7f9db90fbdd96f6c47b89c614c671`  
		Last Modified: Thu, 27 May 2021 12:33:16 GMT  
		Size: 59.1 KB (59096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a9c88d39064b3377476bafe5b4a86f498750df033058cc4a61194f2ca5540b`  
		Last Modified: Thu, 27 May 2021 12:33:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; 386

```console
$ docker pull ubuntu@sha256:88152195106ff09bade23cb5aacfd26c381a8835c9d42124b4cba1dc3c2475e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ba408bae1426c4f394e045b16a140bc555e520d5eaacc97ac60ac5f298313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:57:06 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 25 Mar 2021 22:57:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:57:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea2d50b5278097c6d027fc9fc0caf006649fcd94f094dde6ce578abe865ff21`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:12d9fa858f255e4b70827aff83e8ce37b6fcaddaf6732276aa1f0763402f4fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02949c650aebaafb917ebe6bfd55a42505e22b38e8370878164051da4ae1bcc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:24:04 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Tue, 13 Jul 2021 23:24:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:24:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 13 Jul 2021 23:24:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:24:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aab203a69be44b1617f0da6b00b670e9016c3b00ab311b384ac3f859e86613`  
		Last Modified: Tue, 13 Jul 2021 23:29:07 GMT  
		Size: 63.4 KB (63430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1576c78d220b27404b5d0c3d635c36524229553e3ccf3b9a5ad4ca93c216c6c6`  
		Last Modified: Tue, 13 Jul 2021 23:29:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty-20191217`

```console
$ docker pull ubuntu@sha256:43cb19408de1e0ecf3ba5b5372ec98978963d6d0be42d0ad825e77a3bd16b5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:trusty-20191217` - linux; amd64

```console
$ docker pull ubuntu@sha256:881afbae521c910f764f7187dbfbca3cc10c26f8bafa458c76dda009a901c29d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b66b487594a1f2b75396013bc05d29d9f527852d96c5577cc4f187559875d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:40 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 25 Mar 2021 22:33:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551a797c01db074ab0233ceb567e66b8ebdcb9de9a2e7baa36d57dfbca463a3`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 72.7 KB (72664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512123a864da5e2a62949e65b67106292c5c704eff90cac2b949fc8d7ac1e58e`  
		Last Modified: Thu, 25 Mar 2021 22:35:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:534255069ef3adf1c7a555fd9f614845ab66c61ef9846e438d86e12ae8c89b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2cd03315989aa8326f2c276922d3969994c1304b1310d2e0d33a26d94dd68ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:23:03 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Tue, 13 Jul 2021 23:23:06 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:23:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 13 Jul 2021 23:23:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:23:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c5cd1be699257153c2a6de85968c2d9c413d87470dc4f540c5c3decbca8e47`  
		Last Modified: Tue, 13 Jul 2021 23:28:27 GMT  
		Size: 76.8 KB (76774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf1c32ebce749806713a088af6ff1cbf7c75a8132d310ff391948e3e611ef6`  
		Last Modified: Tue, 13 Jul 2021 23:28:26 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:0fe9a82e42e32a74cca83fc84d5ab80b2ef73b7b90b7bab661b00ef3d16bfad9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:423c4ed354ff1af8b464f13e25792ddb5e0a2c6baa22b5af909e68b557062eec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 27 May 2021 12:30:34 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Thu, 27 May 2021 12:30:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 27 May 2021 12:30:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 27 May 2021 12:30:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 27 May 2021 12:30:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e84a55d935eb29baa4a459e89f330e090e7f9db90fbdd96f6c47b89c614c671`  
		Last Modified: Thu, 27 May 2021 12:33:16 GMT  
		Size: 59.1 KB (59096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a9c88d39064b3377476bafe5b4a86f498750df033058cc4a61194f2ca5540b`  
		Last Modified: Thu, 27 May 2021 12:33:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; 386

```console
$ docker pull ubuntu@sha256:88152195106ff09bade23cb5aacfd26c381a8835c9d42124b4cba1dc3c2475e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18ba408bae1426c4f394e045b16a140bc555e520d5eaacc97ac60ac5f298313`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:57:06 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 25 Mar 2021 22:57:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:57:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea2d50b5278097c6d027fc9fc0caf006649fcd94f094dde6ce578abe865ff21`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:12d9fa858f255e4b70827aff83e8ce37b6fcaddaf6732276aa1f0763402f4fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02949c650aebaafb917ebe6bfd55a42505e22b38e8370878164051da4ae1bcc3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:24:04 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Tue, 13 Jul 2021 23:24:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:24:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 13 Jul 2021 23:24:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:24:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aab203a69be44b1617f0da6b00b670e9016c3b00ab311b384ac3f859e86613`  
		Last Modified: Tue, 13 Jul 2021 23:29:07 GMT  
		Size: 63.4 KB (63430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1576c78d220b27404b5d0c3d635c36524229553e3ccf3b9a5ad4ca93c216c6c6`  
		Last Modified: Tue, 13 Jul 2021 23:29:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial`

```console
$ docker pull ubuntu@sha256:454054f5bbd571b088db25b662099c6c7b3f0cb78536a2077d54adc48f00cd68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial` - linux; amd64

```console
$ docker pull ubuntu@sha256:a3785f78ab8547ae2710c89e627783cfa7ee7824d3468cae6835c9f4eae23ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46499103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f50765242581c887ff1acc2511fa2d885c52d8fb3ac8c4bba131fd86567f2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:b722e2654241f9681f4719dce7aa16a2f0c35769e17a636f5b39a33967d1aeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40313783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033c410d53efaab9e847168b94fea14d551788200a15f4d2424c84e4cd2ab8a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:11c7a73a8eb322a177481fdeafc34957200f2f0d1f2192044ad5262008d4bba9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6834beb45bf45c3a0423173bc99b6c7f1ae051b0187febdf9b9e780beac78af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; 386

```console
$ docker pull ubuntu@sha256:4a6759446930ee402a2091605c0911f237ad18b5c250a535d11563d9402eb15a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac20e7c3411697a4a85c1cb30850f77b8238e0a0ef0e176ca8f0e763066eed4b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cf25d111d193288d47d20a4e5d42a68dc2af24bb962853b067752eca3914355e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47523633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914466c340b7c02825333f4de2597bcd673f18eb0cec83840b13a3cc68338937`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; s390x

```console
$ docker pull ubuntu@sha256:5fea5a070916f61785140faa8e16fa8bf7ca3f152ceed9c48154f8aca4c3667e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb8683432fbdd1ec03145305370c4ec7079b01e22fcc47dd4df1aa862463474`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial-20210804`

```console
$ docker pull ubuntu@sha256:454054f5bbd571b088db25b662099c6c7b3f0cb78536a2077d54adc48f00cd68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial-20210804` - linux; amd64

```console
$ docker pull ubuntu@sha256:a3785f78ab8547ae2710c89e627783cfa7ee7824d3468cae6835c9f4eae23ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46499103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f50765242581c887ff1acc2511fa2d885c52d8fb3ac8c4bba131fd86567f2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:b722e2654241f9681f4719dce7aa16a2f0c35769e17a636f5b39a33967d1aeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40313783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033c410d53efaab9e847168b94fea14d551788200a15f4d2424c84e4cd2ab8a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:28 GMT
ADD file:294a94a081de785c730003a440a0530a85add2bcb60c0f5bc4ce7ee17867ac4e in / 
# Tue, 31 Aug 2021 01:42:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:42:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:42:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:42:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b95ba076a26b98e98eac4b43596b59c20d1e61a36bcaf2afae3aeebadc8844cf`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 40.3 MB (40312250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48547e29bdd75abab2cbd318d0739f4092117ce9d04e7b8f20c36674abd65e59`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebef378167277f2a504e20691b3f74632e59e23c5761cb5e602a634aa32b1b9`  
		Last Modified: Tue, 31 Aug 2021 01:46:37 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97155dfcb43995751a1533d2e37802f3b35f78bd9b0eaf5049f79f56199ac90`  
		Last Modified: Tue, 31 Aug 2021 01:46:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:11c7a73a8eb322a177481fdeafc34957200f2f0d1f2192044ad5262008d4bba9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6834beb45bf45c3a0423173bc99b6c7f1ae051b0187febdf9b9e780beac78af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; 386

```console
$ docker pull ubuntu@sha256:4a6759446930ee402a2091605c0911f237ad18b5c250a535d11563d9402eb15a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac20e7c3411697a4a85c1cb30850f77b8238e0a0ef0e176ca8f0e763066eed4b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:31 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 31 Aug 2021 01:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:39:33 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:39:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250dcd0b24a66322cdee2165435035a76e5b72085df234bfcdc340c5321c74d`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3c7bbf9087c9dae9eb48a2b2a913146a0705560689407ee02802ff92408abf`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea45938bfbd7dd3f314ea2ad08a94370db722a20c33d6407c8eaeaf906b40c5`  
		Last Modified: Tue, 31 Aug 2021 01:40:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cf25d111d193288d47d20a4e5d42a68dc2af24bb962853b067752eca3914355e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47523633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914466c340b7c02825333f4de2597bcd673f18eb0cec83840b13a3cc68338937`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:12:03 GMT
ADD file:c84969ed4d4e336ec5996e26e35261f683b36f1af7a978df587296ef5e7a2627 in / 
# Tue, 31 Aug 2021 02:12:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 02:12:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 02:12:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5057452c10cfe2216f39949f909f3cd83002d256d1bbd564ae242352a5460fe2`  
		Last Modified: Sun, 08 Aug 2021 01:00:30 GMT  
		Size: 47.5 MB (47522137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c76cb7ccfe1638448c02d9e8f51fae873202f130515c9fb7a791038a2bd9586`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a12ad70abdfd318d55001c9a70e7eccffb1f5ece5eee88d8e4e549083928a9`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d97c60bc4668c8613c3ef5ffe0205d9be50368dfe09cb0859beb030ed103`  
		Last Modified: Tue, 31 Aug 2021 02:15:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; s390x

```console
$ docker pull ubuntu@sha256:5fea5a070916f61785140faa8e16fa8bf7ca3f152ceed9c48154f8aca4c3667e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb8683432fbdd1ec03145305370c4ec7079b01e22fcc47dd4df1aa862463474`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:43:07 GMT
ADD file:8719dec76e2491e6bcc4cba5072d8123bd3472e72108280ea29f6a34761adbeb in / 
# Tue, 31 Aug 2021 01:43:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:43:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:43:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:43:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:80d499f9d46bfeec5260ce5a395259ab5e54118e786a0e9023d6550a57730bd4`  
		Last Modified: Tue, 31 Aug 2021 01:45:04 GMT  
		Size: 44.1 MB (44087722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883d7cfe3e67b3dd7ffd87697a9050dfad287116e1f38ed165b815d7285a7d70`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e68cf162fecf9f82ab0d540cd0f3af1a4a74defc8ba9434379cbae3a09b30c`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfcc45f37d760e154b69274e44e31fd64b8537f3cb1cba39203b537246bc891`  
		Last Modified: Tue, 31 Aug 2021 01:44:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
