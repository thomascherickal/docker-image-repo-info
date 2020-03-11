<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.3`](#bonita7103)
-	[`bonita:7.9`](#bonita79)
-	[`bonita:7.9.4`](#bonita794)
-	[`bonita:latest`](#bonitalatest)

## `bonita:7.10`

```console
$ docker pull bonita@sha256:9b758724038a2f45eb3d330d61c847d749c5efbec301ed883f094581fb7b2695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:eb370c66870c0a9b40891ff80e7077c7e3bfc8f4c351d15f68655f9c0801a7eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227043002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70a75148dcd05612ebad832452f6ad148c0bb48d11518dec2948c0c27952f98`
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
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BONITA_VERSION=7.10.1
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Fri, 21 Feb 2020 23:07:18 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 21 Feb 2020 23:07:25 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 23:07:27 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 23:07:28 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 21 Feb 2020 23:07:28 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 23:07:28 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 21 Feb 2020 23:07:29 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 23:07:29 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 23:07:29 GMT
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
	-	`sha256:dd7ef1247c84892dae32e625aebe2424c5d5062d541030162612cf42aabf6183`  
		Last Modified: Fri, 21 Feb 2020 23:08:05 GMT  
		Size: 97.9 MB (97892043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b588537119b781c8e1cd9616a8d91dd409aebde5288fc7ad5cd13d00d178ba`  
		Last Modified: Fri, 21 Feb 2020 23:08:00 GMT  
		Size: 7.6 KB (7593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c845c46aab921783562beea56f3b8d97232e8ebf6f45e27e0c814fe5156edc3`  
		Last Modified: Fri, 21 Feb 2020 23:08:00 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:072894a03f11ec6c58fc4ad34edc6a7bec7b28ec43a748d284e407f47630cd39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.1 MB (215067747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d3d105d191ad7a62321480c529852d331d025c12aac832fdcb23fced63aaf0`
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
# Fri, 21 Feb 2020 22:23:24 GMT
ENV BONITA_VERSION=7.10.1
# Fri, 21 Feb 2020 22:23:25 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Fri, 21 Feb 2020 22:23:26 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 21 Feb 2020 22:23:26 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Fri, 21 Feb 2020 22:23:29 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 21 Feb 2020 22:23:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 22:23:38 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 22:23:40 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 21 Feb 2020 22:23:41 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 22:23:41 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 21 Feb 2020 22:23:42 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 22:23:43 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 22:23:44 GMT
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
	-	`sha256:19933018f0b6da42a37134a1aad3a71b6327a2c7bf0ac2dda546ea7a6550cd5c`  
		Last Modified: Fri, 21 Feb 2020 22:24:42 GMT  
		Size: 97.9 MB (97892067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a70958b14b134e50fe58d6202b217c1710f4abd88f585bb729f94889b66ba95`  
		Last Modified: Fri, 21 Feb 2020 22:24:29 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67871a8f5dd1dda50ccc06bd0fac5b8b1a6110f7abc76b2ba422de3085b0b377`  
		Last Modified: Fri, 21 Feb 2020 22:24:30 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:8fd93a53631e540fe3535aaa60fd0e226f5e2805e3efbb075ef6731aa75cbc9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223731313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4681c645cd8f36db6223773755d0222b4f194c9cb6e7b32a6d0b6105f3756558`
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
# Fri, 21 Feb 2020 23:59:25 GMT
ENV BONITA_VERSION=7.10.1
# Fri, 21 Feb 2020 23:59:34 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Fri, 21 Feb 2020 23:59:39 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 21 Feb 2020 23:59:49 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Sat, 22 Feb 2020 00:00:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Sat, 22 Feb 2020 00:05:08 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Sat, 22 Feb 2020 00:05:17 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Sat, 22 Feb 2020 00:05:25 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Sat, 22 Feb 2020 00:05:28 GMT
VOLUME [/opt/bonita]
# Sat, 22 Feb 2020 00:05:29 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Sat, 22 Feb 2020 00:05:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Sat, 22 Feb 2020 00:05:38 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:05:40 GMT
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
	-	`sha256:381df29b7e14a6a4aebb50736b0951825c6bd6225da98332e03c2091d8f054d8`  
		Last Modified: Sat, 22 Feb 2020 00:06:44 GMT  
		Size: 97.9 MB (97892074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f9546ffd71b0bc9e136773f7c52eebfa65578ee82dbb71cab13ec73134acb`  
		Last Modified: Sat, 22 Feb 2020 00:06:36 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bcd92479045aa95229df017a3bec1fe328257a30c96a5a3b7e6e02b4d3026f`  
		Last Modified: Sat, 22 Feb 2020 00:06:37 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.3`

**does not exist** (yet?)

## `bonita:7.9`

```console
$ docker pull bonita@sha256:db24c25b93deeda9a665eaea3a6cb4ccc4faeebd5ad975b03d14bd0bf6001809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9` - linux; amd64

```console
$ docker pull bonita@sha256:85cf4b51dbc57088ea3e5f7ec01064a904a47bbf9db81176e583c5409cdb6d7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229177166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fecadea35b61a1ebdd19c79ac7ccdf838be194db01a693dc59aaf8bbd0253b`
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
# Fri, 21 Feb 2020 23:06:55 GMT
ENV BONITA_VERSION=7.9.4
# Fri, 21 Feb 2020 23:06:55 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Fri, 21 Feb 2020 23:06:56 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Fri, 21 Feb 2020 23:07:04 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:07:05 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:07:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 21 Feb 2020 23:07:07 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 23:07:07 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 21 Feb 2020 23:07:07 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 23:07:07 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 23:07:08 GMT
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
	-	`sha256:6916720d7f1298f09de63b27864c70026b779a050980cd0d8ceb77f3f4c90ee9`  
		Last Modified: Fri, 21 Feb 2020 23:07:44 GMT  
		Size: 100.0 MB (100026245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1534a08c7e813fab842aa620b3d43c4211d448a1b7610c8b7a20ea02f5bade0`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e37a012bb58c80e9232827253205f6271647841d6f7222c6c5fbc645ac2e11`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.6 KB (1625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:57e52c93bbb564c7d75975adb58dddb9ba1ac0fca445d9e8217bbc67da25a5d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217201924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:292d11dc8e6b953fbf6949f45b25ff530a699944a1629d4279a675603cac662a`
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
# Fri, 21 Feb 2020 22:22:37 GMT
ENV BONITA_VERSION=7.9.4
# Fri, 21 Feb 2020 22:22:37 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Fri, 21 Feb 2020 22:22:38 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Fri, 21 Feb 2020 22:22:52 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 22:22:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 22:22:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 21 Feb 2020 22:23:00 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 22:23:00 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 21 Feb 2020 22:23:01 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 22:23:02 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 22:23:02 GMT
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
	-	`sha256:44de7cc08c0376f83c8d32aa2a5888b5e4949da5164a30bd7213c75fb252c02f`  
		Last Modified: Fri, 21 Feb 2020 22:24:07 GMT  
		Size: 100.0 MB (100026270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc5ef2720f714eb76fc606bda5d2dd293f35e20fc467a82c79bfc46149c4d06`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec07986804bcb1b8d56956bf690abcef22692ba11d00c951d183375f50602157`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.7 KB (1658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; ppc64le

```console
$ docker pull bonita@sha256:50f2ece5d11435b4fe1bd4d7c30309eb337d709993fa4fe101ef75ad118e3e57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225865473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af9589ab8e640c693f620224801841999367afbd53f3b06cba4237555ff8e6`
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
# Fri, 21 Feb 2020 23:57:41 GMT
ENV BONITA_VERSION=7.9.4
# Fri, 21 Feb 2020 23:57:42 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Fri, 21 Feb 2020 23:57:45 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Fri, 21 Feb 2020 23:58:39 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:58:46 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:58:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 21 Feb 2020 23:58:55 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 23:58:56 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 21 Feb 2020 23:58:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 23:59:01 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 23:59:04 GMT
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
	-	`sha256:6300e239ddacf098f907719ff2fc3fe8fe214663071c117fb4a3b2601b2d7bf3`  
		Last Modified: Sat, 22 Feb 2020 00:06:10 GMT  
		Size: 100.0 MB (100026273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a0723cf0060d4d254c070c4013cd595a31771532bf0f92c034e0d1b66857ae`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba25589781e4254bd63978f7579cacf7e482b8b3d0d5285b49c705bb8d9ce1`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9.4`

```console
$ docker pull bonita@sha256:db24c25b93deeda9a665eaea3a6cb4ccc4faeebd5ad975b03d14bd0bf6001809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9.4` - linux; amd64

```console
$ docker pull bonita@sha256:85cf4b51dbc57088ea3e5f7ec01064a904a47bbf9db81176e583c5409cdb6d7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229177166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fecadea35b61a1ebdd19c79ac7ccdf838be194db01a693dc59aaf8bbd0253b`
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
# Fri, 21 Feb 2020 23:06:55 GMT
ENV BONITA_VERSION=7.9.4
# Fri, 21 Feb 2020 23:06:55 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Fri, 21 Feb 2020 23:06:56 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Fri, 21 Feb 2020 23:07:04 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:07:05 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:07:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 21 Feb 2020 23:07:07 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 23:07:07 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 21 Feb 2020 23:07:07 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 23:07:07 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 23:07:08 GMT
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
	-	`sha256:6916720d7f1298f09de63b27864c70026b779a050980cd0d8ceb77f3f4c90ee9`  
		Last Modified: Fri, 21 Feb 2020 23:07:44 GMT  
		Size: 100.0 MB (100026245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1534a08c7e813fab842aa620b3d43c4211d448a1b7610c8b7a20ea02f5bade0`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e37a012bb58c80e9232827253205f6271647841d6f7222c6c5fbc645ac2e11`  
		Last Modified: Fri, 21 Feb 2020 23:07:38 GMT  
		Size: 1.6 KB (1625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:57e52c93bbb564c7d75975adb58dddb9ba1ac0fca445d9e8217bbc67da25a5d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217201924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:292d11dc8e6b953fbf6949f45b25ff530a699944a1629d4279a675603cac662a`
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
# Fri, 21 Feb 2020 22:22:37 GMT
ENV BONITA_VERSION=7.9.4
# Fri, 21 Feb 2020 22:22:37 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Fri, 21 Feb 2020 22:22:38 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Fri, 21 Feb 2020 22:22:52 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 22:22:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 22:22:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 21 Feb 2020 22:23:00 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 22:23:00 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 21 Feb 2020 22:23:01 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 22:23:02 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 22:23:02 GMT
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
	-	`sha256:44de7cc08c0376f83c8d32aa2a5888b5e4949da5164a30bd7213c75fb252c02f`  
		Last Modified: Fri, 21 Feb 2020 22:24:07 GMT  
		Size: 100.0 MB (100026270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc5ef2720f714eb76fc606bda5d2dd293f35e20fc467a82c79bfc46149c4d06`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec07986804bcb1b8d56956bf690abcef22692ba11d00c951d183375f50602157`  
		Last Modified: Fri, 21 Feb 2020 22:23:57 GMT  
		Size: 1.7 KB (1658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:50f2ece5d11435b4fe1bd4d7c30309eb337d709993fa4fe101ef75ad118e3e57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225865473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af9589ab8e640c693f620224801841999367afbd53f3b06cba4237555ff8e6`
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
# Fri, 21 Feb 2020 23:57:41 GMT
ENV BONITA_VERSION=7.9.4
# Fri, 21 Feb 2020 23:57:42 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Fri, 21 Feb 2020 23:57:45 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Fri, 21 Feb 2020 23:58:39 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:58:46 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 21 Feb 2020 23:58:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 21 Feb 2020 23:58:55 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 23:58:56 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 21 Feb 2020 23:58:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 23:59:01 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 23:59:04 GMT
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
	-	`sha256:6300e239ddacf098f907719ff2fc3fe8fe214663071c117fb4a3b2601b2d7bf3`  
		Last Modified: Sat, 22 Feb 2020 00:06:10 GMT  
		Size: 100.0 MB (100026273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a0723cf0060d4d254c070c4013cd595a31771532bf0f92c034e0d1b66857ae`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ba25589781e4254bd63978f7579cacf7e482b8b3d0d5285b49c705bb8d9ce1`  
		Last Modified: Sat, 22 Feb 2020 00:06:02 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:9b758724038a2f45eb3d330d61c847d749c5efbec301ed883f094581fb7b2695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:eb370c66870c0a9b40891ff80e7077c7e3bfc8f4c351d15f68655f9c0801a7eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227043002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70a75148dcd05612ebad832452f6ad148c0bb48d11518dec2948c0c27952f98`
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
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BONITA_VERSION=7.10.1
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 21 Feb 2020 23:07:17 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Fri, 21 Feb 2020 23:07:18 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 21 Feb 2020 23:07:25 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 23:07:27 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 23:07:28 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 21 Feb 2020 23:07:28 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 23:07:28 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 21 Feb 2020 23:07:29 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 23:07:29 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 23:07:29 GMT
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
	-	`sha256:dd7ef1247c84892dae32e625aebe2424c5d5062d541030162612cf42aabf6183`  
		Last Modified: Fri, 21 Feb 2020 23:08:05 GMT  
		Size: 97.9 MB (97892043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b588537119b781c8e1cd9616a8d91dd409aebde5288fc7ad5cd13d00d178ba`  
		Last Modified: Fri, 21 Feb 2020 23:08:00 GMT  
		Size: 7.6 KB (7593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c845c46aab921783562beea56f3b8d97232e8ebf6f45e27e0c814fe5156edc3`  
		Last Modified: Fri, 21 Feb 2020 23:08:00 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:072894a03f11ec6c58fc4ad34edc6a7bec7b28ec43a748d284e407f47630cd39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.1 MB (215067747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d3d105d191ad7a62321480c529852d331d025c12aac832fdcb23fced63aaf0`
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
# Fri, 21 Feb 2020 22:23:24 GMT
ENV BONITA_VERSION=7.10.1
# Fri, 21 Feb 2020 22:23:25 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Fri, 21 Feb 2020 22:23:26 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 21 Feb 2020 22:23:26 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Fri, 21 Feb 2020 22:23:29 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 21 Feb 2020 22:23:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 22:23:38 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 21 Feb 2020 22:23:40 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 21 Feb 2020 22:23:41 GMT
VOLUME [/opt/bonita]
# Fri, 21 Feb 2020 22:23:41 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 21 Feb 2020 22:23:42 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 21 Feb 2020 22:23:43 GMT
EXPOSE 8080
# Fri, 21 Feb 2020 22:23:44 GMT
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
	-	`sha256:19933018f0b6da42a37134a1aad3a71b6327a2c7bf0ac2dda546ea7a6550cd5c`  
		Last Modified: Fri, 21 Feb 2020 22:24:42 GMT  
		Size: 97.9 MB (97892067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a70958b14b134e50fe58d6202b217c1710f4abd88f585bb729f94889b66ba95`  
		Last Modified: Fri, 21 Feb 2020 22:24:29 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67871a8f5dd1dda50ccc06bd0fac5b8b1a6110f7abc76b2ba422de3085b0b377`  
		Last Modified: Fri, 21 Feb 2020 22:24:30 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:8fd93a53631e540fe3535aaa60fd0e226f5e2805e3efbb075ef6731aa75cbc9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223731313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4681c645cd8f36db6223773755d0222b4f194c9cb6e7b32a6d0b6105f3756558`
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
# Fri, 21 Feb 2020 23:59:25 GMT
ENV BONITA_VERSION=7.10.1
# Fri, 21 Feb 2020 23:59:34 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Fri, 21 Feb 2020 23:59:39 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 21 Feb 2020 23:59:49 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Sat, 22 Feb 2020 00:00:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Sat, 22 Feb 2020 00:05:08 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Sat, 22 Feb 2020 00:05:17 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Sat, 22 Feb 2020 00:05:25 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Sat, 22 Feb 2020 00:05:28 GMT
VOLUME [/opt/bonita]
# Sat, 22 Feb 2020 00:05:29 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Sat, 22 Feb 2020 00:05:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Sat, 22 Feb 2020 00:05:38 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:05:40 GMT
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
	-	`sha256:381df29b7e14a6a4aebb50736b0951825c6bd6225da98332e03c2091d8f054d8`  
		Last Modified: Sat, 22 Feb 2020 00:06:44 GMT  
		Size: 97.9 MB (97892074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f9546ffd71b0bc9e136773f7c52eebfa65578ee82dbb71cab13ec73134acb`  
		Last Modified: Sat, 22 Feb 2020 00:06:36 GMT  
		Size: 7.6 KB (7624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bcd92479045aa95229df017a3bec1fe328257a30c96a5a3b7e6e02b4d3026f`  
		Last Modified: Sat, 22 Feb 2020 00:06:37 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
