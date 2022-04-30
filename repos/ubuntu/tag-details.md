<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:14.04`](#ubuntu1404)
-	[`ubuntu:16.04`](#ubuntu1604)
-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:21.10`](#ubuntu2110)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:22.10`](#ubuntu2210)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20220427`](#ubuntubionic-20220427)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20220426`](#ubuntufocal-20220426)
-	[`ubuntu:impish`](#ubuntuimpish)
-	[`ubuntu:impish-20220427`](#ubuntuimpish-20220427)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20220428`](#ubuntujammy-20220428)
-	[`ubuntu:kinetic`](#ubuntukinetic)
-	[`ubuntu:kinetic-20220428`](#ubuntukinetic-20220428)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:rolling`](#ubunturolling)
-	[`ubuntu:trusty`](#ubuntutrusty)
-	[`ubuntu:trusty-20191217`](#ubuntutrusty-20191217)
-	[`ubuntu:xenial`](#ubuntuxenial)
-	[`ubuntu:xenial-20210804`](#ubuntuxenial-20210804)

## `ubuntu:14.04`

```console
$ docker pull ubuntu@sha256:96a36dd3bcd8f149fa9874c4e28c35c01f715b3e5f8f1a8e06b45887619bf43b
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
$ docker pull ubuntu@sha256:5dc82d0f897a1bfd6a68db5b2c3692d81e5ea04e31a09664edc420689f8b450c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7304c635fe5273ccdfbc8a38e839c9089350fc8e80daf57394d1f7a9c5a70c86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:09 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Sat, 16 Oct 2021 01:48:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 16 Oct 2021 01:48:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fc464c2dc9f9ce8d7fe9ccd36f4e746ce32b39f19590f519a8cd3dd76827f8`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 59.1 KB (59100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561f253b7549524704fe8cc1da5ebd27d77bc1a1424b0632b683d90eb58e73d3`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; 386

```console
$ docker pull ubuntu@sha256:c97d63976268e6c2f3764be91e59f82009b2883d22c3dc6ff1f63e3ad6abdb05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a7710ba73fd21ad01442fe2b079693c60a5b77b18403d56e5da5448e325d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:14 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Tue, 05 Apr 2022 22:39:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 05 Apr 2022 22:39:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03124bfb4886d9ba012a00a087fb41b4cc7e99517b3e2a2e6fd1e2ad327af191`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b953ad705784700c1611b7258f6c783a34b06bf27ed3efbd9acc7be80ba991`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 162.0 B  
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
$ docker pull ubuntu@sha256:20858ebbc96215d6c3c574f781133ebffdc7c18d98af4f294cc4c04871a6fe61
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
$ docker pull ubuntu@sha256:70fa660340a344b46cc56b3606dc8abd3bf48b5cbce13d01c720e9793a6bc3c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b34cb9255c8dd390f85c8fe37e6fbe6ac555f86c7e8944cd68da2de2f7633`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; 386

```console
$ docker pull ubuntu@sha256:bcb8397f1390f4f0757ca06ce184f05c8ce0c7a4b5ff93f9ab029a581192917b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276b5b6b7721e99481801a9aaf21a4d2bf6ba6f6676f720f6f4e0da40a71fb19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
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
$ docker pull ubuntu@sha256:d21b6ba9e19feffa328cb3864316e6918e30acfd55e285b5d3df1d8ca3c7fd3f
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
$ docker pull ubuntu@sha256:971a12d7e92a23183dead8bfc415aa650e7deb1cc5fed11a3d21f759a891fde9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26709108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ad7e71ba7d4969784c76f57c4cc9083aa96bb969d802f2ea38f4aaed90ff93`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ec5715e4fd292b212edd9062c1abe247298ed3acf87b9555b55cc9b16e7f628a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22300451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:998a0018caa18ee34b520e0ab73417aefdd24abfb7492fb5aa4cecb0a7ce3466`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:25 GMT
ADD file:9604e3641a386ec134596dd717862c2386c1b90009c0646b1773930f98949d9c in / 
# Fri, 29 Apr 2022 22:58:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:03ca5b55b2bdc3c68d23c18a88c099e2015c6bdcef6e3c43ca0bfb6aea0b032a`  
		Last Modified: Fri, 29 Apr 2022 23:02:31 GMT  
		Size: 22.3 MB (22300451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:6f911cac13c27a4f9936b949161f57f1fd27228b821e9912815fa941dc7bec7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23735089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6f13ca5102d1f202c195aa84a99fb434853f3e039bf9610e6cb771e8d52bf8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:a7ed45c4a95fbe19f9c5fb9d1ca58b2431b2a4984754be2f50ccec99d9428b79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27164138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7676d532710d57b644a18d0c7428c1dd9bff21a26620a9ea60cf4cf1018bc3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:46:47 GMT
ADD file:bcce1e9e400660e474d54b70b67bc484a7976aff4e980b58d10ddcb4daa58a7f in / 
# Fri, 29 Apr 2022 22:46:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:14c49d5e021ef38e29480c34c86df22d89b9b63fe1a57ec4dd970f56497edf9a`  
		Last Modified: Fri, 29 Apr 2022 22:47:32 GMT  
		Size: 27.2 MB (27164138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:740a942c894a06e2e490f6f17b470409fa62e34eea7ab6c2c0c73be7f242277c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30443183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb6ac865363641875a604c1ac20e4c665b6f62f40d3f9dd5227799da41fb957`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:2e9f488d35790e264437c71bd6774aec0704432d91d8c73bb0c599143729371f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25365828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edafd08d1799b5c8023f02483d4f15f7e2b52dd3e38fa647502d36d37a63899`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:47f14534bda344d9fe6ffd6effb95eefe579f4be0d508b7445cf77f61a0e5724
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
$ docker pull ubuntu@sha256:9d42d0e3e57bc067d10a75ee33bdd1a5298e95e5fc3c5d1fce98b455cb879249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28566230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53df61775e8856a464ca52d4cd9eabbf4eb3ceedbde5afecc57e417e7b7155d5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:681dcdedc7ac9708764c1018cb9785907298c490cee08717ce57d401258ac876
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24073650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3dbf2c88b9eed84cee7427e9fc590a188443d72668941196c7395d8af26dc2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:ca83774d06420ceb4682ef73bd9cbbfc38a97a27e061b578547a6761206658b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27169388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1bc6aa58da386bc4ae8c4489e0bda0f6073c49a7b6c2ca24386671b36a1f19`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:55da61c5ad752c43ad671b0bc16a0496371b98d85dcc4cd4dc735c695cced298
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33290661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8c2a68f557812cf6d4826032f0cd968647c228f3ac23b82a5b518165d6b34d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; riscv64

```console
$ docker pull ubuntu@sha256:4df7126c32c74eb9b734113d03545aa1ac4938b91319fbfe8cb693b94adfc6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24228241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1e2591ecd338320e77f4377aae51c48f3de7128de9fb27bdb3a888dd4781d4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:14:50 GMT
ADD file:77e925ea3ddf0d01534094175d808508c4a5d0535f08d304994323efb0173a57 in / 
# Fri, 29 Apr 2022 23:14:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:63ac7876cbf81a317a4c88c281171f026148a0f62b17284f294a5f0eb06bb383`  
		Last Modified: Fri, 29 Apr 2022 23:36:48 GMT  
		Size: 24.2 MB (24228241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:4ca42ab690fab0df13fb1c8f79cdb7d6307442d83abe776d6c9b647b48b09d62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27065417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5571b2169962786dfe503560491daf168d8b9b774d818d4f2ec789f2fa3cc53`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:21.10`

```console
$ docker pull ubuntu@sha256:14d8cab8d7bd72a01e225cd85bf37bbf08bf88115769316fa86c776df4ea5fed
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
$ docker pull ubuntu@sha256:253908b2844746ab3f3a08fc8a44b9b9fc1efc408d5969b093ab9ffa11eb1894
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30383364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:565852265961284e5715ccd6f1a20339c4b0448d7649d76e3abbd4fafab3adc4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:07 GMT
ADD file:e36038a1f6ee02f3f9a7db183e116f58d277e97cb7e71032634097d802654d02 in / 
# Fri, 29 Apr 2022 23:21:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:940122ec7d0c039d048e3bf953a33cd8ef814fd587266a5e732d24d2314af8f1`  
		Last Modified: Fri, 29 Apr 2022 23:22:38 GMT  
		Size: 30.4 MB (30383364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:51927bb029ae20b80e128ab2c5620163a1b89975d4cbed6f56eab57ca591f5f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26920477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a66381c8346b8424a3114f9d6db5e4d331759c66ce3cce459e427d53b1ddf3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:09 GMT
ADD file:98b792cccd674eb149eee0fddc60ebe9484757384fe35630fc361ecfc28f9e42 in / 
# Fri, 29 Apr 2022 22:59:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2a09877f6132d465ce4f615f0c5f4bb1dc0e311ce406712beced416d3257e69c`  
		Last Modified: Fri, 29 Apr 2022 23:03:29 GMT  
		Size: 26.9 MB (26920477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:330330705b92fe325e550f8d35519f2213e1168df212cf8095ea10db63fb6afa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29029534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771a596909ab10d1a46e672acfdae2b4ecae9896feb006e47a62f826f30128dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:43 GMT
ADD file:d800d571fc22b337baaf45095bd1a303ca66065106c8b943a7a869e145896077 in / 
# Fri, 29 Apr 2022 22:49:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:924f038c577f5fb37fec4317d1c44a40bae2f6ee798dc0e31394270b30d69e8d`  
		Last Modified: Fri, 29 Apr 2022 22:51:50 GMT  
		Size: 29.0 MB (29029534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:0d276731b94e2e3853de594483da216a28f7d85d99e54e08cc1d0b7ce88b0678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36172344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6000d2ac9546a6047aae9606bceb162b9217c1174d3a82e78eff866c1f7eb6fd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:47 GMT
ADD file:6fee77e76b27182351bc3f1670478775d45b940b676a9c68b3057638166e1f3e in / 
# Fri, 29 Apr 2022 23:22:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b9131999f6427d8e2f8c2e6af3dc4889e32c5ea861065b2f8c24539e9c7d81a`  
		Last Modified: Fri, 29 Apr 2022 23:25:51 GMT  
		Size: 36.2 MB (36172344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; riscv64

```console
$ docker pull ubuntu@sha256:12121497838f0eeede99311646bc3684fec38672f9bdcb6b4200dd88f85a8271
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18096f6eeb14bbd454bbf5ef5981db09e489f8c622df7e2148260a78d279870c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:16:52 GMT
ADD file:9b1d81091b302d999994d0aff49d52975044c0786e8d7aa0df0ce41ec3c5902b in / 
# Fri, 29 Apr 2022 23:16:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3105f98235ad0afa0e8e8fb758ef0e3a7fa3bc505fc19f49da0968611aa32271`  
		Last Modified: Fri, 29 Apr 2022 23:39:06 GMT  
		Size: 27.2 MB (27210922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:21.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:b8fd502cf99110f83f77a46ce35d1be1cc3a2a22a32207160220ac2b1daaf377
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30502867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a417516b88a5eadd6c55194447e00a7a78c4a559e7d739f16fc763cd6b434982`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:17 GMT
ADD file:1041ef5c07ca82ee2d7f626a60380e731aa09d0d2b9b6877b03abffa280e452b in / 
# Fri, 29 Apr 2022 22:50:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fe0d74cf06c14c44f5210e7c3b5af279f02a1d45707ee11e6afae132344bf765`  
		Last Modified: Fri, 29 Apr 2022 22:52:13 GMT  
		Size: 30.5 MB (30502867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:26c68657ccce2cb0a31b330cb0be2b5e108d467f641c62e13ab40cbec258c68d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:22.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:aa6c2c047467afc828e77e306041b7fa4a65734fe3449a54aa9c280822b0d87d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30421006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e4e1f511320dfb2d0baff2468fcf0526998b73fe10c8890b4684bb7ef8290f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:58ddb1588a8c0304cd3dbdb81bdd40bee55ab67dcd4e9938ec167728bde5ae54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4454e2e75bf4628b8547fb60b3753c9ce8cf250f6e86c944155b45873be77504`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e01a1e915645f9240d02ab90cc15da706b4dee508025785dd0538bb3fc7f859
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d495355b4ebc1367b0a666d029e8bd1f8cb3a85d1ecd0bbe5e20138c37e155`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1ed6cb877f3697c3fa7cdd1cf2e6c5c496fc1ab84ac6d020c9533fff23c8f897
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1a9b14de904dc06d5041a4a4ecd65ff2fa3a66c0a088e831db7d83a26ca0b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:05 GMT
ADD file:db27920209849d42ecc46854d40c0f2c71346054166d0a2e37cc3c0361362391 in / 
# Fri, 29 Apr 2022 23:23:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4cf58bb815afda02904690ca8e3231fd4a3c7c0bfc79bd44118ca3720f18a2cd`  
		Last Modified: Fri, 29 Apr 2022 23:26:14 GMT  
		Size: 35.7 MB (35719376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; riscv64

```console
$ docker pull ubuntu@sha256:904dcdf5747aeeb016cfa00ccd4c25f0baedbae5b6bcd834b38bf47ebcce2783
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a98b3afd049e95d4a4cd74ddc36a0bd0292ee3ea7eba7da6f610367fb2b64b9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:18:56 GMT
ADD file:7350517b53b7fc7556b4df07b2d762e16a9797b68f4760d536321210c8acfd34 in / 
# Fri, 29 Apr 2022 23:18:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29912c87e17183ec23ae82771552de74ad581040d14b5d35e5678e1409ca9a66`  
		Last Modified: Fri, 29 Apr 2022 23:41:25 GMT  
		Size: 27.7 MB (27745174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:c18eff699e090d6b0336dda55b9f83cbbdf126100aa06d16de4fc58e2fa740df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277242fcbfea4007bf94af719bb1c8007b5af5f3ce6942bd3ef798dd73422ab9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:88c79ab062b79c8fe13036065334ecabb3bc2f302f08fcb887a2afc7f80cfa2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:22.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:fb5104deb0ffa22606091c5fc569d7c013e826a58cf9c3d0dedcb7e99ac21cd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30420973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f60b19cdd3178764b1a6c6b19220e3396d5671816b51bb894027fde4a7ac8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:23 GMT
ADD file:ebe265aac135a4affe0b35a5e79cd43480dc94796fba7b04095ff6dd92c42359 in / 
# Fri, 29 Apr 2022 23:21:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0ca6c954284ce98aea2c55589ebabd347d2caf3ba94387f53b5339c1f35ab8b7`  
		Last Modified: Fri, 29 Apr 2022 23:23:13 GMT  
		Size: 30.4 MB (30420973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:99139ea3b12bc75ee149bd32c1e4d295bcfd25002d2e0d857696b3df3c252647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a4f900232301f0c95d7d758c05cb05b1d3f1a9b8f8e2ccdad3c23cd88a4653`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:55 GMT
ADD file:063f432f8adfa6ad56a7bb07ff90f71f00c47c30a03bd892e04ddd744042a0d3 in / 
# Fri, 29 Apr 2022 22:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1fc430d8f49d4d10815388bc3cb533e89d8123bcc10ffd2a333c16216f2e4303`  
		Last Modified: Fri, 29 Apr 2022 23:04:36 GMT  
		Size: 27.0 MB (27015929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:27daec02acc728d62b293e954981c142333eb8dfd8ce4bfd75eac008f5528d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c907287071226ba97298d35b0990fa71f8103054147bf36e2946589478c5ce2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:02 GMT
ADD file:1dcfa00d31cec211ba91522ed6fcf6f72e3f1f4ad30c4f7ca398add7eba377c0 in / 
# Fri, 29 Apr 2022 22:50:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:957fa4daed10cc16359daab2a50b5ffbbc1d762035c4eba567b3d4205e7afbde`  
		Last Modified: Fri, 29 Apr 2022 22:52:30 GMT  
		Size: 28.4 MB (28376165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:045009e9203b47686922bea14515bdbcbb168459bdc987b67e2d6713340de4c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5a463bb8a2d14a5b936418198de915b0021f6efea27d2a68b6366091fc9b91`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:22 GMT
ADD file:255691256b47d5fe6ed4871151edc57eb15be171ec05706f4ac6e574bdaff407 in / 
# Fri, 29 Apr 2022 23:23:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:314e7db37887c48e6b822759045272201a6ed3ff0bb4f89f164f9f3ff64cacaa`  
		Last Modified: Fri, 29 Apr 2022 23:26:43 GMT  
		Size: 35.7 MB (35719018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; riscv64

```console
$ docker pull ubuntu@sha256:c18733fbe1d10983c42f8db215657467128ad8f638d3fdd61bdf0f88e04b5220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd76126609e952f9a5820b162ac407928a97012de59f5a1909c2af75963dcd9a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:28 GMT
ADD file:88e52fba8a3ffc283333df24e0d115ab58328ac1d5f6cf585d17422676e146d3 in / 
# Fri, 29 Apr 2022 23:21:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5e53595b65ef34f5f4d764d94e324a0b884612b1b49f768cdd94321c4f22fefd`  
		Last Modified: Fri, 29 Apr 2022 23:44:55 GMT  
		Size: 27.7 MB (27745108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:8ce2906f39c6d06e337ad8b5ed647dd304ed1a1fa7ee54eab38cc1d5707610fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00438fda1e2923dd12f8d9a545ca5cb1e13a0a6ff5e38ee519c634f280f5207e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:44 GMT
ADD file:55affb702d0be7976581cacdb7c77f2c1b0d6921d2cd689a427471c2fd9d4daf in / 
# Fri, 29 Apr 2022 22:50:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c551bbcabccfb0977b8a9e2ba72099b05f9ba8b7c7106d8a29073b45bc73a9a4`  
		Last Modified: Fri, 29 Apr 2022 22:52:38 GMT  
		Size: 28.6 MB (28637139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:d21b6ba9e19feffa328cb3864316e6918e30acfd55e285b5d3df1d8ca3c7fd3f
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
$ docker pull ubuntu@sha256:971a12d7e92a23183dead8bfc415aa650e7deb1cc5fed11a3d21f759a891fde9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26709108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ad7e71ba7d4969784c76f57c4cc9083aa96bb969d802f2ea38f4aaed90ff93`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ec5715e4fd292b212edd9062c1abe247298ed3acf87b9555b55cc9b16e7f628a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22300451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:998a0018caa18ee34b520e0ab73417aefdd24abfb7492fb5aa4cecb0a7ce3466`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:25 GMT
ADD file:9604e3641a386ec134596dd717862c2386c1b90009c0646b1773930f98949d9c in / 
# Fri, 29 Apr 2022 22:58:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:03ca5b55b2bdc3c68d23c18a88c099e2015c6bdcef6e3c43ca0bfb6aea0b032a`  
		Last Modified: Fri, 29 Apr 2022 23:02:31 GMT  
		Size: 22.3 MB (22300451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:6f911cac13c27a4f9936b949161f57f1fd27228b821e9912815fa941dc7bec7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23735089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6f13ca5102d1f202c195aa84a99fb434853f3e039bf9610e6cb771e8d52bf8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:a7ed45c4a95fbe19f9c5fb9d1ca58b2431b2a4984754be2f50ccec99d9428b79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27164138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7676d532710d57b644a18d0c7428c1dd9bff21a26620a9ea60cf4cf1018bc3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:46:47 GMT
ADD file:bcce1e9e400660e474d54b70b67bc484a7976aff4e980b58d10ddcb4daa58a7f in / 
# Fri, 29 Apr 2022 22:46:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:14c49d5e021ef38e29480c34c86df22d89b9b63fe1a57ec4dd970f56497edf9a`  
		Last Modified: Fri, 29 Apr 2022 22:47:32 GMT  
		Size: 27.2 MB (27164138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:740a942c894a06e2e490f6f17b470409fa62e34eea7ab6c2c0c73be7f242277c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30443183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb6ac865363641875a604c1ac20e4c665b6f62f40d3f9dd5227799da41fb957`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:2e9f488d35790e264437c71bd6774aec0704432d91d8c73bb0c599143729371f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25365828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edafd08d1799b5c8023f02483d4f15f7e2b52dd3e38fa647502d36d37a63899`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic-20220427`

```console
$ docker pull ubuntu@sha256:d21b6ba9e19feffa328cb3864316e6918e30acfd55e285b5d3df1d8ca3c7fd3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic-20220427` - linux; amd64

```console
$ docker pull ubuntu@sha256:971a12d7e92a23183dead8bfc415aa650e7deb1cc5fed11a3d21f759a891fde9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26709108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ad7e71ba7d4969784c76f57c4cc9083aa96bb969d802f2ea38f4aaed90ff93`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220427` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ec5715e4fd292b212edd9062c1abe247298ed3acf87b9555b55cc9b16e7f628a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22300451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:998a0018caa18ee34b520e0ab73417aefdd24abfb7492fb5aa4cecb0a7ce3466`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:25 GMT
ADD file:9604e3641a386ec134596dd717862c2386c1b90009c0646b1773930f98949d9c in / 
# Fri, 29 Apr 2022 22:58:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:03ca5b55b2bdc3c68d23c18a88c099e2015c6bdcef6e3c43ca0bfb6aea0b032a`  
		Last Modified: Fri, 29 Apr 2022 23:02:31 GMT  
		Size: 22.3 MB (22300451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220427` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:6f911cac13c27a4f9936b949161f57f1fd27228b821e9912815fa941dc7bec7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.7 MB (23735089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6f13ca5102d1f202c195aa84a99fb434853f3e039bf9610e6cb771e8d52bf8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220427` - linux; 386

```console
$ docker pull ubuntu@sha256:a7ed45c4a95fbe19f9c5fb9d1ca58b2431b2a4984754be2f50ccec99d9428b79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27164138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7676d532710d57b644a18d0c7428c1dd9bff21a26620a9ea60cf4cf1018bc3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:46:47 GMT
ADD file:bcce1e9e400660e474d54b70b67bc484a7976aff4e980b58d10ddcb4daa58a7f in / 
# Fri, 29 Apr 2022 22:46:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:14c49d5e021ef38e29480c34c86df22d89b9b63fe1a57ec4dd970f56497edf9a`  
		Last Modified: Fri, 29 Apr 2022 22:47:32 GMT  
		Size: 27.2 MB (27164138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220427` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:740a942c894a06e2e490f6f17b470409fa62e34eea7ab6c2c0c73be7f242277c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30443183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb6ac865363641875a604c1ac20e4c665b6f62f40d3f9dd5227799da41fb957`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20220427` - linux; s390x

```console
$ docker pull ubuntu@sha256:2e9f488d35790e264437c71bd6774aec0704432d91d8c73bb0c599143729371f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25365828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edafd08d1799b5c8023f02483d4f15f7e2b52dd3e38fa647502d36d37a63899`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:88c79ab062b79c8fe13036065334ecabb3bc2f302f08fcb887a2afc7f80cfa2d
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
$ docker pull ubuntu@sha256:fb5104deb0ffa22606091c5fc569d7c013e826a58cf9c3d0dedcb7e99ac21cd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30420973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f60b19cdd3178764b1a6c6b19220e3396d5671816b51bb894027fde4a7ac8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:23 GMT
ADD file:ebe265aac135a4affe0b35a5e79cd43480dc94796fba7b04095ff6dd92c42359 in / 
# Fri, 29 Apr 2022 23:21:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0ca6c954284ce98aea2c55589ebabd347d2caf3ba94387f53b5339c1f35ab8b7`  
		Last Modified: Fri, 29 Apr 2022 23:23:13 GMT  
		Size: 30.4 MB (30420973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:99139ea3b12bc75ee149bd32c1e4d295bcfd25002d2e0d857696b3df3c252647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a4f900232301f0c95d7d758c05cb05b1d3f1a9b8f8e2ccdad3c23cd88a4653`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:55 GMT
ADD file:063f432f8adfa6ad56a7bb07ff90f71f00c47c30a03bd892e04ddd744042a0d3 in / 
# Fri, 29 Apr 2022 22:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1fc430d8f49d4d10815388bc3cb533e89d8123bcc10ffd2a333c16216f2e4303`  
		Last Modified: Fri, 29 Apr 2022 23:04:36 GMT  
		Size: 27.0 MB (27015929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:27daec02acc728d62b293e954981c142333eb8dfd8ce4bfd75eac008f5528d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c907287071226ba97298d35b0990fa71f8103054147bf36e2946589478c5ce2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:02 GMT
ADD file:1dcfa00d31cec211ba91522ed6fcf6f72e3f1f4ad30c4f7ca398add7eba377c0 in / 
# Fri, 29 Apr 2022 22:50:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:957fa4daed10cc16359daab2a50b5ffbbc1d762035c4eba567b3d4205e7afbde`  
		Last Modified: Fri, 29 Apr 2022 22:52:30 GMT  
		Size: 28.4 MB (28376165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:045009e9203b47686922bea14515bdbcbb168459bdc987b67e2d6713340de4c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5a463bb8a2d14a5b936418198de915b0021f6efea27d2a68b6366091fc9b91`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:22 GMT
ADD file:255691256b47d5fe6ed4871151edc57eb15be171ec05706f4ac6e574bdaff407 in / 
# Fri, 29 Apr 2022 23:23:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:314e7db37887c48e6b822759045272201a6ed3ff0bb4f89f164f9f3ff64cacaa`  
		Last Modified: Fri, 29 Apr 2022 23:26:43 GMT  
		Size: 35.7 MB (35719018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; riscv64

```console
$ docker pull ubuntu@sha256:c18733fbe1d10983c42f8db215657467128ad8f638d3fdd61bdf0f88e04b5220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd76126609e952f9a5820b162ac407928a97012de59f5a1909c2af75963dcd9a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:28 GMT
ADD file:88e52fba8a3ffc283333df24e0d115ab58328ac1d5f6cf585d17422676e146d3 in / 
# Fri, 29 Apr 2022 23:21:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5e53595b65ef34f5f4d764d94e324a0b884612b1b49f768cdd94321c4f22fefd`  
		Last Modified: Fri, 29 Apr 2022 23:44:55 GMT  
		Size: 27.7 MB (27745108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:8ce2906f39c6d06e337ad8b5ed647dd304ed1a1fa7ee54eab38cc1d5707610fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00438fda1e2923dd12f8d9a545ca5cb1e13a0a6ff5e38ee519c634f280f5207e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:44 GMT
ADD file:55affb702d0be7976581cacdb7c77f2c1b0d6921d2cd689a427471c2fd9d4daf in / 
# Fri, 29 Apr 2022 22:50:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c551bbcabccfb0977b8a9e2ba72099b05f9ba8b7c7106d8a29073b45bc73a9a4`  
		Last Modified: Fri, 29 Apr 2022 22:52:38 GMT  
		Size: 28.6 MB (28637139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:47f14534bda344d9fe6ffd6effb95eefe579f4be0d508b7445cf77f61a0e5724
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
$ docker pull ubuntu@sha256:9d42d0e3e57bc067d10a75ee33bdd1a5298e95e5fc3c5d1fce98b455cb879249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28566230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53df61775e8856a464ca52d4cd9eabbf4eb3ceedbde5afecc57e417e7b7155d5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:681dcdedc7ac9708764c1018cb9785907298c490cee08717ce57d401258ac876
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24073650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3dbf2c88b9eed84cee7427e9fc590a188443d72668941196c7395d8af26dc2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:ca83774d06420ceb4682ef73bd9cbbfc38a97a27e061b578547a6761206658b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27169388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1bc6aa58da386bc4ae8c4489e0bda0f6073c49a7b6c2ca24386671b36a1f19`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:55da61c5ad752c43ad671b0bc16a0496371b98d85dcc4cd4dc735c695cced298
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33290661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8c2a68f557812cf6d4826032f0cd968647c228f3ac23b82a5b518165d6b34d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; riscv64

```console
$ docker pull ubuntu@sha256:4df7126c32c74eb9b734113d03545aa1ac4938b91319fbfe8cb693b94adfc6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24228241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1e2591ecd338320e77f4377aae51c48f3de7128de9fb27bdb3a888dd4781d4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:14:50 GMT
ADD file:77e925ea3ddf0d01534094175d808508c4a5d0535f08d304994323efb0173a57 in / 
# Fri, 29 Apr 2022 23:14:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:63ac7876cbf81a317a4c88c281171f026148a0f62b17284f294a5f0eb06bb383`  
		Last Modified: Fri, 29 Apr 2022 23:36:48 GMT  
		Size: 24.2 MB (24228241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:4ca42ab690fab0df13fb1c8f79cdb7d6307442d83abe776d6c9b647b48b09d62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27065417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5571b2169962786dfe503560491daf168d8b9b774d818d4f2ec789f2fa3cc53`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal-20220426`

```console
$ docker pull ubuntu@sha256:47f14534bda344d9fe6ffd6effb95eefe579f4be0d508b7445cf77f61a0e5724
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:focal-20220426` - linux; amd64

```console
$ docker pull ubuntu@sha256:9d42d0e3e57bc067d10a75ee33bdd1a5298e95e5fc3c5d1fce98b455cb879249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28566230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53df61775e8856a464ca52d4cd9eabbf4eb3ceedbde5afecc57e417e7b7155d5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220426` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:681dcdedc7ac9708764c1018cb9785907298c490cee08717ce57d401258ac876
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24073650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3dbf2c88b9eed84cee7427e9fc590a188443d72668941196c7395d8af26dc2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220426` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:ca83774d06420ceb4682ef73bd9cbbfc38a97a27e061b578547a6761206658b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27169388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1bc6aa58da386bc4ae8c4489e0bda0f6073c49a7b6c2ca24386671b36a1f19`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220426` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:55da61c5ad752c43ad671b0bc16a0496371b98d85dcc4cd4dc735c695cced298
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33290661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8c2a68f557812cf6d4826032f0cd968647c228f3ac23b82a5b518165d6b34d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220426` - linux; riscv64

```console
$ docker pull ubuntu@sha256:4df7126c32c74eb9b734113d03545aa1ac4938b91319fbfe8cb693b94adfc6c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.2 MB (24228241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1e2591ecd338320e77f4377aae51c48f3de7128de9fb27bdb3a888dd4781d4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:14:50 GMT
ADD file:77e925ea3ddf0d01534094175d808508c4a5d0535f08d304994323efb0173a57 in / 
# Fri, 29 Apr 2022 23:14:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:63ac7876cbf81a317a4c88c281171f026148a0f62b17284f294a5f0eb06bb383`  
		Last Modified: Fri, 29 Apr 2022 23:36:48 GMT  
		Size: 24.2 MB (24228241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20220426` - linux; s390x

```console
$ docker pull ubuntu@sha256:4ca42ab690fab0df13fb1c8f79cdb7d6307442d83abe776d6c9b647b48b09d62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27065417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5571b2169962786dfe503560491daf168d8b9b774d818d4f2ec789f2fa3cc53`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:impish`

```console
$ docker pull ubuntu@sha256:14d8cab8d7bd72a01e225cd85bf37bbf08bf88115769316fa86c776df4ea5fed
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
$ docker pull ubuntu@sha256:253908b2844746ab3f3a08fc8a44b9b9fc1efc408d5969b093ab9ffa11eb1894
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30383364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:565852265961284e5715ccd6f1a20339c4b0448d7649d76e3abbd4fafab3adc4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:07 GMT
ADD file:e36038a1f6ee02f3f9a7db183e116f58d277e97cb7e71032634097d802654d02 in / 
# Fri, 29 Apr 2022 23:21:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:940122ec7d0c039d048e3bf953a33cd8ef814fd587266a5e732d24d2314af8f1`  
		Last Modified: Fri, 29 Apr 2022 23:22:38 GMT  
		Size: 30.4 MB (30383364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:51927bb029ae20b80e128ab2c5620163a1b89975d4cbed6f56eab57ca591f5f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26920477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a66381c8346b8424a3114f9d6db5e4d331759c66ce3cce459e427d53b1ddf3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:09 GMT
ADD file:98b792cccd674eb149eee0fddc60ebe9484757384fe35630fc361ecfc28f9e42 in / 
# Fri, 29 Apr 2022 22:59:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2a09877f6132d465ce4f615f0c5f4bb1dc0e311ce406712beced416d3257e69c`  
		Last Modified: Fri, 29 Apr 2022 23:03:29 GMT  
		Size: 26.9 MB (26920477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:330330705b92fe325e550f8d35519f2213e1168df212cf8095ea10db63fb6afa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29029534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771a596909ab10d1a46e672acfdae2b4ecae9896feb006e47a62f826f30128dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:43 GMT
ADD file:d800d571fc22b337baaf45095bd1a303ca66065106c8b943a7a869e145896077 in / 
# Fri, 29 Apr 2022 22:49:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:924f038c577f5fb37fec4317d1c44a40bae2f6ee798dc0e31394270b30d69e8d`  
		Last Modified: Fri, 29 Apr 2022 22:51:50 GMT  
		Size: 29.0 MB (29029534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:0d276731b94e2e3853de594483da216a28f7d85d99e54e08cc1d0b7ce88b0678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36172344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6000d2ac9546a6047aae9606bceb162b9217c1174d3a82e78eff866c1f7eb6fd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:47 GMT
ADD file:6fee77e76b27182351bc3f1670478775d45b940b676a9c68b3057638166e1f3e in / 
# Fri, 29 Apr 2022 23:22:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b9131999f6427d8e2f8c2e6af3dc4889e32c5ea861065b2f8c24539e9c7d81a`  
		Last Modified: Fri, 29 Apr 2022 23:25:51 GMT  
		Size: 36.2 MB (36172344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; riscv64

```console
$ docker pull ubuntu@sha256:12121497838f0eeede99311646bc3684fec38672f9bdcb6b4200dd88f85a8271
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18096f6eeb14bbd454bbf5ef5981db09e489f8c622df7e2148260a78d279870c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:16:52 GMT
ADD file:9b1d81091b302d999994d0aff49d52975044c0786e8d7aa0df0ce41ec3c5902b in / 
# Fri, 29 Apr 2022 23:16:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3105f98235ad0afa0e8e8fb758ef0e3a7fa3bc505fc19f49da0968611aa32271`  
		Last Modified: Fri, 29 Apr 2022 23:39:06 GMT  
		Size: 27.2 MB (27210922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish` - linux; s390x

```console
$ docker pull ubuntu@sha256:b8fd502cf99110f83f77a46ce35d1be1cc3a2a22a32207160220ac2b1daaf377
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30502867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a417516b88a5eadd6c55194447e00a7a78c4a559e7d739f16fc763cd6b434982`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:17 GMT
ADD file:1041ef5c07ca82ee2d7f626a60380e731aa09d0d2b9b6877b03abffa280e452b in / 
# Fri, 29 Apr 2022 22:50:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fe0d74cf06c14c44f5210e7c3b5af279f02a1d45707ee11e6afae132344bf765`  
		Last Modified: Fri, 29 Apr 2022 22:52:13 GMT  
		Size: 30.5 MB (30502867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:impish-20220427`

```console
$ docker pull ubuntu@sha256:14d8cab8d7bd72a01e225cd85bf37bbf08bf88115769316fa86c776df4ea5fed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:impish-20220427` - linux; amd64

```console
$ docker pull ubuntu@sha256:253908b2844746ab3f3a08fc8a44b9b9fc1efc408d5969b093ab9ffa11eb1894
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30383364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:565852265961284e5715ccd6f1a20339c4b0448d7649d76e3abbd4fafab3adc4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:07 GMT
ADD file:e36038a1f6ee02f3f9a7db183e116f58d277e97cb7e71032634097d802654d02 in / 
# Fri, 29 Apr 2022 23:21:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:940122ec7d0c039d048e3bf953a33cd8ef814fd587266a5e732d24d2314af8f1`  
		Last Modified: Fri, 29 Apr 2022 23:22:38 GMT  
		Size: 30.4 MB (30383364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20220427` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:51927bb029ae20b80e128ab2c5620163a1b89975d4cbed6f56eab57ca591f5f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26920477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a66381c8346b8424a3114f9d6db5e4d331759c66ce3cce459e427d53b1ddf3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:09 GMT
ADD file:98b792cccd674eb149eee0fddc60ebe9484757384fe35630fc361ecfc28f9e42 in / 
# Fri, 29 Apr 2022 22:59:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:2a09877f6132d465ce4f615f0c5f4bb1dc0e311ce406712beced416d3257e69c`  
		Last Modified: Fri, 29 Apr 2022 23:03:29 GMT  
		Size: 26.9 MB (26920477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20220427` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:330330705b92fe325e550f8d35519f2213e1168df212cf8095ea10db63fb6afa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29029534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771a596909ab10d1a46e672acfdae2b4ecae9896feb006e47a62f826f30128dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:43 GMT
ADD file:d800d571fc22b337baaf45095bd1a303ca66065106c8b943a7a869e145896077 in / 
# Fri, 29 Apr 2022 22:49:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:924f038c577f5fb37fec4317d1c44a40bae2f6ee798dc0e31394270b30d69e8d`  
		Last Modified: Fri, 29 Apr 2022 22:51:50 GMT  
		Size: 29.0 MB (29029534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20220427` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:0d276731b94e2e3853de594483da216a28f7d85d99e54e08cc1d0b7ce88b0678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36172344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6000d2ac9546a6047aae9606bceb162b9217c1174d3a82e78eff866c1f7eb6fd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:47 GMT
ADD file:6fee77e76b27182351bc3f1670478775d45b940b676a9c68b3057638166e1f3e in / 
# Fri, 29 Apr 2022 23:22:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8b9131999f6427d8e2f8c2e6af3dc4889e32c5ea861065b2f8c24539e9c7d81a`  
		Last Modified: Fri, 29 Apr 2022 23:25:51 GMT  
		Size: 36.2 MB (36172344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20220427` - linux; riscv64

```console
$ docker pull ubuntu@sha256:12121497838f0eeede99311646bc3684fec38672f9bdcb6b4200dd88f85a8271
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27210922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18096f6eeb14bbd454bbf5ef5981db09e489f8c622df7e2148260a78d279870c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:16:52 GMT
ADD file:9b1d81091b302d999994d0aff49d52975044c0786e8d7aa0df0ce41ec3c5902b in / 
# Fri, 29 Apr 2022 23:16:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:3105f98235ad0afa0e8e8fb758ef0e3a7fa3bc505fc19f49da0968611aa32271`  
		Last Modified: Fri, 29 Apr 2022 23:39:06 GMT  
		Size: 27.2 MB (27210922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:impish-20220427` - linux; s390x

```console
$ docker pull ubuntu@sha256:b8fd502cf99110f83f77a46ce35d1be1cc3a2a22a32207160220ac2b1daaf377
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30502867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a417516b88a5eadd6c55194447e00a7a78c4a559e7d739f16fc763cd6b434982`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:17 GMT
ADD file:1041ef5c07ca82ee2d7f626a60380e731aa09d0d2b9b6877b03abffa280e452b in / 
# Fri, 29 Apr 2022 22:50:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:fe0d74cf06c14c44f5210e7c3b5af279f02a1d45707ee11e6afae132344bf765`  
		Last Modified: Fri, 29 Apr 2022 22:52:13 GMT  
		Size: 30.5 MB (30502867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:26c68657ccce2cb0a31b330cb0be2b5e108d467f641c62e13ab40cbec258c68d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:jammy` - linux; amd64

```console
$ docker pull ubuntu@sha256:aa6c2c047467afc828e77e306041b7fa4a65734fe3449a54aa9c280822b0d87d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30421006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e4e1f511320dfb2d0baff2468fcf0526998b73fe10c8890b4684bb7ef8290f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:58ddb1588a8c0304cd3dbdb81bdd40bee55ab67dcd4e9938ec167728bde5ae54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4454e2e75bf4628b8547fb60b3753c9ce8cf250f6e86c944155b45873be77504`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e01a1e915645f9240d02ab90cc15da706b4dee508025785dd0538bb3fc7f859
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d495355b4ebc1367b0a666d029e8bd1f8cb3a85d1ecd0bbe5e20138c37e155`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1ed6cb877f3697c3fa7cdd1cf2e6c5c496fc1ab84ac6d020c9533fff23c8f897
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1a9b14de904dc06d5041a4a4ecd65ff2fa3a66c0a088e831db7d83a26ca0b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:05 GMT
ADD file:db27920209849d42ecc46854d40c0f2c71346054166d0a2e37cc3c0361362391 in / 
# Fri, 29 Apr 2022 23:23:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4cf58bb815afda02904690ca8e3231fd4a3c7c0bfc79bd44118ca3720f18a2cd`  
		Last Modified: Fri, 29 Apr 2022 23:26:14 GMT  
		Size: 35.7 MB (35719376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; riscv64

```console
$ docker pull ubuntu@sha256:904dcdf5747aeeb016cfa00ccd4c25f0baedbae5b6bcd834b38bf47ebcce2783
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a98b3afd049e95d4a4cd74ddc36a0bd0292ee3ea7eba7da6f610367fb2b64b9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:18:56 GMT
ADD file:7350517b53b7fc7556b4df07b2d762e16a9797b68f4760d536321210c8acfd34 in / 
# Fri, 29 Apr 2022 23:18:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29912c87e17183ec23ae82771552de74ad581040d14b5d35e5678e1409ca9a66`  
		Last Modified: Fri, 29 Apr 2022 23:41:25 GMT  
		Size: 27.7 MB (27745174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:c18eff699e090d6b0336dda55b9f83cbbdf126100aa06d16de4fc58e2fa740df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277242fcbfea4007bf94af719bb1c8007b5af5f3ce6942bd3ef798dd73422ab9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:jammy-20220428`

```console
$ docker pull ubuntu@sha256:26c68657ccce2cb0a31b330cb0be2b5e108d467f641c62e13ab40cbec258c68d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:jammy-20220428` - linux; amd64

```console
$ docker pull ubuntu@sha256:aa6c2c047467afc828e77e306041b7fa4a65734fe3449a54aa9c280822b0d87d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30421006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e4e1f511320dfb2d0baff2468fcf0526998b73fe10c8890b4684bb7ef8290f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220428` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:58ddb1588a8c0304cd3dbdb81bdd40bee55ab67dcd4e9938ec167728bde5ae54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4454e2e75bf4628b8547fb60b3753c9ce8cf250f6e86c944155b45873be77504`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220428` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e01a1e915645f9240d02ab90cc15da706b4dee508025785dd0538bb3fc7f859
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d495355b4ebc1367b0a666d029e8bd1f8cb3a85d1ecd0bbe5e20138c37e155`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220428` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1ed6cb877f3697c3fa7cdd1cf2e6c5c496fc1ab84ac6d020c9533fff23c8f897
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1a9b14de904dc06d5041a4a4ecd65ff2fa3a66c0a088e831db7d83a26ca0b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:05 GMT
ADD file:db27920209849d42ecc46854d40c0f2c71346054166d0a2e37cc3c0361362391 in / 
# Fri, 29 Apr 2022 23:23:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4cf58bb815afda02904690ca8e3231fd4a3c7c0bfc79bd44118ca3720f18a2cd`  
		Last Modified: Fri, 29 Apr 2022 23:26:14 GMT  
		Size: 35.7 MB (35719376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220428` - linux; riscv64

```console
$ docker pull ubuntu@sha256:904dcdf5747aeeb016cfa00ccd4c25f0baedbae5b6bcd834b38bf47ebcce2783
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a98b3afd049e95d4a4cd74ddc36a0bd0292ee3ea7eba7da6f610367fb2b64b9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:18:56 GMT
ADD file:7350517b53b7fc7556b4df07b2d762e16a9797b68f4760d536321210c8acfd34 in / 
# Fri, 29 Apr 2022 23:18:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29912c87e17183ec23ae82771552de74ad581040d14b5d35e5678e1409ca9a66`  
		Last Modified: Fri, 29 Apr 2022 23:41:25 GMT  
		Size: 27.7 MB (27745174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20220428` - linux; s390x

```console
$ docker pull ubuntu@sha256:c18eff699e090d6b0336dda55b9f83cbbdf126100aa06d16de4fc58e2fa740df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277242fcbfea4007bf94af719bb1c8007b5af5f3ce6942bd3ef798dd73422ab9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:88c79ab062b79c8fe13036065334ecabb3bc2f302f08fcb887a2afc7f80cfa2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:kinetic` - linux; amd64

```console
$ docker pull ubuntu@sha256:fb5104deb0ffa22606091c5fc569d7c013e826a58cf9c3d0dedcb7e99ac21cd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30420973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f60b19cdd3178764b1a6c6b19220e3396d5671816b51bb894027fde4a7ac8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:23 GMT
ADD file:ebe265aac135a4affe0b35a5e79cd43480dc94796fba7b04095ff6dd92c42359 in / 
# Fri, 29 Apr 2022 23:21:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0ca6c954284ce98aea2c55589ebabd347d2caf3ba94387f53b5339c1f35ab8b7`  
		Last Modified: Fri, 29 Apr 2022 23:23:13 GMT  
		Size: 30.4 MB (30420973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:99139ea3b12bc75ee149bd32c1e4d295bcfd25002d2e0d857696b3df3c252647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a4f900232301f0c95d7d758c05cb05b1d3f1a9b8f8e2ccdad3c23cd88a4653`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:55 GMT
ADD file:063f432f8adfa6ad56a7bb07ff90f71f00c47c30a03bd892e04ddd744042a0d3 in / 
# Fri, 29 Apr 2022 22:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1fc430d8f49d4d10815388bc3cb533e89d8123bcc10ffd2a333c16216f2e4303`  
		Last Modified: Fri, 29 Apr 2022 23:04:36 GMT  
		Size: 27.0 MB (27015929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:27daec02acc728d62b293e954981c142333eb8dfd8ce4bfd75eac008f5528d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c907287071226ba97298d35b0990fa71f8103054147bf36e2946589478c5ce2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:02 GMT
ADD file:1dcfa00d31cec211ba91522ed6fcf6f72e3f1f4ad30c4f7ca398add7eba377c0 in / 
# Fri, 29 Apr 2022 22:50:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:957fa4daed10cc16359daab2a50b5ffbbc1d762035c4eba567b3d4205e7afbde`  
		Last Modified: Fri, 29 Apr 2022 22:52:30 GMT  
		Size: 28.4 MB (28376165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:045009e9203b47686922bea14515bdbcbb168459bdc987b67e2d6713340de4c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5a463bb8a2d14a5b936418198de915b0021f6efea27d2a68b6366091fc9b91`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:22 GMT
ADD file:255691256b47d5fe6ed4871151edc57eb15be171ec05706f4ac6e574bdaff407 in / 
# Fri, 29 Apr 2022 23:23:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:314e7db37887c48e6b822759045272201a6ed3ff0bb4f89f164f9f3ff64cacaa`  
		Last Modified: Fri, 29 Apr 2022 23:26:43 GMT  
		Size: 35.7 MB (35719018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; riscv64

```console
$ docker pull ubuntu@sha256:c18733fbe1d10983c42f8db215657467128ad8f638d3fdd61bdf0f88e04b5220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd76126609e952f9a5820b162ac407928a97012de59f5a1909c2af75963dcd9a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:28 GMT
ADD file:88e52fba8a3ffc283333df24e0d115ab58328ac1d5f6cf585d17422676e146d3 in / 
# Fri, 29 Apr 2022 23:21:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5e53595b65ef34f5f4d764d94e324a0b884612b1b49f768cdd94321c4f22fefd`  
		Last Modified: Fri, 29 Apr 2022 23:44:55 GMT  
		Size: 27.7 MB (27745108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; s390x

```console
$ docker pull ubuntu@sha256:8ce2906f39c6d06e337ad8b5ed647dd304ed1a1fa7ee54eab38cc1d5707610fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00438fda1e2923dd12f8d9a545ca5cb1e13a0a6ff5e38ee519c634f280f5207e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:44 GMT
ADD file:55affb702d0be7976581cacdb7c77f2c1b0d6921d2cd689a427471c2fd9d4daf in / 
# Fri, 29 Apr 2022 22:50:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c551bbcabccfb0977b8a9e2ba72099b05f9ba8b7c7106d8a29073b45bc73a9a4`  
		Last Modified: Fri, 29 Apr 2022 22:52:38 GMT  
		Size: 28.6 MB (28637139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:kinetic-20220428`

```console
$ docker pull ubuntu@sha256:88c79ab062b79c8fe13036065334ecabb3bc2f302f08fcb887a2afc7f80cfa2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `ubuntu:kinetic-20220428` - linux; amd64

```console
$ docker pull ubuntu@sha256:fb5104deb0ffa22606091c5fc569d7c013e826a58cf9c3d0dedcb7e99ac21cd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30420973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f60b19cdd3178764b1a6c6b19220e3396d5671816b51bb894027fde4a7ac8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:23 GMT
ADD file:ebe265aac135a4affe0b35a5e79cd43480dc94796fba7b04095ff6dd92c42359 in / 
# Fri, 29 Apr 2022 23:21:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0ca6c954284ce98aea2c55589ebabd347d2caf3ba94387f53b5339c1f35ab8b7`  
		Last Modified: Fri, 29 Apr 2022 23:23:13 GMT  
		Size: 30.4 MB (30420973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220428` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:99139ea3b12bc75ee149bd32c1e4d295bcfd25002d2e0d857696b3df3c252647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a4f900232301f0c95d7d758c05cb05b1d3f1a9b8f8e2ccdad3c23cd88a4653`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:55 GMT
ADD file:063f432f8adfa6ad56a7bb07ff90f71f00c47c30a03bd892e04ddd744042a0d3 in / 
# Fri, 29 Apr 2022 22:59:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1fc430d8f49d4d10815388bc3cb533e89d8123bcc10ffd2a333c16216f2e4303`  
		Last Modified: Fri, 29 Apr 2022 23:04:36 GMT  
		Size: 27.0 MB (27015929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220428` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:27daec02acc728d62b293e954981c142333eb8dfd8ce4bfd75eac008f5528d95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c907287071226ba97298d35b0990fa71f8103054147bf36e2946589478c5ce2`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:02 GMT
ADD file:1dcfa00d31cec211ba91522ed6fcf6f72e3f1f4ad30c4f7ca398add7eba377c0 in / 
# Fri, 29 Apr 2022 22:50:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:957fa4daed10cc16359daab2a50b5ffbbc1d762035c4eba567b3d4205e7afbde`  
		Last Modified: Fri, 29 Apr 2022 22:52:30 GMT  
		Size: 28.4 MB (28376165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220428` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:045009e9203b47686922bea14515bdbcbb168459bdc987b67e2d6713340de4c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5a463bb8a2d14a5b936418198de915b0021f6efea27d2a68b6366091fc9b91`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:22 GMT
ADD file:255691256b47d5fe6ed4871151edc57eb15be171ec05706f4ac6e574bdaff407 in / 
# Fri, 29 Apr 2022 23:23:26 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:314e7db37887c48e6b822759045272201a6ed3ff0bb4f89f164f9f3ff64cacaa`  
		Last Modified: Fri, 29 Apr 2022 23:26:43 GMT  
		Size: 35.7 MB (35719018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220428` - linux; riscv64

```console
$ docker pull ubuntu@sha256:c18733fbe1d10983c42f8db215657467128ad8f638d3fdd61bdf0f88e04b5220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd76126609e952f9a5820b162ac407928a97012de59f5a1909c2af75963dcd9a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:28 GMT
ADD file:88e52fba8a3ffc283333df24e0d115ab58328ac1d5f6cf585d17422676e146d3 in / 
# Fri, 29 Apr 2022 23:21:30 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5e53595b65ef34f5f4d764d94e324a0b884612b1b49f768cdd94321c4f22fefd`  
		Last Modified: Fri, 29 Apr 2022 23:44:55 GMT  
		Size: 27.7 MB (27745108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20220428` - linux; s390x

```console
$ docker pull ubuntu@sha256:8ce2906f39c6d06e337ad8b5ed647dd304ed1a1fa7ee54eab38cc1d5707610fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00438fda1e2923dd12f8d9a545ca5cb1e13a0a6ff5e38ee519c634f280f5207e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:44 GMT
ADD file:55affb702d0be7976581cacdb7c77f2c1b0d6921d2cd689a427471c2fd9d4daf in / 
# Fri, 29 Apr 2022 22:50:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c551bbcabccfb0977b8a9e2ba72099b05f9ba8b7c7106d8a29073b45bc73a9a4`  
		Last Modified: Fri, 29 Apr 2022 22:52:38 GMT  
		Size: 28.6 MB (28637139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:26c68657ccce2cb0a31b330cb0be2b5e108d467f641c62e13ab40cbec258c68d
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
$ docker pull ubuntu@sha256:aa6c2c047467afc828e77e306041b7fa4a65734fe3449a54aa9c280822b0d87d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30421006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e4e1f511320dfb2d0baff2468fcf0526998b73fe10c8890b4684bb7ef8290f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:58ddb1588a8c0304cd3dbdb81bdd40bee55ab67dcd4e9938ec167728bde5ae54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4454e2e75bf4628b8547fb60b3753c9ce8cf250f6e86c944155b45873be77504`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e01a1e915645f9240d02ab90cc15da706b4dee508025785dd0538bb3fc7f859
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d495355b4ebc1367b0a666d029e8bd1f8cb3a85d1ecd0bbe5e20138c37e155`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1ed6cb877f3697c3fa7cdd1cf2e6c5c496fc1ab84ac6d020c9533fff23c8f897
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1a9b14de904dc06d5041a4a4ecd65ff2fa3a66c0a088e831db7d83a26ca0b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:05 GMT
ADD file:db27920209849d42ecc46854d40c0f2c71346054166d0a2e37cc3c0361362391 in / 
# Fri, 29 Apr 2022 23:23:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4cf58bb815afda02904690ca8e3231fd4a3c7c0bfc79bd44118ca3720f18a2cd`  
		Last Modified: Fri, 29 Apr 2022 23:26:14 GMT  
		Size: 35.7 MB (35719376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; riscv64

```console
$ docker pull ubuntu@sha256:904dcdf5747aeeb016cfa00ccd4c25f0baedbae5b6bcd834b38bf47ebcce2783
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a98b3afd049e95d4a4cd74ddc36a0bd0292ee3ea7eba7da6f610367fb2b64b9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:18:56 GMT
ADD file:7350517b53b7fc7556b4df07b2d762e16a9797b68f4760d536321210c8acfd34 in / 
# Fri, 29 Apr 2022 23:18:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29912c87e17183ec23ae82771552de74ad581040d14b5d35e5678e1409ca9a66`  
		Last Modified: Fri, 29 Apr 2022 23:41:25 GMT  
		Size: 27.7 MB (27745174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:c18eff699e090d6b0336dda55b9f83cbbdf126100aa06d16de4fc58e2fa740df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277242fcbfea4007bf94af719bb1c8007b5af5f3ce6942bd3ef798dd73422ab9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:26c68657ccce2cb0a31b330cb0be2b5e108d467f641c62e13ab40cbec258c68d
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
$ docker pull ubuntu@sha256:aa6c2c047467afc828e77e306041b7fa4a65734fe3449a54aa9c280822b0d87d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30421006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e4e1f511320dfb2d0baff2468fcf0526998b73fe10c8890b4684bb7ef8290f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:15 GMT
ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / 
# Fri, 29 Apr 2022 23:21:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:125a6e411906fe6b0aaa50fc9d600bf6ff9bb11a8651727ce1ed482dc271c24c`  
		Last Modified: Fri, 29 Apr 2022 03:03:30 GMT  
		Size: 30.4 MB (30421006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:58ddb1588a8c0304cd3dbdb81bdd40bee55ab67dcd4e9938ec167728bde5ae54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27015834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4454e2e75bf4628b8547fb60b3753c9ce8cf250f6e86c944155b45873be77504`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8e01a1e915645f9240d02ab90cc15da706b4dee508025785dd0538bb3fc7f859
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28376457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d495355b4ebc1367b0a666d029e8bd1f8cb3a85d1ecd0bbe5e20138c37e155`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1ed6cb877f3697c3fa7cdd1cf2e6c5c496fc1ab84ac6d020c9533fff23c8f897
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35719376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1a9b14de904dc06d5041a4a4ecd65ff2fa3a66c0a088e831db7d83a26ca0b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:23:05 GMT
ADD file:db27920209849d42ecc46854d40c0f2c71346054166d0a2e37cc3c0361362391 in / 
# Fri, 29 Apr 2022 23:23:08 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:4cf58bb815afda02904690ca8e3231fd4a3c7c0bfc79bd44118ca3720f18a2cd`  
		Last Modified: Fri, 29 Apr 2022 23:26:14 GMT  
		Size: 35.7 MB (35719376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; riscv64

```console
$ docker pull ubuntu@sha256:904dcdf5747aeeb016cfa00ccd4c25f0baedbae5b6bcd834b38bf47ebcce2783
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27745174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a98b3afd049e95d4a4cd74ddc36a0bd0292ee3ea7eba7da6f610367fb2b64b9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:18:56 GMT
ADD file:7350517b53b7fc7556b4df07b2d762e16a9797b68f4760d536321210c8acfd34 in / 
# Fri, 29 Apr 2022 23:18:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:29912c87e17183ec23ae82771552de74ad581040d14b5d35e5678e1409ca9a66`  
		Last Modified: Fri, 29 Apr 2022 23:41:25 GMT  
		Size: 27.7 MB (27745174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:c18eff699e090d6b0336dda55b9f83cbbdf126100aa06d16de4fc58e2fa740df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28637232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277242fcbfea4007bf94af719bb1c8007b5af5f3ce6942bd3ef798dd73422ab9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty`

```console
$ docker pull ubuntu@sha256:96a36dd3bcd8f149fa9874c4e28c35c01f715b3e5f8f1a8e06b45887619bf43b
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
$ docker pull ubuntu@sha256:5dc82d0f897a1bfd6a68db5b2c3692d81e5ea04e31a09664edc420689f8b450c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7304c635fe5273ccdfbc8a38e839c9089350fc8e80daf57394d1f7a9c5a70c86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:09 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Sat, 16 Oct 2021 01:48:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 16 Oct 2021 01:48:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fc464c2dc9f9ce8d7fe9ccd36f4e746ce32b39f19590f519a8cd3dd76827f8`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 59.1 KB (59100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561f253b7549524704fe8cc1da5ebd27d77bc1a1424b0632b683d90eb58e73d3`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; 386

```console
$ docker pull ubuntu@sha256:c97d63976268e6c2f3764be91e59f82009b2883d22c3dc6ff1f63e3ad6abdb05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a7710ba73fd21ad01442fe2b079693c60a5b77b18403d56e5da5448e325d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:14 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Tue, 05 Apr 2022 22:39:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 05 Apr 2022 22:39:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03124bfb4886d9ba012a00a087fb41b4cc7e99517b3e2a2e6fd1e2ad327af191`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b953ad705784700c1611b7258f6c783a34b06bf27ed3efbd9acc7be80ba991`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 162.0 B  
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
$ docker pull ubuntu@sha256:96a36dd3bcd8f149fa9874c4e28c35c01f715b3e5f8f1a8e06b45887619bf43b
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
$ docker pull ubuntu@sha256:5dc82d0f897a1bfd6a68db5b2c3692d81e5ea04e31a09664edc420689f8b450c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7304c635fe5273ccdfbc8a38e839c9089350fc8e80daf57394d1f7a9c5a70c86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:09 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Sat, 16 Oct 2021 01:48:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 16 Oct 2021 01:48:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fc464c2dc9f9ce8d7fe9ccd36f4e746ce32b39f19590f519a8cd3dd76827f8`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 59.1 KB (59100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561f253b7549524704fe8cc1da5ebd27d77bc1a1424b0632b683d90eb58e73d3`  
		Last Modified: Sat, 16 Oct 2021 01:50:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; 386

```console
$ docker pull ubuntu@sha256:c97d63976268e6c2f3764be91e59f82009b2883d22c3dc6ff1f63e3ad6abdb05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a7710ba73fd21ad01442fe2b079693c60a5b77b18403d56e5da5448e325d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:14 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Tue, 05 Apr 2022 22:39:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Tue, 05 Apr 2022 22:39:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03124bfb4886d9ba012a00a087fb41b4cc7e99517b3e2a2e6fd1e2ad327af191`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 64.9 KB (64870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b953ad705784700c1611b7258f6c783a34b06bf27ed3efbd9acc7be80ba991`  
		Last Modified: Tue, 05 Apr 2022 22:40:17 GMT  
		Size: 162.0 B  
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
$ docker pull ubuntu@sha256:20858ebbc96215d6c3c574f781133ebffdc7c18d98af4f294cc4c04871a6fe61
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
$ docker pull ubuntu@sha256:70fa660340a344b46cc56b3606dc8abd3bf48b5cbce13d01c720e9793a6bc3c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b34cb9255c8dd390f85c8fe37e6fbe6ac555f86c7e8944cd68da2de2f7633`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; 386

```console
$ docker pull ubuntu@sha256:bcb8397f1390f4f0757ca06ce184f05c8ce0c7a4b5ff93f9ab029a581192917b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276b5b6b7721e99481801a9aaf21a4d2bf6ba6f6676f720f6f4e0da40a71fb19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
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
$ docker pull ubuntu@sha256:20858ebbc96215d6c3c574f781133ebffdc7c18d98af4f294cc4c04871a6fe61
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
$ docker pull ubuntu@sha256:70fa660340a344b46cc56b3606dc8abd3bf48b5cbce13d01c720e9793a6bc3c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41240746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b34cb9255c8dd390f85c8fe37e6fbe6ac555f86c7e8944cd68da2de2f7633`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 16 Oct 2021 01:48:22 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Sat, 16 Oct 2021 01:48:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 16 Oct 2021 01:48:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:48:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 16 Oct 2021 01:48:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238e9b8fdf46981043813ae269c4420735959dd01d4d15c420b66448523e9adc`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5b1b49195905e9415adfe3583301316ef591d794fcfd12b5cd29103fa7ee6b`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a6c6175ba12a0fd708883c2625167711f111f24ce2bb79221fda132487e57`  
		Last Modified: Sat, 16 Oct 2021 01:50:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial-20210804` - linux; 386

```console
$ docker pull ubuntu@sha256:bcb8397f1390f4f0757ca06ce184f05c8ce0c7a4b5ff93f9ab029a581192917b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45817719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276b5b6b7721e99481801a9aaf21a4d2bf6ba6f6676f720f6f4e0da40a71fb19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:39:28 GMT
ADD file:a4ae521feddf8357667e9361bdd972a69ed945f3857cc8c534652592e432575d in / 
# Tue, 05 Apr 2022 22:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Apr 2022 22:39:30 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:39:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Apr 2022 22:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1335d7ebdbbb7325d434cf945bcb54cb20f7288e1ca2a1cf140ae02b324646e6`  
		Last Modified: Sun, 08 Aug 2021 01:00:22 GMT  
		Size: 45.8 MB (45816182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6a227af79fa98ebbd1d2da516e2b7ce1cea5519a760cd0f6688738fbdb951`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3928723c2c34ecd7264ce4e195ddda11403213b1c93d02e8efcd11de4b07a1`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468001dd2f338d54f47d062d65db61c754f09897744d97084afa15cee021200`  
		Last Modified: Tue, 05 Apr 2022 22:40:40 GMT  
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
