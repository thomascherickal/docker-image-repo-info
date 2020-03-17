<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.3`](#bonita7103)
-	[`bonita:7.9`](#bonita79)
-	[`bonita:7.9.5`](#bonita795)
-	[`bonita:latest`](#bonitalatest)

## `bonita:7.10`

```console
$ docker pull bonita@sha256:c92ec853ea88f691d7eabef95bb191b613fd0d524015300fe405d7aaebdc391f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:bdab350e52728f6fe88c6b50f602fe117b66abff218fcfa96e50701556041524
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227055382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:838dd4c3162e4a1352a5cf3f7e3b52398f87580bfe0211c801fd4dfd1cc6efb2`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:06:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:06:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:06:53 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:06:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:06:54 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:07:16 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 23:07:16 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:21:16 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:39:12 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:39:13 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:39:15 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:39:15 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:39:15 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:39:15 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:39:15 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:39:16 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aa4ad5c84ecc44619ed2214f0850dc54d8ed7f5aad1fec1f8e67b5f5f1d5e9`  
		Last Modified: Fri, 21 Feb 2020 23:07:56 GMT  
		Size: 101.8 MB (101838857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19491f92f5cc80d864566f330109d55c8bfec7ecf3f084bca0c95d0b474a7705`  
		Last Modified: Fri, 21 Feb 2020 23:07:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb24e07d4f834a79ae4fd59c6c201d4978541e6252275ef7456592f3344218`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e48474f73bf9c9827637f667be52a93e83fdb917dc5fe1b8646baba3648568`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2178d91a3b0a0b8f74901a74592d60cf235ae224f7a6246e8cbb02b85c9e1a`  
		Last Modified: Wed, 11 Mar 2020 22:39:34 GMT  
		Size: 97.9 MB (97904420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93acf4e6ef60c40d68ac1e8af76363a09ce4ce2814432ac792c1efc4e419e43`  
		Last Modified: Wed, 11 Mar 2020 22:39:33 GMT  
		Size: 7.6 KB (7596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deebf1fbf3a81c2fe3275e66c42ab6e75aa4e84afb7793039fc47f8b774bc4`  
		Last Modified: Wed, 11 Mar 2020 22:39:33 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:abcc2176f127924a4e3346f09b2d82e7b407a9003740c0f9acf319e32fa7c279
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.1 MB (215080141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09753e7c1faec78fd14566c676dce6d7f8219a78befbe4657538e3c982a2b71`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:21:36 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 22:22:27 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 22:22:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 22:22:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 22:22:35 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 22:23:22 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 22:23:23 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:40:47 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:40:47 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:40:48 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:40:48 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:40:50 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:40:59 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:41:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:41:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:41:05 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:41:06 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:41:06 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:41:07 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:41:07 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a57ca1a5a384e11e7a3aa5e40aa3503482c0501ae5e1e7a47570673379321b`  
		Last Modified: Fri, 21 Feb 2020 22:24:23 GMT  
		Size: 92.9 MB (92865144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9dfd9f9516993b9de00bb7a64b64feb61a28e04feb60125337c54fdedd5421`  
		Last Modified: Fri, 21 Feb 2020 22:23:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195a55d9606782f3d98bcc08f9cd186e5125bfdd3e0ea80b76417b51cf675ca`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6d58bc764dd3d807b31f0f44a36f30b4ad199ca4b2929ead5751a2f9ceb39`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 541.8 KB (541817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264a2d2e27332c75bb6c7f1501dc24c6cf345bc195efda6b40082cfb99b1673`  
		Last Modified: Wed, 11 Mar 2020 22:41:29 GMT  
		Size: 97.9 MB (97904455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146ce676556ce29522f600d27d85c3008f04ba49caecdf9d57d22d9e05019a2`  
		Last Modified: Wed, 11 Mar 2020 22:41:18 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38868ef7736e1c930926ea6bf2a3844b3330c59f43dc1c5adf832c99008248`  
		Last Modified: Wed, 11 Mar 2020 22:41:18 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:9d29d16e5cce34c7114bf0b39351c38010f83f4cb762d6b6bd44f782a55b9999
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223743685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1da1170486f51bb13af32276f82126748cdc95be2d1116fe427266803cd46c1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:52:14 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:56:54 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:57:07 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:57:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:57:26 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:57:29 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:57:34 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:59:16 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 23:59:19 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:16:52 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:16:54 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:16:58 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:17:01 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:17:10 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:18:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:18:21 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:18:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:18:37 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:18:38 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:18:39 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:18:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:18:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c97a42c6ae6969773b3fb23c130fa485f285866f5a6781f13bf8fb222b92291`  
		Last Modified: Sat, 22 Feb 2020 00:06:24 GMT  
		Size: 94.8 MB (94848995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006065fc2b6823e54391a74f82604a287864e78a3746a64d83be238c2292fbd8`  
		Last Modified: Sat, 22 Feb 2020 00:06:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bdd3a9195a76e3edeb5a35d0dbcb2bcd1a90445b040ef01c608b89883a8e03`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffbb92d963bd0cbeed187c546e92c556541d8a5873f24b6ec19a160517a6d02`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1225c2111b751ac0245694a1a90720b00b026ac4cb9ceef05bdcfefa4e7cd5`  
		Last Modified: Wed, 11 Mar 2020 22:19:13 GMT  
		Size: 97.9 MB (97904454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea8f33ed9a5e928d42371c0030e5e5698948356d1e9fd2857a2e9056778c07`  
		Last Modified: Wed, 11 Mar 2020 22:19:05 GMT  
		Size: 7.6 KB (7619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e09eba02e00204153a3b9190becef7c7593a6ec97daa0ecc012c0b066fa84f4`  
		Last Modified: Wed, 11 Mar 2020 22:19:05 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.3`

```console
$ docker pull bonita@sha256:c92ec853ea88f691d7eabef95bb191b613fd0d524015300fe405d7aaebdc391f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.3` - linux; amd64

```console
$ docker pull bonita@sha256:bdab350e52728f6fe88c6b50f602fe117b66abff218fcfa96e50701556041524
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227055382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:838dd4c3162e4a1352a5cf3f7e3b52398f87580bfe0211c801fd4dfd1cc6efb2`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:06:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:06:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:06:53 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:06:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:06:54 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:07:16 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 23:07:16 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:21:16 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:39:12 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:39:13 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:39:15 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:39:15 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:39:15 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:39:15 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:39:15 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:39:16 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aa4ad5c84ecc44619ed2214f0850dc54d8ed7f5aad1fec1f8e67b5f5f1d5e9`  
		Last Modified: Fri, 21 Feb 2020 23:07:56 GMT  
		Size: 101.8 MB (101838857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19491f92f5cc80d864566f330109d55c8bfec7ecf3f084bca0c95d0b474a7705`  
		Last Modified: Fri, 21 Feb 2020 23:07:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb24e07d4f834a79ae4fd59c6c201d4978541e6252275ef7456592f3344218`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e48474f73bf9c9827637f667be52a93e83fdb917dc5fe1b8646baba3648568`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2178d91a3b0a0b8f74901a74592d60cf235ae224f7a6246e8cbb02b85c9e1a`  
		Last Modified: Wed, 11 Mar 2020 22:39:34 GMT  
		Size: 97.9 MB (97904420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93acf4e6ef60c40d68ac1e8af76363a09ce4ce2814432ac792c1efc4e419e43`  
		Last Modified: Wed, 11 Mar 2020 22:39:33 GMT  
		Size: 7.6 KB (7596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deebf1fbf3a81c2fe3275e66c42ab6e75aa4e84afb7793039fc47f8b774bc4`  
		Last Modified: Wed, 11 Mar 2020 22:39:33 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.3` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:abcc2176f127924a4e3346f09b2d82e7b407a9003740c0f9acf319e32fa7c279
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.1 MB (215080141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09753e7c1faec78fd14566c676dce6d7f8219a78befbe4657538e3c982a2b71`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:21:36 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 22:22:27 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 22:22:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 22:22:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 22:22:35 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 22:23:22 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 22:23:23 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:40:47 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:40:47 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:40:48 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:40:48 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:40:50 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:40:59 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:41:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:41:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:41:05 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:41:06 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:41:06 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:41:07 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:41:07 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a57ca1a5a384e11e7a3aa5e40aa3503482c0501ae5e1e7a47570673379321b`  
		Last Modified: Fri, 21 Feb 2020 22:24:23 GMT  
		Size: 92.9 MB (92865144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9dfd9f9516993b9de00bb7a64b64feb61a28e04feb60125337c54fdedd5421`  
		Last Modified: Fri, 21 Feb 2020 22:23:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195a55d9606782f3d98bcc08f9cd186e5125bfdd3e0ea80b76417b51cf675ca`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6d58bc764dd3d807b31f0f44a36f30b4ad199ca4b2929ead5751a2f9ceb39`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 541.8 KB (541817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264a2d2e27332c75bb6c7f1501dc24c6cf345bc195efda6b40082cfb99b1673`  
		Last Modified: Wed, 11 Mar 2020 22:41:29 GMT  
		Size: 97.9 MB (97904455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146ce676556ce29522f600d27d85c3008f04ba49caecdf9d57d22d9e05019a2`  
		Last Modified: Wed, 11 Mar 2020 22:41:18 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38868ef7736e1c930926ea6bf2a3844b3330c59f43dc1c5adf832c99008248`  
		Last Modified: Wed, 11 Mar 2020 22:41:18 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.3` - linux; ppc64le

```console
$ docker pull bonita@sha256:9d29d16e5cce34c7114bf0b39351c38010f83f4cb762d6b6bd44f782a55b9999
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223743685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1da1170486f51bb13af32276f82126748cdc95be2d1116fe427266803cd46c1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:52:14 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:56:54 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:57:07 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:57:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:57:26 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:57:29 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:57:34 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:59:16 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 23:59:19 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:16:52 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:16:54 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:16:58 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:17:01 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:17:10 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:18:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:18:21 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:18:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:18:37 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:18:38 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:18:39 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:18:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:18:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c97a42c6ae6969773b3fb23c130fa485f285866f5a6781f13bf8fb222b92291`  
		Last Modified: Sat, 22 Feb 2020 00:06:24 GMT  
		Size: 94.8 MB (94848995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006065fc2b6823e54391a74f82604a287864e78a3746a64d83be238c2292fbd8`  
		Last Modified: Sat, 22 Feb 2020 00:06:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bdd3a9195a76e3edeb5a35d0dbcb2bcd1a90445b040ef01c608b89883a8e03`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffbb92d963bd0cbeed187c546e92c556541d8a5873f24b6ec19a160517a6d02`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1225c2111b751ac0245694a1a90720b00b026ac4cb9ceef05bdcfefa4e7cd5`  
		Last Modified: Wed, 11 Mar 2020 22:19:13 GMT  
		Size: 97.9 MB (97904454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea8f33ed9a5e928d42371c0030e5e5698948356d1e9fd2857a2e9056778c07`  
		Last Modified: Wed, 11 Mar 2020 22:19:05 GMT  
		Size: 7.6 KB (7619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e09eba02e00204153a3b9190becef7c7593a6ec97daa0ecc012c0b066fa84f4`  
		Last Modified: Wed, 11 Mar 2020 22:19:05 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9`

```console
$ docker pull bonita@sha256:511edc512b02f78282baeb38f7eb87a166a927b342c7159a7bc890c98d947241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9` - linux; amd64

```console
$ docker pull bonita@sha256:d4067a46515819753c4162127034d19074cae074710aefb0a7723550a2b9f118
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229175877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6a5835d19adef2e2607e3a459798426c4dfffd0ddf7a4e7ec84ecafeb012ca`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:06:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:06:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:06:53 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:06:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:06:54 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_URL
# Tue, 17 Mar 2020 02:19:20 GMT
ENV BONITA_VERSION=7.9.5
# Tue, 17 Mar 2020 02:19:20 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Tue, 17 Mar 2020 02:19:21 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Tue, 17 Mar 2020 02:19:29 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Tue, 17 Mar 2020 02:19:34 GMT
VOLUME [/opt/bonita]
# Tue, 17 Mar 2020 02:19:34 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Tue, 17 Mar 2020 02:19:35 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 17 Mar 2020 02:19:35 GMT
EXPOSE 8080
# Tue, 17 Mar 2020 02:19:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aa4ad5c84ecc44619ed2214f0850dc54d8ed7f5aad1fec1f8e67b5f5f1d5e9`  
		Last Modified: Fri, 21 Feb 2020 23:07:56 GMT  
		Size: 101.8 MB (101838857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19491f92f5cc80d864566f330109d55c8bfec7ecf3f084bca0c95d0b474a7705`  
		Last Modified: Fri, 21 Feb 2020 23:07:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb24e07d4f834a79ae4fd59c6c201d4978541e6252275ef7456592f3344218`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e48474f73bf9c9827637f667be52a93e83fdb917dc5fe1b8646baba3648568`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29027362147473dfec592fd307ea4acf936a92db38a3355d6d76c77b4a36a05`  
		Last Modified: Tue, 17 Mar 2020 02:19:58 GMT  
		Size: 100.0 MB (100024960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae05876741ee2ab4a0946e113e1f750ff792da251232bc4ea45e89c12d2ae80`  
		Last Modified: Tue, 17 Mar 2020 02:19:52 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efc257c80415e3ead74bb77b0d62471a4d6bad62260865546637cff7cefa053`  
		Last Modified: Tue, 17 Mar 2020 02:19:51 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:0089bdeef94e681414ff86e077e6ea114d4049e4a64178f0e68dbfeb3bb1d203
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217200654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f4fd8214e457ab898550361e964d8c2b688331a0e5fc8d4b942663254ea129e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:21:36 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 22:22:27 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 22:22:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 22:22:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 22:22:35 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_URL
# Tue, 17 Mar 2020 01:43:18 GMT
ENV BONITA_VERSION=7.9.5
# Tue, 17 Mar 2020 01:43:18 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Tue, 17 Mar 2020 01:43:19 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Tue, 17 Mar 2020 01:43:33 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 01:43:36 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 01:43:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Tue, 17 Mar 2020 01:43:39 GMT
VOLUME [/opt/bonita]
# Tue, 17 Mar 2020 01:43:39 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Tue, 17 Mar 2020 01:43:40 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 17 Mar 2020 01:43:40 GMT
EXPOSE 8080
# Tue, 17 Mar 2020 01:43:41 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a57ca1a5a384e11e7a3aa5e40aa3503482c0501ae5e1e7a47570673379321b`  
		Last Modified: Fri, 21 Feb 2020 22:24:23 GMT  
		Size: 92.9 MB (92865144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9dfd9f9516993b9de00bb7a64b64feb61a28e04feb60125337c54fdedd5421`  
		Last Modified: Fri, 21 Feb 2020 22:23:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195a55d9606782f3d98bcc08f9cd186e5125bfdd3e0ea80b76417b51cf675ca`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6d58bc764dd3d807b31f0f44a36f30b4ad199ca4b2929ead5751a2f9ceb39`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 541.8 KB (541817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2945222e1f617ddfbbf24adba31084f81f6081af9fc43175fb99f3ee93682cbb`  
		Last Modified: Tue, 17 Mar 2020 01:44:06 GMT  
		Size: 100.0 MB (100025000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfcddf4b95de827391a8692caafd29f2a46ccded2b267e670444024ce9d4266`  
		Last Modified: Tue, 17 Mar 2020 01:43:56 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a364af6c43105138e10ca1bc1d198f2a1ea8ac5370cf142a04cde5c7df805d`  
		Last Modified: Tue, 17 Mar 2020 01:43:55 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; ppc64le

```console
$ docker pull bonita@sha256:3a137862015f1289eee14ccfc738a4808390dabfd9dd0bc39890ab4b48a23f35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225864189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e03903b33c54ee8278ff527a73b60f91dab6695a5787d2049f3c8ab84eb652`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:52:14 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:56:54 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:57:07 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:57:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:57:26 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:57:29 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:57:34 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:57:37 GMT
ARG BONITA_URL
# Tue, 17 Mar 2020 02:16:38 GMT
ENV BONITA_VERSION=7.9.5
# Tue, 17 Mar 2020 02:16:53 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Tue, 17 Mar 2020 02:17:15 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Tue, 17 Mar 2020 02:18:51 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:04 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Tue, 17 Mar 2020 02:19:16 GMT
VOLUME [/opt/bonita]
# Tue, 17 Mar 2020 02:19:17 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Tue, 17 Mar 2020 02:19:19 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 17 Mar 2020 02:19:22 GMT
EXPOSE 8080
# Tue, 17 Mar 2020 02:19:24 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c97a42c6ae6969773b3fb23c130fa485f285866f5a6781f13bf8fb222b92291`  
		Last Modified: Sat, 22 Feb 2020 00:06:24 GMT  
		Size: 94.8 MB (94848995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006065fc2b6823e54391a74f82604a287864e78a3746a64d83be238c2292fbd8`  
		Last Modified: Sat, 22 Feb 2020 00:06:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bdd3a9195a76e3edeb5a35d0dbcb2bcd1a90445b040ef01c608b89883a8e03`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffbb92d963bd0cbeed187c546e92c556541d8a5873f24b6ec19a160517a6d02`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed91658e4141241336ebe7aa686cd1e9b30e6a66b97631f80048a219b9f9f2ef`  
		Last Modified: Tue, 17 Mar 2020 02:19:50 GMT  
		Size: 100.0 MB (100024999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41b9e85a85d405e9a4ec9a36b432b4e956ec583954265499baffde6ddb4292`  
		Last Modified: Tue, 17 Mar 2020 02:19:41 GMT  
		Size: 7.6 KB (7582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62232ddd995d519a3a7983bfc33fa0df266720d86261352180276a007d7763f1`  
		Last Modified: Tue, 17 Mar 2020 02:19:40 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9.5`

```console
$ docker pull bonita@sha256:511edc512b02f78282baeb38f7eb87a166a927b342c7159a7bc890c98d947241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9.5` - linux; amd64

```console
$ docker pull bonita@sha256:d4067a46515819753c4162127034d19074cae074710aefb0a7723550a2b9f118
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229175877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6a5835d19adef2e2607e3a459798426c4dfffd0ddf7a4e7ec84ecafeb012ca`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:06:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:06:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:06:53 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:06:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:06:54 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_URL
# Tue, 17 Mar 2020 02:19:20 GMT
ENV BONITA_VERSION=7.9.5
# Tue, 17 Mar 2020 02:19:20 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Tue, 17 Mar 2020 02:19:21 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Tue, 17 Mar 2020 02:19:29 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Tue, 17 Mar 2020 02:19:34 GMT
VOLUME [/opt/bonita]
# Tue, 17 Mar 2020 02:19:34 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Tue, 17 Mar 2020 02:19:35 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 17 Mar 2020 02:19:35 GMT
EXPOSE 8080
# Tue, 17 Mar 2020 02:19:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aa4ad5c84ecc44619ed2214f0850dc54d8ed7f5aad1fec1f8e67b5f5f1d5e9`  
		Last Modified: Fri, 21 Feb 2020 23:07:56 GMT  
		Size: 101.8 MB (101838857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19491f92f5cc80d864566f330109d55c8bfec7ecf3f084bca0c95d0b474a7705`  
		Last Modified: Fri, 21 Feb 2020 23:07:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb24e07d4f834a79ae4fd59c6c201d4978541e6252275ef7456592f3344218`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e48474f73bf9c9827637f667be52a93e83fdb917dc5fe1b8646baba3648568`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29027362147473dfec592fd307ea4acf936a92db38a3355d6d76c77b4a36a05`  
		Last Modified: Tue, 17 Mar 2020 02:19:58 GMT  
		Size: 100.0 MB (100024960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae05876741ee2ab4a0946e113e1f750ff792da251232bc4ea45e89c12d2ae80`  
		Last Modified: Tue, 17 Mar 2020 02:19:52 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efc257c80415e3ead74bb77b0d62471a4d6bad62260865546637cff7cefa053`  
		Last Modified: Tue, 17 Mar 2020 02:19:51 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:0089bdeef94e681414ff86e077e6ea114d4049e4a64178f0e68dbfeb3bb1d203
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217200654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f4fd8214e457ab898550361e964d8c2b688331a0e5fc8d4b942663254ea129e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:21:36 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 22:22:27 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 22:22:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 22:22:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 22:22:35 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_URL
# Tue, 17 Mar 2020 01:43:18 GMT
ENV BONITA_VERSION=7.9.5
# Tue, 17 Mar 2020 01:43:18 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Tue, 17 Mar 2020 01:43:19 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Tue, 17 Mar 2020 01:43:33 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 01:43:36 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 01:43:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Tue, 17 Mar 2020 01:43:39 GMT
VOLUME [/opt/bonita]
# Tue, 17 Mar 2020 01:43:39 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Tue, 17 Mar 2020 01:43:40 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 17 Mar 2020 01:43:40 GMT
EXPOSE 8080
# Tue, 17 Mar 2020 01:43:41 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a57ca1a5a384e11e7a3aa5e40aa3503482c0501ae5e1e7a47570673379321b`  
		Last Modified: Fri, 21 Feb 2020 22:24:23 GMT  
		Size: 92.9 MB (92865144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9dfd9f9516993b9de00bb7a64b64feb61a28e04feb60125337c54fdedd5421`  
		Last Modified: Fri, 21 Feb 2020 22:23:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195a55d9606782f3d98bcc08f9cd186e5125bfdd3e0ea80b76417b51cf675ca`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6d58bc764dd3d807b31f0f44a36f30b4ad199ca4b2929ead5751a2f9ceb39`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 541.8 KB (541817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2945222e1f617ddfbbf24adba31084f81f6081af9fc43175fb99f3ee93682cbb`  
		Last Modified: Tue, 17 Mar 2020 01:44:06 GMT  
		Size: 100.0 MB (100025000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfcddf4b95de827391a8692caafd29f2a46ccded2b267e670444024ce9d4266`  
		Last Modified: Tue, 17 Mar 2020 01:43:56 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a364af6c43105138e10ca1bc1d198f2a1ea8ac5370cf142a04cde5c7df805d`  
		Last Modified: Tue, 17 Mar 2020 01:43:55 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; ppc64le

```console
$ docker pull bonita@sha256:3a137862015f1289eee14ccfc738a4808390dabfd9dd0bc39890ab4b48a23f35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225864189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e03903b33c54ee8278ff527a73b60f91dab6695a5787d2049f3c8ab84eb652`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:52:14 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:56:54 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:57:07 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:57:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:57:26 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:57:29 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:57:34 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:57:37 GMT
ARG BONITA_URL
# Tue, 17 Mar 2020 02:16:38 GMT
ENV BONITA_VERSION=7.9.5
# Tue, 17 Mar 2020 02:16:53 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Tue, 17 Mar 2020 02:17:15 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Tue, 17 Mar 2020 02:18:51 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:04 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Tue, 17 Mar 2020 02:19:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Tue, 17 Mar 2020 02:19:16 GMT
VOLUME [/opt/bonita]
# Tue, 17 Mar 2020 02:19:17 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Tue, 17 Mar 2020 02:19:19 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 17 Mar 2020 02:19:22 GMT
EXPOSE 8080
# Tue, 17 Mar 2020 02:19:24 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c97a42c6ae6969773b3fb23c130fa485f285866f5a6781f13bf8fb222b92291`  
		Last Modified: Sat, 22 Feb 2020 00:06:24 GMT  
		Size: 94.8 MB (94848995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006065fc2b6823e54391a74f82604a287864e78a3746a64d83be238c2292fbd8`  
		Last Modified: Sat, 22 Feb 2020 00:06:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bdd3a9195a76e3edeb5a35d0dbcb2bcd1a90445b040ef01c608b89883a8e03`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffbb92d963bd0cbeed187c546e92c556541d8a5873f24b6ec19a160517a6d02`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed91658e4141241336ebe7aa686cd1e9b30e6a66b97631f80048a219b9f9f2ef`  
		Last Modified: Tue, 17 Mar 2020 02:19:50 GMT  
		Size: 100.0 MB (100024999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41b9e85a85d405e9a4ec9a36b432b4e956ec583954265499baffde6ddb4292`  
		Last Modified: Tue, 17 Mar 2020 02:19:41 GMT  
		Size: 7.6 KB (7582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62232ddd995d519a3a7983bfc33fa0df266720d86261352180276a007d7763f1`  
		Last Modified: Tue, 17 Mar 2020 02:19:40 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:c92ec853ea88f691d7eabef95bb191b613fd0d524015300fe405d7aaebdc391f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:bdab350e52728f6fe88c6b50f602fe117b66abff218fcfa96e50701556041524
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227055382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:838dd4c3162e4a1352a5cf3f7e3b52398f87580bfe0211c801fd4dfd1cc6efb2`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:06:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:06:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:06:53 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:06:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:06:54 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:06:55 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:07:16 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 23:07:16 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:21:15 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:21:16 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:39:12 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:39:13 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:39:15 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:39:15 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:39:15 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:39:15 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:39:15 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:39:16 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aa4ad5c84ecc44619ed2214f0850dc54d8ed7f5aad1fec1f8e67b5f5f1d5e9`  
		Last Modified: Fri, 21 Feb 2020 23:07:56 GMT  
		Size: 101.8 MB (101838857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19491f92f5cc80d864566f330109d55c8bfec7ecf3f084bca0c95d0b474a7705`  
		Last Modified: Fri, 21 Feb 2020 23:07:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb24e07d4f834a79ae4fd59c6c201d4978541e6252275ef7456592f3344218`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e48474f73bf9c9827637f667be52a93e83fdb917dc5fe1b8646baba3648568`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2178d91a3b0a0b8f74901a74592d60cf235ae224f7a6246e8cbb02b85c9e1a`  
		Last Modified: Wed, 11 Mar 2020 22:39:34 GMT  
		Size: 97.9 MB (97904420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93acf4e6ef60c40d68ac1e8af76363a09ce4ce2814432ac792c1efc4e419e43`  
		Last Modified: Wed, 11 Mar 2020 22:39:33 GMT  
		Size: 7.6 KB (7596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deebf1fbf3a81c2fe3275e66c42ab6e75aa4e84afb7793039fc47f8b774bc4`  
		Last Modified: Wed, 11 Mar 2020 22:39:33 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:abcc2176f127924a4e3346f09b2d82e7b407a9003740c0f9acf319e32fa7c279
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.1 MB (215080141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09753e7c1faec78fd14566c676dce6d7f8219a78befbe4657538e3c982a2b71`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:21:36 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 22:22:27 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 22:22:32 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 22:22:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 22:22:35 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 22:22:36 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 22:23:22 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 22:23:23 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:40:47 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:40:47 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:40:48 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:40:48 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:40:50 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:40:59 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:41:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:41:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:41:05 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:41:06 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:41:06 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:41:07 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:41:07 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a57ca1a5a384e11e7a3aa5e40aa3503482c0501ae5e1e7a47570673379321b`  
		Last Modified: Fri, 21 Feb 2020 22:24:23 GMT  
		Size: 92.9 MB (92865144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9dfd9f9516993b9de00bb7a64b64feb61a28e04feb60125337c54fdedd5421`  
		Last Modified: Fri, 21 Feb 2020 22:23:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8195a55d9606782f3d98bcc08f9cd186e5125bfdd3e0ea80b76417b51cf675ca`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6d58bc764dd3d807b31f0f44a36f30b4ad199ca4b2929ead5751a2f9ceb39`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 541.8 KB (541817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5264a2d2e27332c75bb6c7f1501dc24c6cf345bc195efda6b40082cfb99b1673`  
		Last Modified: Wed, 11 Mar 2020 22:41:29 GMT  
		Size: 97.9 MB (97904455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146ce676556ce29522f600d27d85c3008f04ba49caecdf9d57d22d9e05019a2`  
		Last Modified: Wed, 11 Mar 2020 22:41:18 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38868ef7736e1c930926ea6bf2a3844b3330c59f43dc1c5adf832c99008248`  
		Last Modified: Wed, 11 Mar 2020 22:41:18 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:9d29d16e5cce34c7114bf0b39351c38010f83f4cb762d6b6bd44f782a55b9999
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223743685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1da1170486f51bb13af32276f82126748cdc95be2d1116fe427266803cd46c1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:52:14 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 21 Feb 2020 23:56:54 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:57:07 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 21 Feb 2020 23:57:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 21 Feb 2020 23:57:26 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 21 Feb 2020 23:57:29 GMT
ARG BONITA_VERSION
# Fri, 21 Feb 2020 23:57:34 GMT
ARG BONITA_SHA256
# Fri, 21 Feb 2020 23:59:16 GMT
ARG BASE_URL
# Fri, 21 Feb 2020 23:59:19 GMT
ARG BONITA_URL
# Wed, 11 Mar 2020 22:16:52 GMT
ENV BONITA_VERSION=7.10.3
# Wed, 11 Mar 2020 22:16:54 GMT
ENV BONITA_SHA256=e6789736e97f10c9ca0ccbbe15f6977708edaed724ec81b69f5d66ce5dbee850
# Wed, 11 Mar 2020 22:16:58 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 11 Mar 2020 22:17:01 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.3.zip
# Wed, 11 Mar 2020 22:17:10 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 11 Mar 2020 22:18:10 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:18:21 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 11 Mar 2020 22:18:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 11 Mar 2020 22:18:37 GMT
VOLUME [/opt/bonita]
# Wed, 11 Mar 2020 22:18:38 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 11 Mar 2020 22:18:39 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 11 Mar 2020 22:18:42 GMT
EXPOSE 8080
# Wed, 11 Mar 2020 22:18:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c97a42c6ae6969773b3fb23c130fa485f285866f5a6781f13bf8fb222b92291`  
		Last Modified: Sat, 22 Feb 2020 00:06:24 GMT  
		Size: 94.8 MB (94848995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006065fc2b6823e54391a74f82604a287864e78a3746a64d83be238c2292fbd8`  
		Last Modified: Sat, 22 Feb 2020 00:06:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bdd3a9195a76e3edeb5a35d0dbcb2bcd1a90445b040ef01c608b89883a8e03`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffbb92d963bd0cbeed187c546e92c556541d8a5873f24b6ec19a160517a6d02`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1225c2111b751ac0245694a1a90720b00b026ac4cb9ceef05bdcfefa4e7cd5`  
		Last Modified: Wed, 11 Mar 2020 22:19:13 GMT  
		Size: 97.9 MB (97904454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea8f33ed9a5e928d42371c0030e5e5698948356d1e9fd2857a2e9056778c07`  
		Last Modified: Wed, 11 Mar 2020 22:19:05 GMT  
		Size: 7.6 KB (7619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e09eba02e00204153a3b9190becef7c7593a6ec97daa0ecc012c0b066fa84f4`  
		Last Modified: Wed, 11 Mar 2020 22:19:05 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
