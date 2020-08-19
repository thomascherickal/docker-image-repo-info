<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:14.04`](#ubuntu1404)
-	[`ubuntu:16.04`](#ubuntu1604)
-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:20.10`](#ubuntu2010)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20200807`](#ubuntubionic-20200807)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20200729`](#ubuntufocal-20200729)
-	[`ubuntu:groovy`](#ubuntugroovy)
-	[`ubuntu:groovy-20200812`](#ubuntugroovy-20200812)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:rolling`](#ubunturolling)
-	[`ubuntu:trusty`](#ubuntutrusty)
-	[`ubuntu:trusty-20191217`](#ubuntutrusty-20191217)
-	[`ubuntu:xenial`](#ubuntuxenial)
-	[`ubuntu:xenial-20200807`](#ubuntuxenial-20200807)

## `ubuntu:14.04`

```console
$ docker pull ubuntu@sha256:ffc76f71dd8be8c9e222d420dc96901a07b61616689a44c7b3ef6a10b7213de4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:14.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:bd0223687054d0f8884fc9e872392c6385a3195d612400495962e270b572ed06
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4f1fe62ff14a4c8119781d47a3739fa97c190e1df38e868794ad7a7cf50a48`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:23:42 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 19 Dec 2019 04:23:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:23:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:23:45 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:23:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bb187ac3fc6c428f38d46409e7765a18dc6b59bc99914f0ba6936463307ec8`  
		Last Modified: Thu, 19 Dec 2019 04:25:41 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a5bcc4a58aeed61f7dbe0a859aa4d37db24efd0c3ca58fb83605b5ad9044b5`  
		Last Modified: Thu, 19 Dec 2019 04:25:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3fc5c28a28125d304462d5b9292d64a61041350304ac5deab416271b25d2e219
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67449d6018f689b7a2a501426015e0b13ada33b377c4c935c68453ce13706712`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:12:57 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Thu, 19 Dec 2019 06:13:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 06:13:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 06:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 06:13:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08b117a826b8d1ae5a5995f7eab5a89f5d582f24fa0016182b6502e42322179`  
		Last Modified: Thu, 19 Dec 2019 06:15:41 GMT  
		Size: 76.8 KB (76765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d5442ddd2dd606cb4dbd9c7243b10f6848c3ee77c176d1b0c667a2232b900c`  
		Last Modified: Thu, 19 Dec 2019 06:15:42 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:79b0f81ad6fc8f0bced3919beee0a79d60d1c8358911188d0787b1f155656d84
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104c127e75190df2e80d312958f30c9b7d2da0b5356f6c1e81e92dc85d3f9740`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:04 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Thu, 19 Dec 2019 03:54:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:54:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:54:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9592077f8570e1222c5a6930a2fdc85b6b607b6c91230a5762c7bd6d84749e25`  
		Last Modified: Thu, 19 Dec 2019 03:56:48 GMT  
		Size: 59.1 KB (59094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b48639f381d2e2566e4c5bdb9792e8666ac2d2cc22918fda5751b8784ee5a5`  
		Last Modified: Thu, 19 Dec 2019 03:56:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; 386

```console
$ docker pull ubuntu@sha256:c8c1d2e6d53d94ef32e73354d146dc6e39c19ce8db2692356b3a6eef5a8ab956
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b01d68827fff530f34f6ff966823624238b7b90aec1bc82b2a9468da476d20e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:42:13 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 19 Dec 2019 04:42:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:42:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:42:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:42:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df46dbd3c04fd4a00981fd885f4d30a154ffa34bc8329bd448e9ca469df32e1`  
		Last Modified: Thu, 19 Dec 2019 04:43:42 GMT  
		Size: 64.9 KB (64855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4ca1e6e5f77f07de7e2107adcb062e1e72e84ce6ff83d5beeb5f84dfcc8418`  
		Last Modified: Thu, 19 Dec 2019 04:43:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:14.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d00cd5726fb0c0523960683e45fe4bbb3807e68ef3edff693d44454aad69b85b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce257c90d69b5ed2a0955447f934ed3a9bc17c4f723fd6f61c0f55218e507b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:20:59 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Thu, 19 Dec 2019 04:21:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d17944a6ab7c0a73210db128de5b677c26f0d4c4c59f3bf6c76b7d1e847098`  
		Last Modified: Thu, 19 Dec 2019 04:26:36 GMT  
		Size: 63.4 KB (63423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d84211dbdd608b55c60bac1fab57fed3dd6de92653162fe123fd0154bcb03e`  
		Last Modified: Thu, 19 Dec 2019 04:26:35 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:16.04`

```console
$ docker pull ubuntu@sha256:0eb024b1147ab61246cfdbdf05c128550ede262790b25a8a6fd93dd3385ab1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:16.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:cc4755a9f2f76ca73055da11f1bdc01d65ce79202a68b041c67c32770c71954b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44402566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab5e942c505d079974d0bb27608d178568973389fd6aadc72c383dee53148a1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d636745b3c2a4b672644c9d1ef071bf62022a15ac0504362bf27846831a5825b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39024526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76cfa4cd6fd320d3537be33628d202f5bb55c3d2050c808751480aa7152af128`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:09:57 GMT
ADD file:c7836321aa9dc9832d8e14c042281f4a3525083619649e000d08159b6da79460 in / 
# Fri, 24 Jul 2020 16:10:21 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:11:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:11:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:11:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:111f37a6818f459bbc8076c0f741a76111210d34c5738743f43dc1488cf91458`  
		Last Modified: Mon, 13 Jul 2020 15:55:00 GMT  
		Size: 39.0 MB (39022996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa2e8f0d9a725920aa624702144baeaae474875e43f4515d9e69c2bddec4bf`  
		Last Modified: Fri, 24 Jul 2020 16:20:13 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c110f6a5721b4e19fdabed9edeb5446f52132952947cd7b409ac4d4e50b7dc02`  
		Last Modified: Fri, 24 Jul 2020 16:20:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07bd4b31471725e34aa841d95fec2e7425ac418ee0a0f69b6d5ca73c6a17c9e`  
		Last Modified: Fri, 24 Jul 2020 16:20:13 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:efe1dd034811acce9285ab90d22163797ad89997ea736a82da39b449d7981817
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40052287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e092214ffcd69f275e4f62a9012475d13aaeddbf3fe2955c5d9d025aa2997d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:25:59 GMT
ADD file:d816988decfebf469e2b28b4858ce7d4a991a101957a43051324255fbe64c86e in / 
# Fri, 24 Jul 2020 16:26:14 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:26:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:26:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f783735449ae0b09fb9e5ee128904f2f3131f6ba46fcf1350fb6a10f872866be`  
		Last Modified: Tue, 07 Jul 2020 00:25:09 GMT  
		Size: 40.1 MB (40050796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35a03aa6fbe0d9147b23501e6fa41d33cd4489470455008ddcbe201063d7b98`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55e221892467d43fdd76b2b592c2fe46e1c69b08e0e9b94f2b383f38e681f65`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a9069021914a77a3d51ffbff02ea5b8a200180601b2be52e9f98d31b6f1389`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; 386

```console
$ docker pull ubuntu@sha256:ea9f9fde6a023145c143db5546e03439aef953cdb120154a44fb6d6c2b6a354e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44309561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032561d1b1b13cfc7d45b69eb922b7d469020682f7602a0299b511840af082cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:38 GMT
ADD file:0281a09e4b674b2f3a51152f0248e69f839a107f4f471cb0f27eff2b47ab726f in / 
# Fri, 24 Jul 2020 14:40:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:40:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c0e0b433333915e5da26fd00978221162b377102e5592ae0404898aee9034774`  
		Last Modified: Mon, 13 Jul 2020 15:54:54 GMT  
		Size: 44.3 MB (44308027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe61969407896fc6a99d8afd1014a71214e79872ad515cb536fb625f179bbef`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058d18b29821b7997f08813144585afd758722b51207239ee260207de7afbc9c`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c34ee61901e83a038c1c1b44b6fa3e2636045fa919ae5ea8b7b37020e71ae`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:e5ec578bd8c334d7c9849fd9bbaa78ec25f2b51b0bf7c9e18b1e9b7ca32d6681
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46213021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8ff96d89d56684a658e9b6a3c3891de598dea918df7286e1440bd359ab1f71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:02 GMT
ADD file:dcd2851859d61fd28750e405e189b57c4be98decb40630483b321127e70c7e09 in / 
# Fri, 24 Jul 2020 14:39:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b63cedd79494e27389a6587d305305c6405fd695b4ec7afb75d1f68bf207ef26`  
		Last Modified: Mon, 13 Jul 2020 15:56:00 GMT  
		Size: 46.2 MB (46211522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78d9771dc7acf0b6f60d469c9b7a9e77989fd64a0b0efb42e1f33bafd86065`  
		Last Modified: Fri, 24 Jul 2020 14:43:33 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed6828e9eba3a3a47f543b8e5cd196fc712376d35e3b4eb322896a90501447f`  
		Last Modified: Fri, 24 Jul 2020 14:43:34 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5111fc2327dba7ff082661e123c7a3589ad2d5cd4dcc2588f1eefc61c8162f4`  
		Last Modified: Fri, 24 Jul 2020 14:43:34 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:16.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:91c8408fcd69b67621810e2787ab8f661a7449ee2f7a0133f0b0771dcb0b1091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42931004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9fe172094fed28581ee6cb7a799cfabb4076d2445205b27336147f780e7a9ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:45:03 GMT
ADD file:bf2a54d719510136249335d267c595d8495031cf3ed3d69c9975f05444bb5129 in / 
# Fri, 24 Jul 2020 14:45:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:45:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:45:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:45:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dbf86c3f4bdb4fdbb59faf631c0d05be1eb33fe938b6332ee07ab035db0a4f8e`  
		Last Modified: Mon, 13 Jul 2020 15:56:10 GMT  
		Size: 42.9 MB (42929517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ce80f41f1cfc5a98c8078530c4618f86fa77832bdf0b0bb484211359473956`  
		Last Modified: Fri, 24 Jul 2020 14:46:17 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdadef093efdb822d71f1ac71a76f40485cac65269a99e6cb366a8fd5548f7d`  
		Last Modified: Fri, 24 Jul 2020 14:46:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f849fe87969087a98487dbc416d25c3dda1b7f7aae893a93963b8615ca8b7903`  
		Last Modified: Fri, 24 Jul 2020 14:46:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:a61728f6128fb4a7a20efaa7597607ed6e69973ee9b9123e3b4fd28b7bba100b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:18.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:767eea1efb29ab7e215e1d97c8d758df5d587ca86e769a2dfb254c6b022895c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26733500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb2d388e1a255c98029f40d6d7f8029fb13f1030abc8f11ccacbca686a8dc12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:8d8280314eac99b6ce1e5307d0093411150a8c09b59f390658952d50139c4722
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22314138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d364ec676a9895226aa2dad9f3bd193151e824600c1f2d343d4986bc9892b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:04:27 GMT
ADD file:934b4bc073556bbba45a5017b40df7ac076a57b031b6b7225919b1ea3c1d89ff in / 
# Fri, 24 Jul 2020 16:04:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:05:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:05:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:05:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de691405df56c17462a8052d9b88a283d955c448deda7a610d70096a5454ff13`  
		Last Modified: Mon, 13 Jul 2020 15:47:13 GMT  
		Size: 22.3 MB (22277635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a766b93ee2f7ed0525d6d90b71c5e860e5e54d4b5259de86c81e5c49ff120c`  
		Last Modified: Fri, 24 Jul 2020 16:13:28 GMT  
		Size: 35.5 KB (35459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c97e104d7363348d21ddc11159cfa859c18d58712fcafc215fefb535baccbae`  
		Last Modified: Fri, 24 Jul 2020 16:13:28 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a97b3bf2bf845ce898abe48aed267cb2a554e220ee512500495c2791ea6ea8`  
		Last Modified: Fri, 24 Jul 2020 16:13:28 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:c83c9f63974b7a72b38f21fadcaa51ab46a75622c114e41fd7c54c9e7bd1371b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23757364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc42dcf4e4b0b31d8937a7f4521cd709ada553cd1dfd9cfee760daae9a4040f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:515e7c555486235ae2ad9c3820c0edf636aacbf25c8402ae70e1a2c3cd6b28f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27159246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1edaca493ec36631fa0d6bd1101e63b106e4ea23a79278b4bfacd9f4f3f7590f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:18 GMT
ADD file:1041a59a13c0d49b1cb87f211694f68be4c9b76f2deb36e2d8955b77c4d2836f in / 
# Fri, 24 Jul 2020 14:40:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:40:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89823af3b784a3ef6d57a90159cbd5f28c863927aa03d4c43b44b6c37479fa1c`  
		Last Modified: Mon, 13 Jul 2020 15:46:56 GMT  
		Size: 27.1 MB (27123624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28677484c2569b014ecb876df3111b11e825c82629306b3af99a1c12f3b234e2`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 34.6 KB (34611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c914b15d9c03339769ddd662b893654bbc371dbed4f8cdfa29ca1c57c0bb98e`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc7dbf6d65bca5959e6f7c892f468288c27e6a0ef07eec142d4497ee07e6cd`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:654769f02fc482e110ca0aa956d81339397e1aa055cdc4749dc03cd621982598
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30441191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fb84f9af6f908e395aed2ee0dee54acd0c53e2c99920595d81d8f15afe022d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:7172b354da3696f8faf5edc61bfe7af3e5851a3f872cea86d8696deef1e646df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25406733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d408badaac51c3893ac324d04eb5206662c4fc0adcd48d62121089f72bfdfa8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:5d1d5407f353843ecf8b16524bc5565aa332e9e6a1297c73a92d3e754b8a636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:20.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:60f560e52264ed1cb7829a0d59b1ee7740d7580e0eb293aca2d722136edb1e24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28590639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4467b07108685c38297025797890f0492c4ec509212e2e4b4822d367fe6bc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6701deddfa3bdabb3a50eb0a24175367b9c7b145e8b2f889ee3b2c52a295ec0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014028cfedab937e84159afcad15a9f4fd8ab921268f6f1ca83b49308587a074`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:06:12 GMT
ADD file:bcba01fb27d025c2931e46af0b091f98e743ab46eaa1d2d2dd38e6aeb9706267 in / 
# Fri, 24 Jul 2020 16:06:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:06:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:06:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:06:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86924fd76ad7a77a1ec54ad07fdb4d2d51c12b6070f2dfe92dbf92e3f99702d7`  
		Last Modified: Mon, 20 Jul 2020 15:50:15 GMT  
		Size: 24.0 MB (24034159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e967235e6adc918de90ffb2d143fb1ad2659c63f6c0c8a9c70c8e08bff13917`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 32.3 KB (32349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabf100c8ea14f6342f16b9b10cb81a1355aa9a9d6b8f607c04119c9790f1a51`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344cec738d225bc4e9abb563b22a040685352088e9d588d910c09039fa47ac35`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8351cb483b295a97ee3cc15150285a58ccf0669e422d4730a9a608988bd5e902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27192812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acd9dae93deacc082f1d3643437b1a1ad4df9e53eb561a5e508531a692d7ea80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:24:06 GMT
ADD file:26bd57f1dbcfd1a91715cc84cf0f221783655f16bbb7a912aaf20507cc252535 in / 
# Fri, 24 Jul 2020 16:24:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:24:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:24:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:24:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3583fd5e2faf2976fb6333a3a15414f2708dc284c018a672e37112326bc7b7a1`  
		Last Modified: Mon, 20 Jul 2020 15:50:10 GMT  
		Size: 27.2 MB (27159444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d9e0aed378588f59f8f4276e70ea379b773d7d6507046cd7a044601499785`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 32.3 KB (32333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a6dca9e536449681a937b8f49022cb56b230e352da8aed9b616fadb14dc30`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d9e98650a6106452fc9e640abe8929399fa4f7a0d3ef58a593e8d68cdf3a6`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d5b40885539615b9aeb7119516427959a158386af13e00d79a7da43ad1b3fb87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33312390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8760d637d5ffca565be33295b10ecf04e581ebd433a48dfd5af138a9c801529a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:35:30 GMT
ADD file:fec1d8aac4ab3a3c2326e15808c04b0df4c06c2c4e66d3f34e3e31d3408fd793 in / 
# Fri, 24 Jul 2020 14:35:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:36:13 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:36:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:36:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4739cd2f4f486596c583c79f6033f1a9dee019389d512603609494678c8ccd53`  
		Last Modified: Mon, 20 Jul 2020 15:51:10 GMT  
		Size: 33.3 MB (33279182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f57f5c67707a22a55ae858c6c54f236321b919889f34c321e1a3cc35b9a7988`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 32.2 KB (32166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b0395dde9514c1a521632a61afda1494fe836f816badcab196bd067b4891c`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b459fe5e4dff59e4cc2b4b5207df42a369d6f0ac774f26c55184b3ccd491996`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:5679518149183fed9dcba60e60f35b0a5ceb59e1ad7b7f9143dc227eda68b202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27302775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a934bfaaf1240f4126c0bdb3327ff5a2d58efa5737524e8205376845b6db8b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:16 GMT
ADD file:6c803b66511ab9cbe066bf89c4d7eb4d7ee4e5a277c36a87dcf63834e18fcfb6 in / 
# Fri, 24 Jul 2020 14:44:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72b8403ae854f945520d1213c568e1b3edf3c0c608fa66780ac822be2ce76657`  
		Last Modified: Mon, 20 Jul 2020 15:56:17 GMT  
		Size: 27.3 MB (27268775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824bb95b6ed456a4fb312de39690e22ca2dac1131067ef2e32679e61e1bf4e76`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 33.0 KB (32965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daf151e726997888df7ebd2403777ed7675e924280e5e5a4180528029a48c0c`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72590bfaf79d6d4e391712b6a34001678f6d42795816fc127ce10762be56d826`  
		Last Modified: Fri, 24 Jul 2020 14:45:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.10`

```console
$ docker pull ubuntu@sha256:162ef5d7086f12982b4bd0fb94e9184fa456f6f1b8d345b52379a5b9f838e675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:20.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:2fb1f8af49f296081dd4fbf33f3f0c5da3be8dc4c413bb6545628f086c0f6408
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28390799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:188e030eedba1500bd3082eece304c1ee29ac38affada33744f4208cb4248596`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:45 GMT
ADD file:8cda7bfcf6c3010f9498acf5db465d8affd86bacb786338974486e23ea62b05d in / 
# Fri, 24 Jul 2020 14:38:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5f55bfaf77a136f7c6b5063e591480c2e7690ed1c29b0ee354caf8f6c62741e0`  
		Last Modified: Fri, 24 Jul 2020 14:39:44 GMT  
		Size: 28.4 MB (28357957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef373180da2631c7a56d9629e37de8010fe57414453617dde3a2c1e9861f1eb`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 31.8 KB (31838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d10b513df5337d26a6e2ccaf4875267999084d7f0d2f3102c54d7430cfa35`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552f92805e8c6585c466083ac60f40092ae127e794d498c599a31bd67df21c09`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:121bd40b7e5df56bcbfe7650e25f69950a71b1e28a184ec0ec1d0d3052bdd1df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23880255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe68c7eedf153aaa9383c727fe9eabb23558d140653fe488c13d8f67b7e25b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:07:21 GMT
ADD file:52d86d22ed47d0da1087414482ade7e5bded2a6a8d539e7214a7f6433820de24 in / 
# Fri, 24 Jul 2020 16:07:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:08:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:08:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:08:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:abee97477daae5ba1c098c334fa7126af27e46cb55f92383c47ee4752cca6b34`  
		Last Modified: Fri, 24 Jul 2020 16:17:36 GMT  
		Size: 23.8 MB (23847354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6932344878e72d9fc106f6b10714cc0590c46ab1bed3d33b7f005de5e8f44dad`  
		Last Modified: Fri, 24 Jul 2020 16:17:30 GMT  
		Size: 31.9 KB (31864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73c3d9eb80a07ca3c2917ec92d98f1dc20cce68119a1400b6dd5598ed03e90e`  
		Last Modified: Fri, 24 Jul 2020 16:17:29 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642ef31c2598b6d4f19ef5a77988b491517e1fd8fe77d266651b8bf97f76fa25`  
		Last Modified: Fri, 24 Jul 2020 16:17:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f388e7c61860c95e835f7f0257d912dc8677c5fa5d2c3377b7f0fcca5c79ff5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26990712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5131fad3254b5b1bd9a41355df1315aee4a69c76083c63cf79380a5dd888bbdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:25:04 GMT
ADD file:d70c9745470cda91695a18f189dd80bae5a680e704e1763095d25b73d54b3a74 in / 
# Fri, 24 Jul 2020 16:25:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:25:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:25:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:25:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ba5c49f251d9cd367877b4bb56a54c6c2cd649877fc1f3866a8c116211dcb43`  
		Last Modified: Fri, 24 Jul 2020 16:27:37 GMT  
		Size: 27.0 MB (26957842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869d6f4731727c8eee5a616ee243640c38bfd44a35c601ca60f3f8976637c7c8`  
		Last Modified: Fri, 24 Jul 2020 16:27:30 GMT  
		Size: 31.8 KB (31835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e46e1d5ec59f731bb7c1ef190b7269114c504db02a71b24bf310a987fb74a0`  
		Last Modified: Fri, 24 Jul 2020 16:27:29 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7393ecc5b169f761ed9ca88de6fc2aed57f05f141499a65a0f1bbeb2244b9b04`  
		Last Modified: Fri, 24 Jul 2020 16:27:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:027242691f288b0770ec88389e9643f7141ac61200396a2a890795c43223a56e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32985345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29933d6f8d91ece30bd342f40955af0eaf4b0cce7cb1e5eaddbac7eea91e32c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:37:12 GMT
ADD file:c00451f5cfe44d733a24fd1ed2ffcd58dd03d160b3be1f23a23c6988bfdde5f9 in / 
# Fri, 24 Jul 2020 14:37:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:37:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ef413e40463b2cc51faddfd43a7ccebc442b8f3e610f2099c9b9f43ab4c794c`  
		Last Modified: Fri, 24 Jul 2020 14:43:13 GMT  
		Size: 33.0 MB (32952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a2aa97dce56eeeb38597752e261e49aa1782887302c44ab406af8642599fc`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 31.7 KB (31677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0098b0f09cf883a00d68448733220790bdd0cf13bdbf30b747c84687fa0ca2`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f899dca8f8bc39cfcda10bb89d224e2d1b4dbcb2a0c7d0b2bfd4e11bd11f0f61`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:2c2f1bd5f0e8469d0913dfcf2f5ebb5e0848f6d1a338b3f6444423a2f7257f83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27263645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6579b622c1a85a84003396d344881960164c590e676d704aee0925dcf753c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:39 GMT
ADD file:c2305b9c6b3d1f88851d28a75f00aefa09cd090dceed56cea0be0ef7848de90d in / 
# Fri, 24 Jul 2020 14:44:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:96ee9d07fad79c13f98051a8b3a80c5aa966b8b8e5c86f129811fc3e03c6a937`  
		Last Modified: Fri, 24 Jul 2020 14:46:02 GMT  
		Size: 27.2 MB (27230132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e509548444259d3ffae6be4cff91bdbd942e76236063786c133bd7a9916cb74`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 32.5 KB (32481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45af8f70e0f28da9bf410c9369c787d38fdd7d9bf805098562a6a4aefe14c3a`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13885bcf94b5ef67414fbe9d1bc297ddc27a295f43fef37c3e0b67cb4449003e`  
		Last Modified: Fri, 24 Jul 2020 14:45:59 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:a61728f6128fb4a7a20efaa7597607ed6e69973ee9b9123e3b4fd28b7bba100b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic` - linux; amd64

```console
$ docker pull ubuntu@sha256:767eea1efb29ab7e215e1d97c8d758df5d587ca86e769a2dfb254c6b022895c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26733500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb2d388e1a255c98029f40d6d7f8029fb13f1030abc8f11ccacbca686a8dc12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:8d8280314eac99b6ce1e5307d0093411150a8c09b59f390658952d50139c4722
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22314138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d364ec676a9895226aa2dad9f3bd193151e824600c1f2d343d4986bc9892b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:04:27 GMT
ADD file:934b4bc073556bbba45a5017b40df7ac076a57b031b6b7225919b1ea3c1d89ff in / 
# Fri, 24 Jul 2020 16:04:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:05:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:05:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:05:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de691405df56c17462a8052d9b88a283d955c448deda7a610d70096a5454ff13`  
		Last Modified: Mon, 13 Jul 2020 15:47:13 GMT  
		Size: 22.3 MB (22277635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a766b93ee2f7ed0525d6d90b71c5e860e5e54d4b5259de86c81e5c49ff120c`  
		Last Modified: Fri, 24 Jul 2020 16:13:28 GMT  
		Size: 35.5 KB (35459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c97e104d7363348d21ddc11159cfa859c18d58712fcafc215fefb535baccbae`  
		Last Modified: Fri, 24 Jul 2020 16:13:28 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a97b3bf2bf845ce898abe48aed267cb2a554e220ee512500495c2791ea6ea8`  
		Last Modified: Fri, 24 Jul 2020 16:13:28 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:c83c9f63974b7a72b38f21fadcaa51ab46a75622c114e41fd7c54c9e7bd1371b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23757364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc42dcf4e4b0b31d8937a7f4521cd709ada553cd1dfd9cfee760daae9a4040f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:515e7c555486235ae2ad9c3820c0edf636aacbf25c8402ae70e1a2c3cd6b28f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27159246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1edaca493ec36631fa0d6bd1101e63b106e4ea23a79278b4bfacd9f4f3f7590f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:18 GMT
ADD file:1041a59a13c0d49b1cb87f211694f68be4c9b76f2deb36e2d8955b77c4d2836f in / 
# Fri, 24 Jul 2020 14:40:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:40:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89823af3b784a3ef6d57a90159cbd5f28c863927aa03d4c43b44b6c37479fa1c`  
		Last Modified: Mon, 13 Jul 2020 15:46:56 GMT  
		Size: 27.1 MB (27123624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28677484c2569b014ecb876df3111b11e825c82629306b3af99a1c12f3b234e2`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 34.6 KB (34611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c914b15d9c03339769ddd662b893654bbc371dbed4f8cdfa29ca1c57c0bb98e`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc7dbf6d65bca5959e6f7c892f468288c27e6a0ef07eec142d4497ee07e6cd`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:654769f02fc482e110ca0aa956d81339397e1aa055cdc4749dc03cd621982598
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30441191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31fb84f9af6f908e395aed2ee0dee54acd0c53e2c99920595d81d8f15afe022d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:7172b354da3696f8faf5edc61bfe7af3e5851a3f872cea86d8696deef1e646df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.4 MB (25406733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d408badaac51c3893ac324d04eb5206662c4fc0adcd48d62121089f72bfdfa8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic-20200807`

```console
$ docker pull ubuntu@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:162ef5d7086f12982b4bd0fb94e9184fa456f6f1b8d345b52379a5b9f838e675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:2fb1f8af49f296081dd4fbf33f3f0c5da3be8dc4c413bb6545628f086c0f6408
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28390799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:188e030eedba1500bd3082eece304c1ee29ac38affada33744f4208cb4248596`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:45 GMT
ADD file:8cda7bfcf6c3010f9498acf5db465d8affd86bacb786338974486e23ea62b05d in / 
# Fri, 24 Jul 2020 14:38:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5f55bfaf77a136f7c6b5063e591480c2e7690ed1c29b0ee354caf8f6c62741e0`  
		Last Modified: Fri, 24 Jul 2020 14:39:44 GMT  
		Size: 28.4 MB (28357957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef373180da2631c7a56d9629e37de8010fe57414453617dde3a2c1e9861f1eb`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 31.8 KB (31838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d10b513df5337d26a6e2ccaf4875267999084d7f0d2f3102c54d7430cfa35`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552f92805e8c6585c466083ac60f40092ae127e794d498c599a31bd67df21c09`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:121bd40b7e5df56bcbfe7650e25f69950a71b1e28a184ec0ec1d0d3052bdd1df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23880255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe68c7eedf153aaa9383c727fe9eabb23558d140653fe488c13d8f67b7e25b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:07:21 GMT
ADD file:52d86d22ed47d0da1087414482ade7e5bded2a6a8d539e7214a7f6433820de24 in / 
# Fri, 24 Jul 2020 16:07:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:08:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:08:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:08:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:abee97477daae5ba1c098c334fa7126af27e46cb55f92383c47ee4752cca6b34`  
		Last Modified: Fri, 24 Jul 2020 16:17:36 GMT  
		Size: 23.8 MB (23847354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6932344878e72d9fc106f6b10714cc0590c46ab1bed3d33b7f005de5e8f44dad`  
		Last Modified: Fri, 24 Jul 2020 16:17:30 GMT  
		Size: 31.9 KB (31864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73c3d9eb80a07ca3c2917ec92d98f1dc20cce68119a1400b6dd5598ed03e90e`  
		Last Modified: Fri, 24 Jul 2020 16:17:29 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642ef31c2598b6d4f19ef5a77988b491517e1fd8fe77d266651b8bf97f76fa25`  
		Last Modified: Fri, 24 Jul 2020 16:17:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f388e7c61860c95e835f7f0257d912dc8677c5fa5d2c3377b7f0fcca5c79ff5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26990712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5131fad3254b5b1bd9a41355df1315aee4a69c76083c63cf79380a5dd888bbdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:25:04 GMT
ADD file:d70c9745470cda91695a18f189dd80bae5a680e704e1763095d25b73d54b3a74 in / 
# Fri, 24 Jul 2020 16:25:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:25:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:25:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:25:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ba5c49f251d9cd367877b4bb56a54c6c2cd649877fc1f3866a8c116211dcb43`  
		Last Modified: Fri, 24 Jul 2020 16:27:37 GMT  
		Size: 27.0 MB (26957842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869d6f4731727c8eee5a616ee243640c38bfd44a35c601ca60f3f8976637c7c8`  
		Last Modified: Fri, 24 Jul 2020 16:27:30 GMT  
		Size: 31.8 KB (31835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e46e1d5ec59f731bb7c1ef190b7269114c504db02a71b24bf310a987fb74a0`  
		Last Modified: Fri, 24 Jul 2020 16:27:29 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7393ecc5b169f761ed9ca88de6fc2aed57f05f141499a65a0f1bbeb2244b9b04`  
		Last Modified: Fri, 24 Jul 2020 16:27:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:027242691f288b0770ec88389e9643f7141ac61200396a2a890795c43223a56e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32985345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29933d6f8d91ece30bd342f40955af0eaf4b0cce7cb1e5eaddbac7eea91e32c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:37:12 GMT
ADD file:c00451f5cfe44d733a24fd1ed2ffcd58dd03d160b3be1f23a23c6988bfdde5f9 in / 
# Fri, 24 Jul 2020 14:37:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:37:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ef413e40463b2cc51faddfd43a7ccebc442b8f3e610f2099c9b9f43ab4c794c`  
		Last Modified: Fri, 24 Jul 2020 14:43:13 GMT  
		Size: 33.0 MB (32952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a2aa97dce56eeeb38597752e261e49aa1782887302c44ab406af8642599fc`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 31.7 KB (31677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0098b0f09cf883a00d68448733220790bdd0cf13bdbf30b747c84687fa0ca2`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f899dca8f8bc39cfcda10bb89d224e2d1b4dbcb2a0c7d0b2bfd4e11bd11f0f61`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:2c2f1bd5f0e8469d0913dfcf2f5ebb5e0848f6d1a338b3f6444423a2f7257f83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27263645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6579b622c1a85a84003396d344881960164c590e676d704aee0925dcf753c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:39 GMT
ADD file:c2305b9c6b3d1f88851d28a75f00aefa09cd090dceed56cea0be0ef7848de90d in / 
# Fri, 24 Jul 2020 14:44:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:96ee9d07fad79c13f98051a8b3a80c5aa966b8b8e5c86f129811fc3e03c6a937`  
		Last Modified: Fri, 24 Jul 2020 14:46:02 GMT  
		Size: 27.2 MB (27230132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e509548444259d3ffae6be4cff91bdbd942e76236063786c133bd7a9916cb74`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 32.5 KB (32481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45af8f70e0f28da9bf410c9369c787d38fdd7d9bf805098562a6a4aefe14c3a`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13885bcf94b5ef67414fbe9d1bc297ddc27a295f43fef37c3e0b67cb4449003e`  
		Last Modified: Fri, 24 Jul 2020 14:45:59 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:5d1d5407f353843ecf8b16524bc5565aa332e9e6a1297c73a92d3e754b8a636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal` - linux; amd64

```console
$ docker pull ubuntu@sha256:60f560e52264ed1cb7829a0d59b1ee7740d7580e0eb293aca2d722136edb1e24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28590639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4467b07108685c38297025797890f0492c4ec509212e2e4b4822d367fe6bc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6701deddfa3bdabb3a50eb0a24175367b9c7b145e8b2f889ee3b2c52a295ec0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014028cfedab937e84159afcad15a9f4fd8ab921268f6f1ca83b49308587a074`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:06:12 GMT
ADD file:bcba01fb27d025c2931e46af0b091f98e743ab46eaa1d2d2dd38e6aeb9706267 in / 
# Fri, 24 Jul 2020 16:06:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:06:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:06:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:06:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86924fd76ad7a77a1ec54ad07fdb4d2d51c12b6070f2dfe92dbf92e3f99702d7`  
		Last Modified: Mon, 20 Jul 2020 15:50:15 GMT  
		Size: 24.0 MB (24034159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e967235e6adc918de90ffb2d143fb1ad2659c63f6c0c8a9c70c8e08bff13917`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 32.3 KB (32349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabf100c8ea14f6342f16b9b10cb81a1355aa9a9d6b8f607c04119c9790f1a51`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344cec738d225bc4e9abb563b22a040685352088e9d588d910c09039fa47ac35`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8351cb483b295a97ee3cc15150285a58ccf0669e422d4730a9a608988bd5e902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27192812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acd9dae93deacc082f1d3643437b1a1ad4df9e53eb561a5e508531a692d7ea80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:24:06 GMT
ADD file:26bd57f1dbcfd1a91715cc84cf0f221783655f16bbb7a912aaf20507cc252535 in / 
# Fri, 24 Jul 2020 16:24:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:24:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:24:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:24:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3583fd5e2faf2976fb6333a3a15414f2708dc284c018a672e37112326bc7b7a1`  
		Last Modified: Mon, 20 Jul 2020 15:50:10 GMT  
		Size: 27.2 MB (27159444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d9e0aed378588f59f8f4276e70ea379b773d7d6507046cd7a044601499785`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 32.3 KB (32333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a6dca9e536449681a937b8f49022cb56b230e352da8aed9b616fadb14dc30`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d9e98650a6106452fc9e640abe8929399fa4f7a0d3ef58a593e8d68cdf3a6`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d5b40885539615b9aeb7119516427959a158386af13e00d79a7da43ad1b3fb87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33312390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8760d637d5ffca565be33295b10ecf04e581ebd433a48dfd5af138a9c801529a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:35:30 GMT
ADD file:fec1d8aac4ab3a3c2326e15808c04b0df4c06c2c4e66d3f34e3e31d3408fd793 in / 
# Fri, 24 Jul 2020 14:35:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:36:13 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:36:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:36:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4739cd2f4f486596c583c79f6033f1a9dee019389d512603609494678c8ccd53`  
		Last Modified: Mon, 20 Jul 2020 15:51:10 GMT  
		Size: 33.3 MB (33279182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f57f5c67707a22a55ae858c6c54f236321b919889f34c321e1a3cc35b9a7988`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 32.2 KB (32166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b0395dde9514c1a521632a61afda1494fe836f816badcab196bd067b4891c`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b459fe5e4dff59e4cc2b4b5207df42a369d6f0ac774f26c55184b3ccd491996`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:5679518149183fed9dcba60e60f35b0a5ceb59e1ad7b7f9143dc227eda68b202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27302775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a934bfaaf1240f4126c0bdb3327ff5a2d58efa5737524e8205376845b6db8b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:16 GMT
ADD file:6c803b66511ab9cbe066bf89c4d7eb4d7ee4e5a277c36a87dcf63834e18fcfb6 in / 
# Fri, 24 Jul 2020 14:44:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72b8403ae854f945520d1213c568e1b3edf3c0c608fa66780ac822be2ce76657`  
		Last Modified: Mon, 20 Jul 2020 15:56:17 GMT  
		Size: 27.3 MB (27268775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824bb95b6ed456a4fb312de39690e22ca2dac1131067ef2e32679e61e1bf4e76`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 33.0 KB (32965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daf151e726997888df7ebd2403777ed7675e924280e5e5a4180528029a48c0c`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72590bfaf79d6d4e391712b6a34001678f6d42795816fc127ce10762be56d826`  
		Last Modified: Fri, 24 Jul 2020 14:45:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal-20200729`

```console
$ docker pull ubuntu@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `ubuntu:groovy`

```console
$ docker pull ubuntu@sha256:162ef5d7086f12982b4bd0fb94e9184fa456f6f1b8d345b52379a5b9f838e675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:groovy` - linux; amd64

```console
$ docker pull ubuntu@sha256:2fb1f8af49f296081dd4fbf33f3f0c5da3be8dc4c413bb6545628f086c0f6408
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28390799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:188e030eedba1500bd3082eece304c1ee29ac38affada33744f4208cb4248596`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:45 GMT
ADD file:8cda7bfcf6c3010f9498acf5db465d8affd86bacb786338974486e23ea62b05d in / 
# Fri, 24 Jul 2020 14:38:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5f55bfaf77a136f7c6b5063e591480c2e7690ed1c29b0ee354caf8f6c62741e0`  
		Last Modified: Fri, 24 Jul 2020 14:39:44 GMT  
		Size: 28.4 MB (28357957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef373180da2631c7a56d9629e37de8010fe57414453617dde3a2c1e9861f1eb`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 31.8 KB (31838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d10b513df5337d26a6e2ccaf4875267999084d7f0d2f3102c54d7430cfa35`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552f92805e8c6585c466083ac60f40092ae127e794d498c599a31bd67df21c09`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:121bd40b7e5df56bcbfe7650e25f69950a71b1e28a184ec0ec1d0d3052bdd1df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23880255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe68c7eedf153aaa9383c727fe9eabb23558d140653fe488c13d8f67b7e25b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:07:21 GMT
ADD file:52d86d22ed47d0da1087414482ade7e5bded2a6a8d539e7214a7f6433820de24 in / 
# Fri, 24 Jul 2020 16:07:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:08:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:08:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:08:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:abee97477daae5ba1c098c334fa7126af27e46cb55f92383c47ee4752cca6b34`  
		Last Modified: Fri, 24 Jul 2020 16:17:36 GMT  
		Size: 23.8 MB (23847354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6932344878e72d9fc106f6b10714cc0590c46ab1bed3d33b7f005de5e8f44dad`  
		Last Modified: Fri, 24 Jul 2020 16:17:30 GMT  
		Size: 31.9 KB (31864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73c3d9eb80a07ca3c2917ec92d98f1dc20cce68119a1400b6dd5598ed03e90e`  
		Last Modified: Fri, 24 Jul 2020 16:17:29 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642ef31c2598b6d4f19ef5a77988b491517e1fd8fe77d266651b8bf97f76fa25`  
		Last Modified: Fri, 24 Jul 2020 16:17:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f388e7c61860c95e835f7f0257d912dc8677c5fa5d2c3377b7f0fcca5c79ff5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26990712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5131fad3254b5b1bd9a41355df1315aee4a69c76083c63cf79380a5dd888bbdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:25:04 GMT
ADD file:d70c9745470cda91695a18f189dd80bae5a680e704e1763095d25b73d54b3a74 in / 
# Fri, 24 Jul 2020 16:25:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:25:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:25:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:25:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ba5c49f251d9cd367877b4bb56a54c6c2cd649877fc1f3866a8c116211dcb43`  
		Last Modified: Fri, 24 Jul 2020 16:27:37 GMT  
		Size: 27.0 MB (26957842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869d6f4731727c8eee5a616ee243640c38bfd44a35c601ca60f3f8976637c7c8`  
		Last Modified: Fri, 24 Jul 2020 16:27:30 GMT  
		Size: 31.8 KB (31835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e46e1d5ec59f731bb7c1ef190b7269114c504db02a71b24bf310a987fb74a0`  
		Last Modified: Fri, 24 Jul 2020 16:27:29 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7393ecc5b169f761ed9ca88de6fc2aed57f05f141499a65a0f1bbeb2244b9b04`  
		Last Modified: Fri, 24 Jul 2020 16:27:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:027242691f288b0770ec88389e9643f7141ac61200396a2a890795c43223a56e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32985345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29933d6f8d91ece30bd342f40955af0eaf4b0cce7cb1e5eaddbac7eea91e32c2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:37:12 GMT
ADD file:c00451f5cfe44d733a24fd1ed2ffcd58dd03d160b3be1f23a23c6988bfdde5f9 in / 
# Fri, 24 Jul 2020 14:37:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:37:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ef413e40463b2cc51faddfd43a7ccebc442b8f3e610f2099c9b9f43ab4c794c`  
		Last Modified: Fri, 24 Jul 2020 14:43:13 GMT  
		Size: 33.0 MB (32952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a2aa97dce56eeeb38597752e261e49aa1782887302c44ab406af8642599fc`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 31.7 KB (31677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0098b0f09cf883a00d68448733220790bdd0cf13bdbf30b747c84687fa0ca2`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f899dca8f8bc39cfcda10bb89d224e2d1b4dbcb2a0c7d0b2bfd4e11bd11f0f61`  
		Last Modified: Fri, 24 Jul 2020 14:43:07 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:groovy` - linux; s390x

```console
$ docker pull ubuntu@sha256:2c2f1bd5f0e8469d0913dfcf2f5ebb5e0848f6d1a338b3f6444423a2f7257f83
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27263645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6579b622c1a85a84003396d344881960164c590e676d704aee0925dcf753c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:39 GMT
ADD file:c2305b9c6b3d1f88851d28a75f00aefa09cd090dceed56cea0be0ef7848de90d in / 
# Fri, 24 Jul 2020 14:44:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:96ee9d07fad79c13f98051a8b3a80c5aa966b8b8e5c86f129811fc3e03c6a937`  
		Last Modified: Fri, 24 Jul 2020 14:46:02 GMT  
		Size: 27.2 MB (27230132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e509548444259d3ffae6be4cff91bdbd942e76236063786c133bd7a9916cb74`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 32.5 KB (32481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45af8f70e0f28da9bf410c9369c787d38fdd7d9bf805098562a6a4aefe14c3a`  
		Last Modified: Fri, 24 Jul 2020 14:45:58 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13885bcf94b5ef67414fbe9d1bc297ddc27a295f43fef37c3e0b67cb4449003e`  
		Last Modified: Fri, 24 Jul 2020 14:45:59 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:groovy-20200812`

```console
$ docker pull ubuntu@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:5d1d5407f353843ecf8b16524bc5565aa332e9e6a1297c73a92d3e754b8a636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:latest` - linux; amd64

```console
$ docker pull ubuntu@sha256:60f560e52264ed1cb7829a0d59b1ee7740d7580e0eb293aca2d722136edb1e24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28590639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4467b07108685c38297025797890f0492c4ec509212e2e4b4822d367fe6bc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6701deddfa3bdabb3a50eb0a24175367b9c7b145e8b2f889ee3b2c52a295ec0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014028cfedab937e84159afcad15a9f4fd8ab921268f6f1ca83b49308587a074`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:06:12 GMT
ADD file:bcba01fb27d025c2931e46af0b091f98e743ab46eaa1d2d2dd38e6aeb9706267 in / 
# Fri, 24 Jul 2020 16:06:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:06:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:06:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:06:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86924fd76ad7a77a1ec54ad07fdb4d2d51c12b6070f2dfe92dbf92e3f99702d7`  
		Last Modified: Mon, 20 Jul 2020 15:50:15 GMT  
		Size: 24.0 MB (24034159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e967235e6adc918de90ffb2d143fb1ad2659c63f6c0c8a9c70c8e08bff13917`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 32.3 KB (32349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabf100c8ea14f6342f16b9b10cb81a1355aa9a9d6b8f607c04119c9790f1a51`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344cec738d225bc4e9abb563b22a040685352088e9d588d910c09039fa47ac35`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8351cb483b295a97ee3cc15150285a58ccf0669e422d4730a9a608988bd5e902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27192812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acd9dae93deacc082f1d3643437b1a1ad4df9e53eb561a5e508531a692d7ea80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:24:06 GMT
ADD file:26bd57f1dbcfd1a91715cc84cf0f221783655f16bbb7a912aaf20507cc252535 in / 
# Fri, 24 Jul 2020 16:24:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:24:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:24:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:24:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3583fd5e2faf2976fb6333a3a15414f2708dc284c018a672e37112326bc7b7a1`  
		Last Modified: Mon, 20 Jul 2020 15:50:10 GMT  
		Size: 27.2 MB (27159444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d9e0aed378588f59f8f4276e70ea379b773d7d6507046cd7a044601499785`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 32.3 KB (32333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a6dca9e536449681a937b8f49022cb56b230e352da8aed9b616fadb14dc30`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d9e98650a6106452fc9e640abe8929399fa4f7a0d3ef58a593e8d68cdf3a6`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d5b40885539615b9aeb7119516427959a158386af13e00d79a7da43ad1b3fb87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33312390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8760d637d5ffca565be33295b10ecf04e581ebd433a48dfd5af138a9c801529a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:35:30 GMT
ADD file:fec1d8aac4ab3a3c2326e15808c04b0df4c06c2c4e66d3f34e3e31d3408fd793 in / 
# Fri, 24 Jul 2020 14:35:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:36:13 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:36:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:36:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4739cd2f4f486596c583c79f6033f1a9dee019389d512603609494678c8ccd53`  
		Last Modified: Mon, 20 Jul 2020 15:51:10 GMT  
		Size: 33.3 MB (33279182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f57f5c67707a22a55ae858c6c54f236321b919889f34c321e1a3cc35b9a7988`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 32.2 KB (32166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b0395dde9514c1a521632a61afda1494fe836f816badcab196bd067b4891c`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b459fe5e4dff59e4cc2b4b5207df42a369d6f0ac774f26c55184b3ccd491996`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:5679518149183fed9dcba60e60f35b0a5ceb59e1ad7b7f9143dc227eda68b202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27302775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a934bfaaf1240f4126c0bdb3327ff5a2d58efa5737524e8205376845b6db8b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:16 GMT
ADD file:6c803b66511ab9cbe066bf89c4d7eb4d7ee4e5a277c36a87dcf63834e18fcfb6 in / 
# Fri, 24 Jul 2020 14:44:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72b8403ae854f945520d1213c568e1b3edf3c0c608fa66780ac822be2ce76657`  
		Last Modified: Mon, 20 Jul 2020 15:56:17 GMT  
		Size: 27.3 MB (27268775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824bb95b6ed456a4fb312de39690e22ca2dac1131067ef2e32679e61e1bf4e76`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 33.0 KB (32965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daf151e726997888df7ebd2403777ed7675e924280e5e5a4180528029a48c0c`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72590bfaf79d6d4e391712b6a34001678f6d42795816fc127ce10762be56d826`  
		Last Modified: Fri, 24 Jul 2020 14:45:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:5d1d5407f353843ecf8b16524bc5565aa332e9e6a1297c73a92d3e754b8a636d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:60f560e52264ed1cb7829a0d59b1ee7740d7580e0eb293aca2d722136edb1e24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28590639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4467b07108685c38297025797890f0492c4ec509212e2e4b4822d367fe6bc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:32 GMT
ADD file:65a1cc50a9867c153deb3bed36d9d51d469fb123df6ee0ba31e01646edf1a1c4 in / 
# Fri, 24 Jul 2020 14:38:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ff22d22a8554f746f90a78b501da38d56a46f2ddba0dfec8b260aebaa61b3ba`  
		Last Modified: Mon, 20 Jul 2020 15:20:12 GMT  
		Size: 28.6 MB (28557306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb79d19722c46b9c0829811d7a5a0ae82c8771ab7f2f68e7d3a3ed6bd5d5d0`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 32.3 KB (32320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d0d660b6a7da8df08a01dbc7250f38cfa2161db00c7c27c0b20be07a8236a`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f616834fd07522cbfd33f0dfa848903599320b5c7191b59fe9aa7562f956a1`  
		Last Modified: Fri, 24 Jul 2020 14:39:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:6701deddfa3bdabb3a50eb0a24175367b9c7b145e8b2f889ee3b2c52a295ec0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24067546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014028cfedab937e84159afcad15a9f4fd8ab921268f6f1ca83b49308587a074`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:06:12 GMT
ADD file:bcba01fb27d025c2931e46af0b091f98e743ab46eaa1d2d2dd38e6aeb9706267 in / 
# Fri, 24 Jul 2020 16:06:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:06:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:06:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:06:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86924fd76ad7a77a1ec54ad07fdb4d2d51c12b6070f2dfe92dbf92e3f99702d7`  
		Last Modified: Mon, 20 Jul 2020 15:50:15 GMT  
		Size: 24.0 MB (24034159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e967235e6adc918de90ffb2d143fb1ad2659c63f6c0c8a9c70c8e08bff13917`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 32.3 KB (32349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabf100c8ea14f6342f16b9b10cb81a1355aa9a9d6b8f607c04119c9790f1a51`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344cec738d225bc4e9abb563b22a040685352088e9d588d910c09039fa47ac35`  
		Last Modified: Fri, 24 Jul 2020 16:14:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:8351cb483b295a97ee3cc15150285a58ccf0669e422d4730a9a608988bd5e902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27192812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acd9dae93deacc082f1d3643437b1a1ad4df9e53eb561a5e508531a692d7ea80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:24:06 GMT
ADD file:26bd57f1dbcfd1a91715cc84cf0f221783655f16bbb7a912aaf20507cc252535 in / 
# Fri, 24 Jul 2020 16:24:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:24:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:24:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:24:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3583fd5e2faf2976fb6333a3a15414f2708dc284c018a672e37112326bc7b7a1`  
		Last Modified: Mon, 20 Jul 2020 15:50:10 GMT  
		Size: 27.2 MB (27159444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d9e0aed378588f59f8f4276e70ea379b773d7d6507046cd7a044601499785`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 32.3 KB (32333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a6dca9e536449681a937b8f49022cb56b230e352da8aed9b616fadb14dc30`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d9e98650a6106452fc9e640abe8929399fa4f7a0d3ef58a593e8d68cdf3a6`  
		Last Modified: Fri, 24 Jul 2020 16:27:14 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d5b40885539615b9aeb7119516427959a158386af13e00d79a7da43ad1b3fb87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33312390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8760d637d5ffca565be33295b10ecf04e581ebd433a48dfd5af138a9c801529a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:35:30 GMT
ADD file:fec1d8aac4ab3a3c2326e15808c04b0df4c06c2c4e66d3f34e3e31d3408fd793 in / 
# Fri, 24 Jul 2020 14:35:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:36:13 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:36:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:36:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4739cd2f4f486596c583c79f6033f1a9dee019389d512603609494678c8ccd53`  
		Last Modified: Mon, 20 Jul 2020 15:51:10 GMT  
		Size: 33.3 MB (33279182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f57f5c67707a22a55ae858c6c54f236321b919889f34c321e1a3cc35b9a7988`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 32.2 KB (32166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b0395dde9514c1a521632a61afda1494fe836f816badcab196bd067b4891c`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b459fe5e4dff59e4cc2b4b5207df42a369d6f0ac774f26c55184b3ccd491996`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:5679518149183fed9dcba60e60f35b0a5ceb59e1ad7b7f9143dc227eda68b202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27302775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a934bfaaf1240f4126c0bdb3327ff5a2d58efa5737524e8205376845b6db8b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:44:16 GMT
ADD file:6c803b66511ab9cbe066bf89c4d7eb4d7ee4e5a277c36a87dcf63834e18fcfb6 in / 
# Fri, 24 Jul 2020 14:44:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72b8403ae854f945520d1213c568e1b3edf3c0c608fa66780ac822be2ce76657`  
		Last Modified: Mon, 20 Jul 2020 15:56:17 GMT  
		Size: 27.3 MB (27268775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824bb95b6ed456a4fb312de39690e22ca2dac1131067ef2e32679e61e1bf4e76`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 33.0 KB (32965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daf151e726997888df7ebd2403777ed7675e924280e5e5a4180528029a48c0c`  
		Last Modified: Fri, 24 Jul 2020 14:45:44 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72590bfaf79d6d4e391712b6a34001678f6d42795816fc127ce10762be56d826`  
		Last Modified: Fri, 24 Jul 2020 14:45:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty`

```console
$ docker pull ubuntu@sha256:ffc76f71dd8be8c9e222d420dc96901a07b61616689a44c7b3ef6a10b7213de4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:trusty` - linux; amd64

```console
$ docker pull ubuntu@sha256:bd0223687054d0f8884fc9e872392c6385a3195d612400495962e270b572ed06
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4f1fe62ff14a4c8119781d47a3739fa97c190e1df38e868794ad7a7cf50a48`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:23:42 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 19 Dec 2019 04:23:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:23:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:23:45 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:23:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bb187ac3fc6c428f38d46409e7765a18dc6b59bc99914f0ba6936463307ec8`  
		Last Modified: Thu, 19 Dec 2019 04:25:41 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a5bcc4a58aeed61f7dbe0a859aa4d37db24efd0c3ca58fb83605b5ad9044b5`  
		Last Modified: Thu, 19 Dec 2019 04:25:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3fc5c28a28125d304462d5b9292d64a61041350304ac5deab416271b25d2e219
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67449d6018f689b7a2a501426015e0b13ada33b377c4c935c68453ce13706712`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:12:57 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Thu, 19 Dec 2019 06:13:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 06:13:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 06:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 06:13:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08b117a826b8d1ae5a5995f7eab5a89f5d582f24fa0016182b6502e42322179`  
		Last Modified: Thu, 19 Dec 2019 06:15:41 GMT  
		Size: 76.8 KB (76765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d5442ddd2dd606cb4dbd9c7243b10f6848c3ee77c176d1b0c667a2232b900c`  
		Last Modified: Thu, 19 Dec 2019 06:15:42 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:79b0f81ad6fc8f0bced3919beee0a79d60d1c8358911188d0787b1f155656d84
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104c127e75190df2e80d312958f30c9b7d2da0b5356f6c1e81e92dc85d3f9740`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:04 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Thu, 19 Dec 2019 03:54:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:54:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:54:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9592077f8570e1222c5a6930a2fdc85b6b607b6c91230a5762c7bd6d84749e25`  
		Last Modified: Thu, 19 Dec 2019 03:56:48 GMT  
		Size: 59.1 KB (59094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b48639f381d2e2566e4c5bdb9792e8666ac2d2cc22918fda5751b8784ee5a5`  
		Last Modified: Thu, 19 Dec 2019 03:56:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; 386

```console
$ docker pull ubuntu@sha256:c8c1d2e6d53d94ef32e73354d146dc6e39c19ce8db2692356b3a6eef5a8ab956
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b01d68827fff530f34f6ff966823624238b7b90aec1bc82b2a9468da476d20e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:42:13 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 19 Dec 2019 04:42:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:42:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:42:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:42:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df46dbd3c04fd4a00981fd885f4d30a154ffa34bc8329bd448e9ca469df32e1`  
		Last Modified: Thu, 19 Dec 2019 04:43:42 GMT  
		Size: 64.9 KB (64855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4ca1e6e5f77f07de7e2107adcb062e1e72e84ce6ff83d5beeb5f84dfcc8418`  
		Last Modified: Thu, 19 Dec 2019 04:43:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d00cd5726fb0c0523960683e45fe4bbb3807e68ef3edff693d44454aad69b85b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce257c90d69b5ed2a0955447f934ed3a9bc17c4f723fd6f61c0f55218e507b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:20:59 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Thu, 19 Dec 2019 04:21:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d17944a6ab7c0a73210db128de5b677c26f0d4c4c59f3bf6c76b7d1e847098`  
		Last Modified: Thu, 19 Dec 2019 04:26:36 GMT  
		Size: 63.4 KB (63423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d84211dbdd608b55c60bac1fab57fed3dd6de92653162fe123fd0154bcb03e`  
		Last Modified: Thu, 19 Dec 2019 04:26:35 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:trusty-20191217`

```console
$ docker pull ubuntu@sha256:ffc76f71dd8be8c9e222d420dc96901a07b61616689a44c7b3ef6a10b7213de4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ubuntu:trusty-20191217` - linux; amd64

```console
$ docker pull ubuntu@sha256:bd0223687054d0f8884fc9e872392c6385a3195d612400495962e270b572ed06
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70764399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4f1fe62ff14a4c8119781d47a3739fa97c190e1df38e868794ad7a7cf50a48`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:23:42 GMT
ADD file:276b5d943a4d284f8a7b249176a31f93d95e852480c2b851de287e53ff622bba in / 
# Thu, 19 Dec 2019 04:23:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:23:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:23:45 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:23:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2e6e20c8e2e69fa5c3fcc310f419975cef5fbeb6f7f2fe1374071141281b6a06`  
		Last Modified: Wed, 18 Dec 2019 13:21:28 GMT  
		Size: 70.7 MB (70691577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bb187ac3fc6c428f38d46409e7765a18dc6b59bc99914f0ba6936463307ec8`  
		Last Modified: Thu, 19 Dec 2019 04:25:41 GMT  
		Size: 72.7 KB (72659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a5bcc4a58aeed61f7dbe0a859aa4d37db24efd0c3ca58fb83605b5ad9044b5`  
		Last Modified: Thu, 19 Dec 2019 04:25:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3fc5c28a28125d304462d5b9292d64a61041350304ac5deab416271b25d2e219
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64700967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67449d6018f689b7a2a501426015e0b13ada33b377c4c935c68453ce13706712`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:12:57 GMT
ADD file:e9d55e059869915743a8ca8e64582d23c48fe7e90e439daccd56d3e08e8673b4 in / 
# Thu, 19 Dec 2019 06:13:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 06:13:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 06:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 06:13:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0db3a87a3d7959895fd860c8b924980adda6e77f5d315b6676a4ac0e12518978`  
		Last Modified: Thu, 19 Dec 2019 06:16:01 GMT  
		Size: 64.6 MB (64624015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08b117a826b8d1ae5a5995f7eab5a89f5d582f24fa0016182b6502e42322179`  
		Last Modified: Thu, 19 Dec 2019 06:15:41 GMT  
		Size: 76.8 KB (76765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d5442ddd2dd606cb4dbd9c7243b10f6848c3ee77c176d1b0c667a2232b900c`  
		Last Modified: Thu, 19 Dec 2019 06:15:42 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:79b0f81ad6fc8f0bced3919beee0a79d60d1c8358911188d0787b1f155656d84
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104c127e75190df2e80d312958f30c9b7d2da0b5356f6c1e81e92dc85d3f9740`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:54:04 GMT
ADD file:b0eb0db52e323748ea9b8d7f8aecbc523a747619cd08663bab0fe60ab59bc60e in / 
# Thu, 19 Dec 2019 03:54:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:54:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:54:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1a5a1e51f251c3431dec02e2cc8d157e92d1b46913708ce9e600747a6274977`  
		Last Modified: Thu, 19 Dec 2019 03:57:08 GMT  
		Size: 66.5 MB (66466219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9592077f8570e1222c5a6930a2fdc85b6b607b6c91230a5762c7bd6d84749e25`  
		Last Modified: Thu, 19 Dec 2019 03:56:48 GMT  
		Size: 59.1 KB (59094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b48639f381d2e2566e4c5bdb9792e8666ac2d2cc22918fda5751b8784ee5a5`  
		Last Modified: Thu, 19 Dec 2019 03:56:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; 386

```console
$ docker pull ubuntu@sha256:c8c1d2e6d53d94ef32e73354d146dc6e39c19ce8db2692356b3a6eef5a8ab956
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68445457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b01d68827fff530f34f6ff966823624238b7b90aec1bc82b2a9468da476d20e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:42:13 GMT
ADD file:e034601a525da53b0f39bb04d6e2264e2a592d0ae7c21e00697b9b62ca1efec9 in / 
# Thu, 19 Dec 2019 04:42:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:42:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:42:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:42:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:630712fe5783a35ad52a7026002143cb4f8fe65d34097dcaa4c4331b1b059a17`  
		Last Modified: Thu, 19 Dec 2019 04:44:02 GMT  
		Size: 68.4 MB (68380440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df46dbd3c04fd4a00981fd885f4d30a154ffa34bc8329bd448e9ca469df32e1`  
		Last Modified: Thu, 19 Dec 2019 04:43:42 GMT  
		Size: 64.9 KB (64855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4ca1e6e5f77f07de7e2107adcb062e1e72e84ce6ff83d5beeb5f84dfcc8418`  
		Last Modified: Thu, 19 Dec 2019 04:43:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:trusty-20191217` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d00cd5726fb0c0523960683e45fe4bbb3807e68ef3edff693d44454aad69b85b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73443147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce257c90d69b5ed2a0955447f934ed3a9bc17c4f723fd6f61c0f55218e507b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:20:59 GMT
ADD file:581665e92c72c8638b40fe509de6479dc1a5d7b5ffe8d6706006178c406e35e2 in / 
# Thu, 19 Dec 2019 04:21:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bed4146d918c6c9a57bc3a8bf829e702975b0e53c7f25920fe9435b58ed6b64f`  
		Last Modified: Thu, 19 Dec 2019 04:26:52 GMT  
		Size: 73.4 MB (73379539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d17944a6ab7c0a73210db128de5b677c26f0d4c4c59f3bf6c76b7d1e847098`  
		Last Modified: Thu, 19 Dec 2019 04:26:36 GMT  
		Size: 63.4 KB (63423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d84211dbdd608b55c60bac1fab57fed3dd6de92653162fe123fd0154bcb03e`  
		Last Modified: Thu, 19 Dec 2019 04:26:35 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial`

```console
$ docker pull ubuntu@sha256:0eb024b1147ab61246cfdbdf05c128550ede262790b25a8a6fd93dd3385ab1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:xenial` - linux; amd64

```console
$ docker pull ubuntu@sha256:cc4755a9f2f76ca73055da11f1bdc01d65ce79202a68b041c67c32770c71954b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44402566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab5e942c505d079974d0bb27608d178568973389fd6aadc72c383dee53148a1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:06 GMT
ADD file:513ae777bc4042f8446c0454f8cffc9a94f8429de963651d9a6dab95d4502007 in / 
# Fri, 24 Jul 2020 14:39:07 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:39:08 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:39:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7b378fa0f9085667ced1c76c9919cde8663becf2218e8d20e2df8d0824311531`  
		Last Modified: Tue, 07 Jul 2020 13:19:56 GMT  
		Size: 44.4 MB (44401021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d77b1b29f2e9b6f141b9d8f74b601f40eb998544783f4a0a3cdc384873c1a4e`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c793be88baee3f3204444e4d4e49c4e44c1709d40182c131cd5681c94e17227`  
		Last Modified: Fri, 24 Jul 2020 14:39:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc05c8a19c0cf83f2f44263c967c3fe81fffc4b41b592ad088fb1534c206e70`  
		Last Modified: Fri, 24 Jul 2020 14:39:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d636745b3c2a4b672644c9d1ef071bf62022a15ac0504362bf27846831a5825b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39024526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76cfa4cd6fd320d3537be33628d202f5bb55c3d2050c808751480aa7152af128`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:09:57 GMT
ADD file:c7836321aa9dc9832d8e14c042281f4a3525083619649e000d08159b6da79460 in / 
# Fri, 24 Jul 2020 16:10:21 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:11:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:11:42 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:11:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:111f37a6818f459bbc8076c0f741a76111210d34c5738743f43dc1488cf91458`  
		Last Modified: Mon, 13 Jul 2020 15:55:00 GMT  
		Size: 39.0 MB (39022996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa2e8f0d9a725920aa624702144baeaae474875e43f4515d9e69c2bddec4bf`  
		Last Modified: Fri, 24 Jul 2020 16:20:13 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c110f6a5721b4e19fdabed9edeb5446f52132952947cd7b409ac4d4e50b7dc02`  
		Last Modified: Fri, 24 Jul 2020 16:20:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07bd4b31471725e34aa841d95fec2e7425ac418ee0a0f69b6d5ca73c6a17c9e`  
		Last Modified: Fri, 24 Jul 2020 16:20:13 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:efe1dd034811acce9285ab90d22163797ad89997ea736a82da39b449d7981817
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40052287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e092214ffcd69f275e4f62a9012475d13aaeddbf3fe2955c5d9d025aa2997d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 16:25:59 GMT
ADD file:d816988decfebf469e2b28b4858ce7d4a991a101957a43051324255fbe64c86e in / 
# Fri, 24 Jul 2020 16:26:14 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:26:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:26:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f783735449ae0b09fb9e5ee128904f2f3131f6ba46fcf1350fb6a10f872866be`  
		Last Modified: Tue, 07 Jul 2020 00:25:09 GMT  
		Size: 40.1 MB (40050796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35a03aa6fbe0d9147b23501e6fa41d33cd4489470455008ddcbe201063d7b98`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55e221892467d43fdd76b2b592c2fe46e1c69b08e0e9b94f2b383f38e681f65`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a9069021914a77a3d51ffbff02ea5b8a200180601b2be52e9f98d31b6f1389`  
		Last Modified: Fri, 24 Jul 2020 16:27:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; 386

```console
$ docker pull ubuntu@sha256:ea9f9fde6a023145c143db5546e03439aef953cdb120154a44fb6d6c2b6a354e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44309561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032561d1b1b13cfc7d45b69eb922b7d469020682f7602a0299b511840af082cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:38 GMT
ADD file:0281a09e4b674b2f3a51152f0248e69f839a107f4f471cb0f27eff2b47ab726f in / 
# Fri, 24 Jul 2020 14:40:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:40:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c0e0b433333915e5da26fd00978221162b377102e5592ae0404898aee9034774`  
		Last Modified: Mon, 13 Jul 2020 15:54:54 GMT  
		Size: 44.3 MB (44308027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe61969407896fc6a99d8afd1014a71214e79872ad515cb536fb625f179bbef`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058d18b29821b7997f08813144585afd758722b51207239ee260207de7afbc9c`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c34ee61901e83a038c1c1b44b6fa3e2636045fa919ae5ea8b7b37020e71ae`  
		Last Modified: Fri, 24 Jul 2020 14:41:00 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:e5ec578bd8c334d7c9849fd9bbaa78ec25f2b51b0bf7c9e18b1e9b7ca32d6681
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46213021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8ff96d89d56684a658e9b6a3c3891de598dea918df7286e1440bd359ab1f71`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:39:02 GMT
ADD file:dcd2851859d61fd28750e405e189b57c4be98decb40630483b321127e70c7e09 in / 
# Fri, 24 Jul 2020 14:39:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:39:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b63cedd79494e27389a6587d305305c6405fd695b4ec7afb75d1f68bf207ef26`  
		Last Modified: Mon, 13 Jul 2020 15:56:00 GMT  
		Size: 46.2 MB (46211522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a78d9771dc7acf0b6f60d469c9b7a9e77989fd64a0b0efb42e1f33bafd86065`  
		Last Modified: Fri, 24 Jul 2020 14:43:33 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed6828e9eba3a3a47f543b8e5cd196fc712376d35e3b4eb322896a90501447f`  
		Last Modified: Fri, 24 Jul 2020 14:43:34 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5111fc2327dba7ff082661e123c7a3589ad2d5cd4dcc2588f1eefc61c8162f4`  
		Last Modified: Fri, 24 Jul 2020 14:43:34 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:xenial` - linux; s390x

```console
$ docker pull ubuntu@sha256:91c8408fcd69b67621810e2787ab8f661a7449ee2f7a0133f0b0771dcb0b1091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42931004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9fe172094fed28581ee6cb7a799cfabb4076d2445205b27336147f780e7a9ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:45:03 GMT
ADD file:bf2a54d719510136249335d267c595d8495031cf3ed3d69c9975f05444bb5129 in / 
# Fri, 24 Jul 2020 14:45:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:45:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:45:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:45:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dbf86c3f4bdb4fdbb59faf631c0d05be1eb33fe938b6332ee07ab035db0a4f8e`  
		Last Modified: Mon, 13 Jul 2020 15:56:10 GMT  
		Size: 42.9 MB (42929517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ce80f41f1cfc5a98c8078530c4618f86fa77832bdf0b0bb484211359473956`  
		Last Modified: Fri, 24 Jul 2020 14:46:17 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdadef093efdb822d71f1ac71a76f40485cac65269a99e6cb366a8fd5548f7d`  
		Last Modified: Fri, 24 Jul 2020 14:46:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f849fe87969087a98487dbc416d25c3dda1b7f7aae893a93963b8615ca8b7903`  
		Last Modified: Fri, 24 Jul 2020 14:46:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:xenial-20200807`

```console
$ docker pull ubuntu@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
