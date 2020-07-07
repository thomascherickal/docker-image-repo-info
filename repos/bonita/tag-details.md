<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.5`](#bonita7105)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.0`](#bonita7110)
-	[`bonita:7.9`](#bonita79)
-	[`bonita:7.9.5`](#bonita795)
-	[`bonita:latest`](#bonitalatest)

## `bonita:7.10`

```console
$ docker pull bonita@sha256:32c8143dff9c76bd0bdf9d41bc7bf3941a39018bae7277d4572102f70b785102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:eb4d7a205ffc6a9f110dae4481722dd3935b5dffb8d74c6be4aa4f5b85bc0686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227146063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e7decd716da9d1fc3323e5c275590a00408fa98b482f0e341c60afe53aaf78`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:07 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BONITA_VERSION=7.10.5
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Mon, 06 Jul 2020 23:31:09 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:31:16 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:19 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:20 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:20 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Mon, 06 Jul 2020 23:31:21 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:31:21 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a708f4afdad4d442ee8c954a6657a5edcef0aafefc7f21953aab284f34fa62d4`  
		Last Modified: Mon, 06 Jul 2020 23:32:11 GMT  
		Size: 98.0 MB (97955936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762143c90eb69055f0c62282e83c6cd1082a1bd36c35d1edb57f481702225d6d`  
		Last Modified: Mon, 06 Jul 2020 23:32:06 GMT  
		Size: 7.6 KB (7594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08259ac08f873cd77008a8dfaf29087fb83c491f3a0b9b54bedc0d83a9ff1a1e`  
		Last Modified: Mon, 06 Jul 2020 23:32:07 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:91bdf7ed71893cd85ad5cbd211e1c6ae69a7888d56fb666178a14f72f9b2eb8d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.2 MB (215153016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04b5195bf91bdb8232f189d5dc8383c4fb03ab83eecbe224181f30724aa0f7c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:43:21 GMT
ARG BASE_URL
# Wed, 17 Jun 2020 02:43:22 GMT
ARG BONITA_URL
# Wed, 17 Jun 2020 02:43:23 GMT
ENV BONITA_VERSION=7.10.5
# Wed, 17 Jun 2020 02:43:24 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Wed, 17 Jun 2020 02:43:26 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 17 Jun 2020 02:43:27 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Wed, 17 Jun 2020 02:43:30 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 17 Jun 2020 02:43:39 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 17 Jun 2020 02:43:41 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 17 Jun 2020 02:43:44 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 17 Jun 2020 02:43:45 GMT
VOLUME [/opt/bonita]
# Wed, 17 Jun 2020 02:43:46 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 17 Jun 2020 02:43:47 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 17 Jun 2020 02:43:47 GMT
EXPOSE 8080
# Wed, 17 Jun 2020 02:43:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3601430c499d32abe16da3e4266438d956207eaad1d46e5d232c3d1290e2264e`  
		Last Modified: Wed, 17 Jun 2020 02:44:46 GMT  
		Size: 98.0 MB (97955965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cdfd3afe32da65d05cb95c8acb480eeb3a45b54a3899b45dd178542a13045`  
		Last Modified: Wed, 17 Jun 2020 02:44:36 GMT  
		Size: 7.6 KB (7620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d0cd1b984a5aa8bca584efee31e40a335e4ac0dcb31ce85baa1a85b7087b9`  
		Last Modified: Wed, 17 Jun 2020 02:44:36 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:fe98c4bfef12e50b9c92ded113bcab54cf93207a4714bd19982f3432740d8a3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223809322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b796d7481a9fcb77c3b11362971db7482ac03eb7e34f33c9d8c7fcffade7e3c6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:29 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:36 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:41 GMT
ENV BONITA_VERSION=7.10.5
# Mon, 06 Jul 2020 23:31:45 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Mon, 06 Jul 2020 23:31:50 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Mon, 06 Jul 2020 23:31:55 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Mon, 06 Jul 2020 23:32:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:33:02 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:33:12 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:33:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:33:21 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:33:23 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Mon, 06 Jul 2020 23:33:24 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:33:26 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:33:28 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3b19161aa1287dd100dcb895b6eb1c4b0364d4d38ee06e438ebc47289f8b8a`  
		Last Modified: Mon, 06 Jul 2020 23:36:12 GMT  
		Size: 98.0 MB (97955972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d1dae53164aeea768398f8ba8c1a0766e1aca199face47458ffa5707d52af8`  
		Last Modified: Mon, 06 Jul 2020 23:36:05 GMT  
		Size: 7.6 KB (7622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d954c8016670d80c013f1d9a57b7f3617678d44e00f9f199b36e3b4a4fc34024`  
		Last Modified: Mon, 06 Jul 2020 23:36:04 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.5`

```console
$ docker pull bonita@sha256:32c8143dff9c76bd0bdf9d41bc7bf3941a39018bae7277d4572102f70b785102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.5` - linux; amd64

```console
$ docker pull bonita@sha256:eb4d7a205ffc6a9f110dae4481722dd3935b5dffb8d74c6be4aa4f5b85bc0686
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227146063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e7decd716da9d1fc3323e5c275590a00408fa98b482f0e341c60afe53aaf78`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:07 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BONITA_VERSION=7.10.5
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Mon, 06 Jul 2020 23:31:08 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Mon, 06 Jul 2020 23:31:09 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:31:16 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:19 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:20 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:20 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Mon, 06 Jul 2020 23:31:21 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:31:21 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a708f4afdad4d442ee8c954a6657a5edcef0aafefc7f21953aab284f34fa62d4`  
		Last Modified: Mon, 06 Jul 2020 23:32:11 GMT  
		Size: 98.0 MB (97955936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762143c90eb69055f0c62282e83c6cd1082a1bd36c35d1edb57f481702225d6d`  
		Last Modified: Mon, 06 Jul 2020 23:32:06 GMT  
		Size: 7.6 KB (7594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08259ac08f873cd77008a8dfaf29087fb83c491f3a0b9b54bedc0d83a9ff1a1e`  
		Last Modified: Mon, 06 Jul 2020 23:32:07 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.5` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:91bdf7ed71893cd85ad5cbd211e1c6ae69a7888d56fb666178a14f72f9b2eb8d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.2 MB (215153016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04b5195bf91bdb8232f189d5dc8383c4fb03ab83eecbe224181f30724aa0f7c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:43:21 GMT
ARG BASE_URL
# Wed, 17 Jun 2020 02:43:22 GMT
ARG BONITA_URL
# Wed, 17 Jun 2020 02:43:23 GMT
ENV BONITA_VERSION=7.10.5
# Wed, 17 Jun 2020 02:43:24 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Wed, 17 Jun 2020 02:43:26 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 17 Jun 2020 02:43:27 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Wed, 17 Jun 2020 02:43:30 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 17 Jun 2020 02:43:39 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 17 Jun 2020 02:43:41 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 17 Jun 2020 02:43:44 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 17 Jun 2020 02:43:45 GMT
VOLUME [/opt/bonita]
# Wed, 17 Jun 2020 02:43:46 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 17 Jun 2020 02:43:47 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 17 Jun 2020 02:43:47 GMT
EXPOSE 8080
# Wed, 17 Jun 2020 02:43:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3601430c499d32abe16da3e4266438d956207eaad1d46e5d232c3d1290e2264e`  
		Last Modified: Wed, 17 Jun 2020 02:44:46 GMT  
		Size: 98.0 MB (97955965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cdfd3afe32da65d05cb95c8acb480eeb3a45b54a3899b45dd178542a13045`  
		Last Modified: Wed, 17 Jun 2020 02:44:36 GMT  
		Size: 7.6 KB (7620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d0cd1b984a5aa8bca584efee31e40a335e4ac0dcb31ce85baa1a85b7087b9`  
		Last Modified: Wed, 17 Jun 2020 02:44:36 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.5` - linux; ppc64le

```console
$ docker pull bonita@sha256:fe98c4bfef12e50b9c92ded113bcab54cf93207a4714bd19982f3432740d8a3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223809322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b796d7481a9fcb77c3b11362971db7482ac03eb7e34f33c9d8c7fcffade7e3c6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:29 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:36 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:41 GMT
ENV BONITA_VERSION=7.10.5
# Mon, 06 Jul 2020 23:31:45 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Mon, 06 Jul 2020 23:31:50 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Mon, 06 Jul 2020 23:31:55 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Mon, 06 Jul 2020 23:32:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:33:02 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:33:12 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:33:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:33:21 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:33:23 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Mon, 06 Jul 2020 23:33:24 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:33:26 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:33:28 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3b19161aa1287dd100dcb895b6eb1c4b0364d4d38ee06e438ebc47289f8b8a`  
		Last Modified: Mon, 06 Jul 2020 23:36:12 GMT  
		Size: 98.0 MB (97955972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d1dae53164aeea768398f8ba8c1a0766e1aca199face47458ffa5707d52af8`  
		Last Modified: Mon, 06 Jul 2020 23:36:05 GMT  
		Size: 7.6 KB (7622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d954c8016670d80c013f1d9a57b7f3617678d44e00f9f199b36e3b4a4fc34024`  
		Last Modified: Mon, 06 Jul 2020 23:36:04 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:6308fad666eb7e7172454a573194e470a3ee5cd0140386383c34c01d5c96db78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:a3edb90d54c87cbf5c2b1261eae54bee1d51a2bb5031d0a4095007b445c39eef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.4 MB (242411758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbd3922096b5c8ca88961188b6fd81ef214b805b99ac5c83ad3a01ff2269049e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:07 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:26 GMT
ENV BONITA_VERSION=7.11.0
# Mon, 06 Jul 2020 23:31:26 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Mon, 06 Jul 2020 23:31:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 06 Jul 2020 23:31:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Mon, 06 Jul 2020 23:31:27 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:31:30 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:34 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:34 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Mon, 06 Jul 2020 23:31:34 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Mon, 06 Jul 2020 23:31:34 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bf9960435230d25d853029b722cbe0fa0e3952311e2e55e1224cba6663300d`  
		Last Modified: Mon, 06 Jul 2020 23:32:24 GMT  
		Size: 113.2 MB (113221577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bc491840b73f5b999f686279c9f60258d368198a2d6892c421624499d5767`  
		Last Modified: Mon, 06 Jul 2020 23:32:18 GMT  
		Size: 7.6 KB (7597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bebeec36e0817b89a37dd029791681652e61daba9cb1c38dadfa6c3bfc90f97`  
		Last Modified: Mon, 06 Jul 2020 23:32:19 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:65ba0e2092b7bafa8f4c812130451af1c212c08775aff508d87cd7e1cb9f83c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230418729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5464e79dfb5c4d44ac9d5c6408232297da9600beda3dac56079fc0d127efab8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:43:21 GMT
ARG BASE_URL
# Wed, 17 Jun 2020 02:43:22 GMT
ARG BONITA_URL
# Wed, 24 Jun 2020 17:40:14 GMT
ENV BONITA_VERSION=7.11.0
# Wed, 24 Jun 2020 17:40:15 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Wed, 24 Jun 2020 17:40:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 24 Jun 2020 17:40:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Wed, 24 Jun 2020 17:40:19 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 24 Jun 2020 17:40:28 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 24 Jun 2020 17:40:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 24 Jun 2020 17:40:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 24 Jun 2020 17:40:34 GMT
VOLUME [/opt/bonita]
# Fri, 03 Jul 2020 17:39:47 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Fri, 03 Jul 2020 17:39:48 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 03 Jul 2020 17:39:49 GMT
EXPOSE 8080
# Fri, 03 Jul 2020 17:39:49 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee3b35a452661ddca4c2185aeaeaf603b1937d0b4115a8ed159e89b484d9029`  
		Last Modified: Wed, 24 Jun 2020 17:41:00 GMT  
		Size: 113.2 MB (113221612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3693802575293a0aece91313aedab1a4c96463acb5c399ab24bf64eda2e15e6c`  
		Last Modified: Fri, 03 Jul 2020 17:40:03 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1103b7a50b8f307fffc3657789584c32b8df6e7097dcbf8a21981b7bd1309e12`  
		Last Modified: Fri, 03 Jul 2020 17:40:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:abb6bf1f182f6660be47c25185a09eb26cfeabba37dd10fcbb67912d9dc43ed7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239075022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9b91e6a4d1f55558e53cda217ce77753552451fc11263166637ac7fa026f6e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:29 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:36 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:33:40 GMT
ENV BONITA_VERSION=7.11.0
# Mon, 06 Jul 2020 23:33:43 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Mon, 06 Jul 2020 23:33:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 06 Jul 2020 23:33:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Mon, 06 Jul 2020 23:33:57 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:34:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:34:21 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:34:29 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:34:31 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:34:32 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Mon, 06 Jul 2020 23:34:35 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Mon, 06 Jul 2020 23:34:48 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:34:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9139e63dbdf506429f6bb9a8559dd330a603e7b6ed4349cc7e5d0e384b034c`  
		Last Modified: Mon, 06 Jul 2020 23:36:35 GMT  
		Size: 113.2 MB (113221612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c5c66750ebbdcfa12195c7cd8891dff5cbb4f5bec172b8022890283de38e5c`  
		Last Modified: Mon, 06 Jul 2020 23:36:29 GMT  
		Size: 7.6 KB (7630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a171764f467afbee2a75fb679968cd7d8c4b9c3eed16d524a4569c3710be7`  
		Last Modified: Mon, 06 Jul 2020 23:36:27 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.0`

```console
$ docker pull bonita@sha256:6308fad666eb7e7172454a573194e470a3ee5cd0140386383c34c01d5c96db78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.0` - linux; amd64

```console
$ docker pull bonita@sha256:a3edb90d54c87cbf5c2b1261eae54bee1d51a2bb5031d0a4095007b445c39eef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.4 MB (242411758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbd3922096b5c8ca88961188b6fd81ef214b805b99ac5c83ad3a01ff2269049e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:07 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:26 GMT
ENV BONITA_VERSION=7.11.0
# Mon, 06 Jul 2020 23:31:26 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Mon, 06 Jul 2020 23:31:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 06 Jul 2020 23:31:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Mon, 06 Jul 2020 23:31:27 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:31:30 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:34 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:34 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Mon, 06 Jul 2020 23:31:34 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Mon, 06 Jul 2020 23:31:34 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bf9960435230d25d853029b722cbe0fa0e3952311e2e55e1224cba6663300d`  
		Last Modified: Mon, 06 Jul 2020 23:32:24 GMT  
		Size: 113.2 MB (113221577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bc491840b73f5b999f686279c9f60258d368198a2d6892c421624499d5767`  
		Last Modified: Mon, 06 Jul 2020 23:32:18 GMT  
		Size: 7.6 KB (7597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bebeec36e0817b89a37dd029791681652e61daba9cb1c38dadfa6c3bfc90f97`  
		Last Modified: Mon, 06 Jul 2020 23:32:19 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:65ba0e2092b7bafa8f4c812130451af1c212c08775aff508d87cd7e1cb9f83c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230418729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5464e79dfb5c4d44ac9d5c6408232297da9600beda3dac56079fc0d127efab8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:43:21 GMT
ARG BASE_URL
# Wed, 17 Jun 2020 02:43:22 GMT
ARG BONITA_URL
# Wed, 24 Jun 2020 17:40:14 GMT
ENV BONITA_VERSION=7.11.0
# Wed, 24 Jun 2020 17:40:15 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Wed, 24 Jun 2020 17:40:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 24 Jun 2020 17:40:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Wed, 24 Jun 2020 17:40:19 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 24 Jun 2020 17:40:28 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 24 Jun 2020 17:40:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 24 Jun 2020 17:40:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 24 Jun 2020 17:40:34 GMT
VOLUME [/opt/bonita]
# Fri, 03 Jul 2020 17:39:47 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Fri, 03 Jul 2020 17:39:48 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 03 Jul 2020 17:39:49 GMT
EXPOSE 8080
# Fri, 03 Jul 2020 17:39:49 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee3b35a452661ddca4c2185aeaeaf603b1937d0b4115a8ed159e89b484d9029`  
		Last Modified: Wed, 24 Jun 2020 17:41:00 GMT  
		Size: 113.2 MB (113221612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3693802575293a0aece91313aedab1a4c96463acb5c399ab24bf64eda2e15e6c`  
		Last Modified: Fri, 03 Jul 2020 17:40:03 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1103b7a50b8f307fffc3657789584c32b8df6e7097dcbf8a21981b7bd1309e12`  
		Last Modified: Fri, 03 Jul 2020 17:40:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:abb6bf1f182f6660be47c25185a09eb26cfeabba37dd10fcbb67912d9dc43ed7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239075022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9b91e6a4d1f55558e53cda217ce77753552451fc11263166637ac7fa026f6e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:29 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:36 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:33:40 GMT
ENV BONITA_VERSION=7.11.0
# Mon, 06 Jul 2020 23:33:43 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Mon, 06 Jul 2020 23:33:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 06 Jul 2020 23:33:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Mon, 06 Jul 2020 23:33:57 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:34:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:34:21 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:34:29 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:34:31 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:34:32 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Mon, 06 Jul 2020 23:34:35 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Mon, 06 Jul 2020 23:34:48 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:34:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9139e63dbdf506429f6bb9a8559dd330a603e7b6ed4349cc7e5d0e384b034c`  
		Last Modified: Mon, 06 Jul 2020 23:36:35 GMT  
		Size: 113.2 MB (113221612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c5c66750ebbdcfa12195c7cd8891dff5cbb4f5bec172b8022890283de38e5c`  
		Last Modified: Mon, 06 Jul 2020 23:36:29 GMT  
		Size: 7.6 KB (7630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a171764f467afbee2a75fb679968cd7d8c4b9c3eed16d524a4569c3710be7`  
		Last Modified: Mon, 06 Jul 2020 23:36:27 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9`

```console
$ docker pull bonita@sha256:f687d563e20cb573aff8f7aac39f5616a9c5cec322471ae0501df30b6ad1e0db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9` - linux; amd64

```console
$ docker pull bonita@sha256:da5310be5eedc0dfa6b9234110669f814ef3fcb6c4aefdbb482d83180c4e06cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229215047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b69433509771a6384b6001ce7155a5ae5ee364623338edbb4b4d09bd14c1feca`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:30:51 GMT
ENV BONITA_VERSION=7.9.5
# Mon, 06 Jul 2020 23:30:51 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Mon, 06 Jul 2020 23:30:51 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Mon, 06 Jul 2020 23:30:59 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:31:00 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:31:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:02 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:02 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Mon, 06 Jul 2020 23:31:02 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:31:02 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf0559b59cf4e4b1b0ab87d14a11a177f009a6d53c059a61fe8a01bddffffff`  
		Last Modified: Mon, 06 Jul 2020 23:31:51 GMT  
		Size: 100.0 MB (100024958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fe929199e9f43e43d30480a9310552576cae0b5f52f4addfb903c9a1fdb64c`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f1c3893db7404931896030f979ed3148343baa6616805152a249e8956eb55`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ce90dd4da7b0cbbdd2726872ada27c36005088b451ba9bff024d7dadbc320662
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217222019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896e36877b518c9a79f598b901dd64c0090dd16ec3415c13ff4913449145fdc7`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:42:43 GMT
ARG BONITA_URL
# Wed, 17 Jun 2020 02:42:45 GMT
ENV BONITA_VERSION=7.9.5
# Wed, 17 Jun 2020 02:42:46 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Wed, 17 Jun 2020 02:42:48 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Wed, 17 Jun 2020 02:42:56 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 17 Jun 2020 02:42:59 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 17 Jun 2020 02:43:02 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Wed, 17 Jun 2020 02:43:03 GMT
VOLUME [/opt/bonita]
# Wed, 17 Jun 2020 02:43:04 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Wed, 17 Jun 2020 02:43:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 17 Jun 2020 02:43:06 GMT
EXPOSE 8080
# Wed, 17 Jun 2020 02:43:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9d6f808e1c6cb80145e13a9c836b06cb6335b2c7ec7216430ca8b40058ae64`  
		Last Modified: Wed, 17 Jun 2020 02:44:11 GMT  
		Size: 100.0 MB (100025000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a913ca2abfe76bed14e8b1e6ddafb3a4ff8b5f99b099bc3cd23157ff5b7d750`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67827ddc9dac11f17288052b212bdd665b4103a04efa7f80214cc439545f8b6c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; ppc64le

```console
$ docker pull bonita@sha256:1ec0ffcdf34fa9dbdd0831621e345551fa15cfb51c62b0b3e0a687be044b6be6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225878321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f59acc56e82be2476aaf90a86b8675423c3ac3c62ce907b32add7f51336f12cc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:29:30 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:29:33 GMT
ENV BONITA_VERSION=7.9.5
# Mon, 06 Jul 2020 23:29:34 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Mon, 06 Jul 2020 23:29:38 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Mon, 06 Jul 2020 23:30:35 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:30:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:30:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:30:55 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:30:57 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Mon, 06 Jul 2020 23:30:58 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:31:02 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:07 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12c4d67fe7fe0b4eb026a48d922e97f4d9a268516bc6d94eafe2c369d5a6ba8`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 100.0 MB (100025006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c2593d0935d285b0d956221cdb2e757686b28ae63750fee3d897870f2738df`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046a751eaf54400bd938b336f93f95e4fbaba066e5a2cced9028a04618da0e98`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9.5`

```console
$ docker pull bonita@sha256:f687d563e20cb573aff8f7aac39f5616a9c5cec322471ae0501df30b6ad1e0db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9.5` - linux; amd64

```console
$ docker pull bonita@sha256:da5310be5eedc0dfa6b9234110669f814ef3fcb6c4aefdbb482d83180c4e06cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229215047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b69433509771a6384b6001ce7155a5ae5ee364623338edbb4b4d09bd14c1feca`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:30:51 GMT
ENV BONITA_VERSION=7.9.5
# Mon, 06 Jul 2020 23:30:51 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Mon, 06 Jul 2020 23:30:51 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Mon, 06 Jul 2020 23:30:59 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:31:00 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:31:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:02 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:02 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Mon, 06 Jul 2020 23:31:02 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:31:02 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf0559b59cf4e4b1b0ab87d14a11a177f009a6d53c059a61fe8a01bddffffff`  
		Last Modified: Mon, 06 Jul 2020 23:31:51 GMT  
		Size: 100.0 MB (100024958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fe929199e9f43e43d30480a9310552576cae0b5f52f4addfb903c9a1fdb64c`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f1c3893db7404931896030f979ed3148343baa6616805152a249e8956eb55`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ce90dd4da7b0cbbdd2726872ada27c36005088b451ba9bff024d7dadbc320662
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217222019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896e36877b518c9a79f598b901dd64c0090dd16ec3415c13ff4913449145fdc7`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:42:43 GMT
ARG BONITA_URL
# Wed, 17 Jun 2020 02:42:45 GMT
ENV BONITA_VERSION=7.9.5
# Wed, 17 Jun 2020 02:42:46 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Wed, 17 Jun 2020 02:42:48 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Wed, 17 Jun 2020 02:42:56 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 17 Jun 2020 02:42:59 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 17 Jun 2020 02:43:02 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Wed, 17 Jun 2020 02:43:03 GMT
VOLUME [/opt/bonita]
# Wed, 17 Jun 2020 02:43:04 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Wed, 17 Jun 2020 02:43:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 17 Jun 2020 02:43:06 GMT
EXPOSE 8080
# Wed, 17 Jun 2020 02:43:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9d6f808e1c6cb80145e13a9c836b06cb6335b2c7ec7216430ca8b40058ae64`  
		Last Modified: Wed, 17 Jun 2020 02:44:11 GMT  
		Size: 100.0 MB (100025000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a913ca2abfe76bed14e8b1e6ddafb3a4ff8b5f99b099bc3cd23157ff5b7d750`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67827ddc9dac11f17288052b212bdd665b4103a04efa7f80214cc439545f8b6c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; ppc64le

```console
$ docker pull bonita@sha256:1ec0ffcdf34fa9dbdd0831621e345551fa15cfb51c62b0b3e0a687be044b6be6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225878321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f59acc56e82be2476aaf90a86b8675423c3ac3c62ce907b32add7f51336f12cc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:29:30 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:29:33 GMT
ENV BONITA_VERSION=7.9.5
# Mon, 06 Jul 2020 23:29:34 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Mon, 06 Jul 2020 23:29:38 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Mon, 06 Jul 2020 23:30:35 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:30:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Mon, 06 Jul 2020 23:30:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:30:55 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:30:57 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Mon, 06 Jul 2020 23:30:58 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Mon, 06 Jul 2020 23:31:02 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:07 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12c4d67fe7fe0b4eb026a48d922e97f4d9a268516bc6d94eafe2c369d5a6ba8`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 100.0 MB (100025006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c2593d0935d285b0d956221cdb2e757686b28ae63750fee3d897870f2738df`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046a751eaf54400bd938b336f93f95e4fbaba066e5a2cced9028a04618da0e98`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:6308fad666eb7e7172454a573194e470a3ee5cd0140386383c34c01d5c96db78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:a3edb90d54c87cbf5c2b1261eae54bee1d51a2bb5031d0a4095007b445c39eef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.4 MB (242411758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbd3922096b5c8ca88961188b6fd81ef214b805b99ac5c83ad3a01ff2269049e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:30:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:30:46 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:30:47 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:30:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:30:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:30:50 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:07 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:08 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:31:26 GMT
ENV BONITA_VERSION=7.11.0
# Mon, 06 Jul 2020 23:31:26 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Mon, 06 Jul 2020 23:31:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 06 Jul 2020 23:31:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Mon, 06 Jul 2020 23:31:27 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:31:30 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:31:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:31:34 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:31:34 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Mon, 06 Jul 2020 23:31:34 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Mon, 06 Jul 2020 23:31:34 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:31:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94530f848a439d944a125fa32a98a04112b3d546be2cbb7d4636cf3ff511e9f0`  
		Last Modified: Mon, 06 Jul 2020 23:32:01 GMT  
		Size: 101.9 MB (101873926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6add29569c3b322e4e8bbbd2138fd2c9cd23823dab87fed1d95520c7bb7a3`  
		Last Modified: Mon, 06 Jul 2020 23:31:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15d2fd6e088f03bb92ba188130dbcc952c0c891263de0007a6d9ef11ebfa8a8`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5342a7cef84fcec3b60bdfec50df557b2cc565d5d96cb1a16fb2418106c6`  
		Last Modified: Mon, 06 Jul 2020 23:31:44 GMT  
		Size: 572.4 KB (572377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bf9960435230d25d853029b722cbe0fa0e3952311e2e55e1224cba6663300d`  
		Last Modified: Mon, 06 Jul 2020 23:32:24 GMT  
		Size: 113.2 MB (113221577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bc491840b73f5b999f686279c9f60258d368198a2d6892c421624499d5767`  
		Last Modified: Mon, 06 Jul 2020 23:32:18 GMT  
		Size: 7.6 KB (7597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bebeec36e0817b89a37dd029791681652e61daba9cb1c38dadfa6c3bfc90f97`  
		Last Modified: Mon, 06 Jul 2020 23:32:19 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:65ba0e2092b7bafa8f4c812130451af1c212c08775aff508d87cd7e1cb9f83c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230418729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5464e79dfb5c4d44ac9d5c6408232297da9600beda3dac56079fc0d127efab8c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 17 Jun 2020 01:42:33 GMT
ADD file:7dc8819fd3d4b84ad19fb836e5bfda64a5ffefc371166f70d4d41dff6b22d450 in / 
# Wed, 17 Jun 2020 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:42:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:42:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:42:45 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 02:40:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 17 Jun 2020 02:42:25 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 02:42:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 17 Jun 2020 02:42:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 17 Jun 2020 02:42:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 17 Jun 2020 02:42:40 GMT
ARG BONITA_VERSION
# Wed, 17 Jun 2020 02:42:41 GMT
ARG BONITA_SHA256
# Wed, 17 Jun 2020 02:43:21 GMT
ARG BASE_URL
# Wed, 17 Jun 2020 02:43:22 GMT
ARG BONITA_URL
# Wed, 24 Jun 2020 17:40:14 GMT
ENV BONITA_VERSION=7.11.0
# Wed, 24 Jun 2020 17:40:15 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Wed, 24 Jun 2020 17:40:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 24 Jun 2020 17:40:16 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Wed, 24 Jun 2020 17:40:19 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 24 Jun 2020 17:40:28 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 24 Jun 2020 17:40:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 24 Jun 2020 17:40:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 24 Jun 2020 17:40:34 GMT
VOLUME [/opt/bonita]
# Fri, 03 Jul 2020 17:39:47 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Fri, 03 Jul 2020 17:39:48 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 03 Jul 2020 17:39:49 GMT
EXPOSE 8080
# Fri, 03 Jul 2020 17:39:49 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2e8bea8b22f8f5a4fd5aa85019945dd8ae04f283a4ba2a7aeb4536fe2f1d1ec2`  
		Last Modified: Tue, 26 May 2020 16:25:25 GMT  
		Size: 23.7 MB (23721687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90876b9c9a7343ae432eaec7c8dc8859c1e84b6193da8d386815fde165a70e`  
		Last Modified: Wed, 17 Jun 2020 01:44:48 GMT  
		Size: 35.2 KB (35192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bfc658a5210a9f0c9cfcda5f504e720da9268e9f3f3bf48e3a9a7af360c959`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef0f1b06b2142ff2bf35cc565f019ed9e4efe0d8f332825167538c2337bac8a`  
		Last Modified: Wed, 17 Jun 2020 01:44:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2e7783d3202312a68d1bae9863062d6bfcad302b838d982a971b6d1eace7cf`  
		Last Modified: Wed, 17 Jun 2020 02:44:30 GMT  
		Size: 92.9 MB (92885966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7449c9a39dcb1672a84ad09440887b1968c4c7f83d49fe0ecbfa775c89ca9`  
		Last Modified: Wed, 17 Jun 2020 02:44:04 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da90b862c2b844579dc9210fe78f9026d832b17f0b9d594f703d8dacf603d7`  
		Last Modified: Wed, 17 Jun 2020 02:44:03 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832035663682d494bbcc67a3f9e4927458156bf6e392d821d11d63f4c6532f3c`  
		Last Modified: Wed, 17 Jun 2020 02:44:02 GMT  
		Size: 541.8 KB (541818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee3b35a452661ddca4c2185aeaeaf603b1937d0b4115a8ed159e89b484d9029`  
		Last Modified: Wed, 24 Jun 2020 17:41:00 GMT  
		Size: 113.2 MB (113221612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3693802575293a0aece91313aedab1a4c96463acb5c399ab24bf64eda2e15e6c`  
		Last Modified: Fri, 03 Jul 2020 17:40:03 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1103b7a50b8f307fffc3657789584c32b8df6e7097dcbf8a21981b7bd1309e12`  
		Last Modified: Fri, 03 Jul 2020 17:40:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:abb6bf1f182f6660be47c25185a09eb26cfeabba37dd10fcbb67912d9dc43ed7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239075022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9b91e6a4d1f55558e53cda217ce77753552451fc11263166637ac7fa026f6e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:23:25 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Mon, 06 Jul 2020 23:28:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:28:52 GMT
RUN mkdir /opt/custom-init.d/
# Mon, 06 Jul 2020 23:29:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Mon, 06 Jul 2020 23:29:16 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Mon, 06 Jul 2020 23:29:19 GMT
ARG BONITA_VERSION
# Mon, 06 Jul 2020 23:29:26 GMT
ARG BONITA_SHA256
# Mon, 06 Jul 2020 23:31:29 GMT
ARG BASE_URL
# Mon, 06 Jul 2020 23:31:36 GMT
ARG BONITA_URL
# Mon, 06 Jul 2020 23:33:40 GMT
ENV BONITA_VERSION=7.11.0
# Mon, 06 Jul 2020 23:33:43 GMT
ENV BONITA_SHA256=f1d0d3c2f57c0d32ee068c1acd4e21fcf5c866d17fb097b1db97e663697dc8fe
# Mon, 06 Jul 2020 23:33:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Mon, 06 Jul 2020 23:33:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.0/BonitaCommunity-7.11.0.zip
# Mon, 06 Jul 2020 23:33:57 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Mon, 06 Jul 2020 23:34:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:34:21 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Mon, 06 Jul 2020 23:34:29 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Mon, 06 Jul 2020 23:34:31 GMT
VOLUME [/opt/bonita]
# Mon, 06 Jul 2020 23:34:32 GMT
COPY dir:7f0e6270bb2bea49c029cca8eb0e60f9f0c9c5d47fd807149e3e18c746693278 in /opt/files 
# Mon, 06 Jul 2020 23:34:35 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Mon, 06 Jul 2020 23:34:48 GMT
EXPOSE 8080
# Mon, 06 Jul 2020 23:34:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8337bd9f1f971e3b6108ec05ad68a63de1f0b5df1d722cf43d6917c6eca9f76`  
		Last Modified: Mon, 06 Jul 2020 23:35:52 GMT  
		Size: 94.9 MB (94860728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a039796f34ef8f2ac4461b1d85644e658e3b2dff526ec836744c59e968a2e010`  
		Last Modified: Mon, 06 Jul 2020 23:35:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab5eed2162a438efac2e003c564ce84a01711d3e4cd2fd341aa6415789c2a28`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 1.9 KB (1926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bcb01f35a2ed59cfce12942d3da8add2f0d5c4ab42e06bc16fe7d4526350f4`  
		Last Modified: Mon, 06 Jul 2020 23:35:22 GMT  
		Size: 541.5 KB (541541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9139e63dbdf506429f6bb9a8559dd330a603e7b6ed4349cc7e5d0e384b034c`  
		Last Modified: Mon, 06 Jul 2020 23:36:35 GMT  
		Size: 113.2 MB (113221612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c5c66750ebbdcfa12195c7cd8891dff5cbb4f5bec172b8022890283de38e5c`  
		Last Modified: Mon, 06 Jul 2020 23:36:29 GMT  
		Size: 7.6 KB (7630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649a171764f467afbee2a75fb679968cd7d8c4b9c3eed16d524a4569c3710be7`  
		Last Modified: Mon, 06 Jul 2020 23:36:27 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
