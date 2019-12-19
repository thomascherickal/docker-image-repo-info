<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.0`](#bonita7100)
-	[`bonita:7.9`](#bonita79)
-	[`bonita:7.9.4`](#bonita794)
-	[`bonita:latest`](#bonitalatest)

## `bonita:7.10`

**does not exist** (yet?)

## `bonita:7.10.0`

**does not exist** (yet?)

## `bonita:7.9`

```console
$ docker pull bonita@sha256:5cf32bfa6c6017047764719ab022d32470cd4646b2d7e0c7cc5099e03029fe3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9` - linux; amd64

```console
$ docker pull bonita@sha256:7c624d9079f53c015f45893b4f36ca4f09bcc26b41a412a46a09e3ffa896260a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229077793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f59315454bc322995846dc0be036edaa49e3762cdb49980189e5eb6a64ab53`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:52:42 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 06:53:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:53:41 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 06:53:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 06:53:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 06:53:44 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 06:53:45 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 06:53:46 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 06:53:46 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 06:53:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 06:53:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 06:53:56 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 06:53:57 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 06:53:57 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 06:53:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 06:53:57 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 06:53:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170227ec870627cbe82ad7fd58b3ab28188e5dcd2cd0455f05ac68824901db1`  
		Last Modified: Thu, 19 Dec 2019 06:54:59 GMT  
		Size: 101.7 MB (101742034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db661a6e0825e45f53aea1d3e30cc53bb0e7a942e300b477337216ba6bf490`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f396ca202aa29dfb69fdd7256afef6cac8396b9ab3d0b55dde2acb96f0266`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e70cbaa2126eb2ddf509ea37cbbab4e42220e63afba09527db1da4035fc9c01`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 572.4 KB (572378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc00ef4b1762f9c04da18a746caa7c39942d495313acadd7b5c0f6f6b18d1124`  
		Last Modified: Thu, 19 Dec 2019 06:54:46 GMT  
		Size: 100.0 MB (100026247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997953d7dfbec44234a03ed292f5e5f07b68832b2bc75d54e4bbd594cff95d47`  
		Last Modified: Thu, 19 Dec 2019 06:54:39 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1d9f419046b06e99bd1f82a0495198e259ea1a35eaa0fdb20f7865330665ab`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ec29ecb22a348890bf72d80c04dd43a7864f66ba66b42e2c729482daa0688e85
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217094552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee6f09b4b9201aa6183685ad772ded6724343f1637345196fbb7ba603926825`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 03:49:55 GMT
ADD file:1f180a3d70349350f43f477e4053af7a5fbc4d62d4e76ada091884500bfb6ee1 in / 
# Thu, 19 Dec 2019 03:50:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:50:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:50:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:50:20 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 08:01:24 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 08:02:50 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 08:03:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 08:03:06 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 08:03:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 08:03:13 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 08:03:14 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 08:03:16 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 08:03:17 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 08:03:19 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 08:03:22 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 08:03:32 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 08:03:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 08:03:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 08:03:39 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 08:03:40 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 08:03:40 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 08:03:42 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 08:03:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:083ab90813fd405397dbca2b021972603ae62211e401e42b4e928dff050de9c2`  
		Last Modified: Mon, 02 Dec 2019 15:30:26 GMT  
		Size: 23.7 MB (23718714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87467c9ed1fdecf80ce31dc51b980ebd7b2391419ff6113f32e4d170c9f4c4b6`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7a1b2b6a922bf6c8024e2f9276928ed5e5538fd58bf3f0ba6a4a193d515ee7`  
		Last Modified: Thu, 19 Dec 2019 03:55:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69de117a966f92306b4142bdfbccb0b74cbef319ce8b1c6652cf92ce28b0ddf1`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443a608c3163dadc992c54bcdcff7aa6a5523d4d43f1dcd9551d1e3ee18486ba`  
		Last Modified: Thu, 19 Dec 2019 08:04:56 GMT  
		Size: 92.8 MB (92760193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62c646ea143b7a7dd976a5770f9857c4ea11c36e72f33bbf762bf277b80f42`  
		Last Modified: Thu, 19 Dec 2019 08:04:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfe768061a33d6c6421f1a53866b8074abcb686b3f7f2a77bc815d5a6461ab9`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6b6b39701aa9bc350a8722c4aadba85f69bb1d21f02c9e93707a3215b1dc4`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 541.8 KB (541819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625c4fafe5567ffb7c64ca522adcfd44227148d8ea920593b22d803fcc3792`  
		Last Modified: Thu, 19 Dec 2019 08:04:40 GMT  
		Size: 100.0 MB (100026272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c7132bd2689dacdaa5df1647ffaa32587fc50a98be158900c544cfcde146fa`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c7ce7740398dc45511729f4359218e5f0dd349a04b12a29e661a4c50e0ca59`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; ppc64le

```console
$ docker pull bonita@sha256:3e61b7f580007334ad7154a0753fe5fe2eedb959622c07c3498b0ef213aa65db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.8 MB (225772818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1084e9d06ce00dd2f7a1cc8452b662a0986e3618fc365690def8f0a15afaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:17:50 GMT
ADD file:04095d1b229274e65c9beb48f6cf33050e58d8ee2cd59c0063d23301a1b68f40 in / 
# Thu, 19 Dec 2019 04:17:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:18:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:18:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:18:08 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:05:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 09:07:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 09:07:58 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 09:08:04 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 09:08:12 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 09:08:14 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 09:08:16 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 09:08:18 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 09:08:20 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 09:08:22 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 09:08:23 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 09:09:11 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 09:09:15 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 09:09:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 09:09:22 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 09:09:23 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 09:09:24 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 09:09:25 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 09:09:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:fc185e8867852536dd99638d9087ed0059bd4d581436d4c2aac0d0e17666457a`  
		Last Modified: Mon, 02 Dec 2019 15:30:19 GMT  
		Size: 30.4 MB (30400283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e561dfe3fdb898460f7652cbe0a7bb83e64b240d2504cec93d1b4a1cff37951`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5731b4e21c4ef8f9ab7c0d9535bc069ed88e51e1701f2c89b9260bbabc3ab4`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c7d0deb99d27ed750b5a40c0b038d79913a8644af69d2954631935aab9d88`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67a74488fd80b101ca952140e3ef48dbd39197f1d7f0dd349ca7b8160ef81af`  
		Last Modified: Thu, 19 Dec 2019 09:10:46 GMT  
		Size: 94.8 MB (94757160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e66c98cb74b4efc907e66b9b991aeecf8de984a4d0cf5e935b6468be2bb3a0`  
		Last Modified: Thu, 19 Dec 2019 09:10:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c5f99428d6d73821011b103a3b1bd656701141e8d054d615890c06c4caa8b5`  
		Last Modified: Thu, 19 Dec 2019 09:10:23 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56404ca74743e278ac37ae9c2f1394d3169131600ac3f91291af13f6568d8901`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 541.5 KB (541543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcbf174ed7483cce8f44ceb4795768ea9deb71fcf13c18e9c684cd8ee628791`  
		Last Modified: Thu, 19 Dec 2019 09:10:33 GMT  
		Size: 100.0 MB (100026271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b97e814f3c9bd01c49a528cb91b0038939ddbd9fa9fb62183cb6deddcada6`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da71769dbfb4e9524f0b34c0da19c261e6de85ab13590506c9d26d49e5d4b418`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9.4`

```console
$ docker pull bonita@sha256:5cf32bfa6c6017047764719ab022d32470cd4646b2d7e0c7cc5099e03029fe3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9.4` - linux; amd64

```console
$ docker pull bonita@sha256:7c624d9079f53c015f45893b4f36ca4f09bcc26b41a412a46a09e3ffa896260a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229077793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f59315454bc322995846dc0be036edaa49e3762cdb49980189e5eb6a64ab53`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:52:42 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 06:53:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:53:41 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 06:53:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 06:53:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 06:53:44 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 06:53:45 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 06:53:46 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 06:53:46 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 06:53:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 06:53:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 06:53:56 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 06:53:57 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 06:53:57 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 06:53:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 06:53:57 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 06:53:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170227ec870627cbe82ad7fd58b3ab28188e5dcd2cd0455f05ac68824901db1`  
		Last Modified: Thu, 19 Dec 2019 06:54:59 GMT  
		Size: 101.7 MB (101742034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db661a6e0825e45f53aea1d3e30cc53bb0e7a942e300b477337216ba6bf490`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f396ca202aa29dfb69fdd7256afef6cac8396b9ab3d0b55dde2acb96f0266`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e70cbaa2126eb2ddf509ea37cbbab4e42220e63afba09527db1da4035fc9c01`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 572.4 KB (572378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc00ef4b1762f9c04da18a746caa7c39942d495313acadd7b5c0f6f6b18d1124`  
		Last Modified: Thu, 19 Dec 2019 06:54:46 GMT  
		Size: 100.0 MB (100026247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997953d7dfbec44234a03ed292f5e5f07b68832b2bc75d54e4bbd594cff95d47`  
		Last Modified: Thu, 19 Dec 2019 06:54:39 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1d9f419046b06e99bd1f82a0495198e259ea1a35eaa0fdb20f7865330665ab`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ec29ecb22a348890bf72d80c04dd43a7864f66ba66b42e2c729482daa0688e85
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217094552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee6f09b4b9201aa6183685ad772ded6724343f1637345196fbb7ba603926825`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 03:49:55 GMT
ADD file:1f180a3d70349350f43f477e4053af7a5fbc4d62d4e76ada091884500bfb6ee1 in / 
# Thu, 19 Dec 2019 03:50:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:50:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:50:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:50:20 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 08:01:24 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 08:02:50 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 08:03:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 08:03:06 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 08:03:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 08:03:13 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 08:03:14 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 08:03:16 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 08:03:17 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 08:03:19 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 08:03:22 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 08:03:32 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 08:03:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 08:03:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 08:03:39 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 08:03:40 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 08:03:40 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 08:03:42 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 08:03:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:083ab90813fd405397dbca2b021972603ae62211e401e42b4e928dff050de9c2`  
		Last Modified: Mon, 02 Dec 2019 15:30:26 GMT  
		Size: 23.7 MB (23718714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87467c9ed1fdecf80ce31dc51b980ebd7b2391419ff6113f32e4d170c9f4c4b6`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7a1b2b6a922bf6c8024e2f9276928ed5e5538fd58bf3f0ba6a4a193d515ee7`  
		Last Modified: Thu, 19 Dec 2019 03:55:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69de117a966f92306b4142bdfbccb0b74cbef319ce8b1c6652cf92ce28b0ddf1`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443a608c3163dadc992c54bcdcff7aa6a5523d4d43f1dcd9551d1e3ee18486ba`  
		Last Modified: Thu, 19 Dec 2019 08:04:56 GMT  
		Size: 92.8 MB (92760193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62c646ea143b7a7dd976a5770f9857c4ea11c36e72f33bbf762bf277b80f42`  
		Last Modified: Thu, 19 Dec 2019 08:04:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfe768061a33d6c6421f1a53866b8074abcb686b3f7f2a77bc815d5a6461ab9`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6b6b39701aa9bc350a8722c4aadba85f69bb1d21f02c9e93707a3215b1dc4`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 541.8 KB (541819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625c4fafe5567ffb7c64ca522adcfd44227148d8ea920593b22d803fcc3792`  
		Last Modified: Thu, 19 Dec 2019 08:04:40 GMT  
		Size: 100.0 MB (100026272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c7132bd2689dacdaa5df1647ffaa32587fc50a98be158900c544cfcde146fa`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c7ce7740398dc45511729f4359218e5f0dd349a04b12a29e661a4c50e0ca59`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:3e61b7f580007334ad7154a0753fe5fe2eedb959622c07c3498b0ef213aa65db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.8 MB (225772818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1084e9d06ce00dd2f7a1cc8452b662a0986e3618fc365690def8f0a15afaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:17:50 GMT
ADD file:04095d1b229274e65c9beb48f6cf33050e58d8ee2cd59c0063d23301a1b68f40 in / 
# Thu, 19 Dec 2019 04:17:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:18:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:18:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:18:08 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:05:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 09:07:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 09:07:58 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 09:08:04 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 09:08:12 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 09:08:14 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 09:08:16 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 09:08:18 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 09:08:20 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 09:08:22 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 09:08:23 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 09:09:11 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 09:09:15 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 09:09:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 09:09:22 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 09:09:23 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 09:09:24 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 09:09:25 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 09:09:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:fc185e8867852536dd99638d9087ed0059bd4d581436d4c2aac0d0e17666457a`  
		Last Modified: Mon, 02 Dec 2019 15:30:19 GMT  
		Size: 30.4 MB (30400283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e561dfe3fdb898460f7652cbe0a7bb83e64b240d2504cec93d1b4a1cff37951`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5731b4e21c4ef8f9ab7c0d9535bc069ed88e51e1701f2c89b9260bbabc3ab4`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c7d0deb99d27ed750b5a40c0b038d79913a8644af69d2954631935aab9d88`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67a74488fd80b101ca952140e3ef48dbd39197f1d7f0dd349ca7b8160ef81af`  
		Last Modified: Thu, 19 Dec 2019 09:10:46 GMT  
		Size: 94.8 MB (94757160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e66c98cb74b4efc907e66b9b991aeecf8de984a4d0cf5e935b6468be2bb3a0`  
		Last Modified: Thu, 19 Dec 2019 09:10:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c5f99428d6d73821011b103a3b1bd656701141e8d054d615890c06c4caa8b5`  
		Last Modified: Thu, 19 Dec 2019 09:10:23 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56404ca74743e278ac37ae9c2f1394d3169131600ac3f91291af13f6568d8901`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 541.5 KB (541543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcbf174ed7483cce8f44ceb4795768ea9deb71fcf13c18e9c684cd8ee628791`  
		Last Modified: Thu, 19 Dec 2019 09:10:33 GMT  
		Size: 100.0 MB (100026271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b97e814f3c9bd01c49a528cb91b0038939ddbd9fa9fb62183cb6deddcada6`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da71769dbfb4e9524f0b34c0da19c261e6de85ab13590506c9d26d49e5d4b418`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:5cf32bfa6c6017047764719ab022d32470cd4646b2d7e0c7cc5099e03029fe3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:7c624d9079f53c015f45893b4f36ca4f09bcc26b41a412a46a09e3ffa896260a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229077793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f59315454bc322995846dc0be036edaa49e3762cdb49980189e5eb6a64ab53`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:52:42 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 06:53:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:53:41 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 06:53:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 06:53:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 06:53:44 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 06:53:45 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 06:53:46 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 06:53:46 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 06:53:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 06:53:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 06:53:56 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 06:53:57 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 06:53:57 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 06:53:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 06:53:57 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 06:53:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170227ec870627cbe82ad7fd58b3ab28188e5dcd2cd0455f05ac68824901db1`  
		Last Modified: Thu, 19 Dec 2019 06:54:59 GMT  
		Size: 101.7 MB (101742034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db661a6e0825e45f53aea1d3e30cc53bb0e7a942e300b477337216ba6bf490`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f396ca202aa29dfb69fdd7256afef6cac8396b9ab3d0b55dde2acb96f0266`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e70cbaa2126eb2ddf509ea37cbbab4e42220e63afba09527db1da4035fc9c01`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 572.4 KB (572378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc00ef4b1762f9c04da18a746caa7c39942d495313acadd7b5c0f6f6b18d1124`  
		Last Modified: Thu, 19 Dec 2019 06:54:46 GMT  
		Size: 100.0 MB (100026247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997953d7dfbec44234a03ed292f5e5f07b68832b2bc75d54e4bbd594cff95d47`  
		Last Modified: Thu, 19 Dec 2019 06:54:39 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1d9f419046b06e99bd1f82a0495198e259ea1a35eaa0fdb20f7865330665ab`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ec29ecb22a348890bf72d80c04dd43a7864f66ba66b42e2c729482daa0688e85
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217094552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee6f09b4b9201aa6183685ad772ded6724343f1637345196fbb7ba603926825`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 03:49:55 GMT
ADD file:1f180a3d70349350f43f477e4053af7a5fbc4d62d4e76ada091884500bfb6ee1 in / 
# Thu, 19 Dec 2019 03:50:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:50:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:50:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:50:20 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 08:01:24 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 08:02:50 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 08:03:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 08:03:06 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 08:03:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 08:03:13 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 08:03:14 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 08:03:16 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 08:03:17 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 08:03:19 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 08:03:22 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 08:03:32 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 08:03:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 08:03:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 08:03:39 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 08:03:40 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 08:03:40 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 08:03:42 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 08:03:42 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:083ab90813fd405397dbca2b021972603ae62211e401e42b4e928dff050de9c2`  
		Last Modified: Mon, 02 Dec 2019 15:30:26 GMT  
		Size: 23.7 MB (23718714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87467c9ed1fdecf80ce31dc51b980ebd7b2391419ff6113f32e4d170c9f4c4b6`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7a1b2b6a922bf6c8024e2f9276928ed5e5538fd58bf3f0ba6a4a193d515ee7`  
		Last Modified: Thu, 19 Dec 2019 03:55:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69de117a966f92306b4142bdfbccb0b74cbef319ce8b1c6652cf92ce28b0ddf1`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443a608c3163dadc992c54bcdcff7aa6a5523d4d43f1dcd9551d1e3ee18486ba`  
		Last Modified: Thu, 19 Dec 2019 08:04:56 GMT  
		Size: 92.8 MB (92760193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62c646ea143b7a7dd976a5770f9857c4ea11c36e72f33bbf762bf277b80f42`  
		Last Modified: Thu, 19 Dec 2019 08:04:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfe768061a33d6c6421f1a53866b8074abcb686b3f7f2a77bc815d5a6461ab9`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6b6b39701aa9bc350a8722c4aadba85f69bb1d21f02c9e93707a3215b1dc4`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 541.8 KB (541819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625c4fafe5567ffb7c64ca522adcfd44227148d8ea920593b22d803fcc3792`  
		Last Modified: Thu, 19 Dec 2019 08:04:40 GMT  
		Size: 100.0 MB (100026272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c7132bd2689dacdaa5df1647ffaa32587fc50a98be158900c544cfcde146fa`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c7ce7740398dc45511729f4359218e5f0dd349a04b12a29e661a4c50e0ca59`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:3e61b7f580007334ad7154a0753fe5fe2eedb959622c07c3498b0ef213aa65db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.8 MB (225772818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b1084e9d06ce00dd2f7a1cc8452b662a0986e3618fc365690def8f0a15afaf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:17:50 GMT
ADD file:04095d1b229274e65c9beb48f6cf33050e58d8ee2cd59c0063d23301a1b68f40 in / 
# Thu, 19 Dec 2019 04:17:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:18:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:18:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:18:08 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:05:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 09:07:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 09:07:58 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 09:08:04 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 09:08:12 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 09:08:14 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 09:08:16 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 09:08:18 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 09:08:20 GMT
ENV BONITA_VERSION=7.9.4
# Thu, 19 Dec 2019 09:08:22 GMT
ENV BONITA_SHA256=0ef0adc47b3886a588802626cc941e43c8fb5c99d0ad815b3e96bdee17c321f7
# Thu, 19 Dec 2019 09:08:23 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.4-tomcat.zip
# Thu, 19 Dec 2019 09:09:11 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 09:09:15 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Thu, 19 Dec 2019 09:09:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Thu, 19 Dec 2019 09:09:22 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 09:09:23 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Thu, 19 Dec 2019 09:09:24 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 09:09:25 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 09:09:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:fc185e8867852536dd99638d9087ed0059bd4d581436d4c2aac0d0e17666457a`  
		Last Modified: Mon, 02 Dec 2019 15:30:19 GMT  
		Size: 30.4 MB (30400283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e561dfe3fdb898460f7652cbe0a7bb83e64b240d2504cec93d1b4a1cff37951`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5731b4e21c4ef8f9ab7c0d9535bc069ed88e51e1701f2c89b9260bbabc3ab4`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c7d0deb99d27ed750b5a40c0b038d79913a8644af69d2954631935aab9d88`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67a74488fd80b101ca952140e3ef48dbd39197f1d7f0dd349ca7b8160ef81af`  
		Last Modified: Thu, 19 Dec 2019 09:10:46 GMT  
		Size: 94.8 MB (94757160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e66c98cb74b4efc907e66b9b991aeecf8de984a4d0cf5e935b6468be2bb3a0`  
		Last Modified: Thu, 19 Dec 2019 09:10:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c5f99428d6d73821011b103a3b1bd656701141e8d054d615890c06c4caa8b5`  
		Last Modified: Thu, 19 Dec 2019 09:10:23 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56404ca74743e278ac37ae9c2f1394d3169131600ac3f91291af13f6568d8901`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 541.5 KB (541543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcbf174ed7483cce8f44ceb4795768ea9deb71fcf13c18e9c684cd8ee628791`  
		Last Modified: Thu, 19 Dec 2019 09:10:33 GMT  
		Size: 100.0 MB (100026271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b97e814f3c9bd01c49a528cb91b0038939ddbd9fa9fb62183cb6deddcada6`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da71769dbfb4e9524f0b34c0da19c261e6de85ab13590506c9d26d49e5d4b418`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
