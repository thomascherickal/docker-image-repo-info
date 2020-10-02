<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.6`](#bonita7106)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.2`](#bonita7112)
-	[`bonita:7.9`](#bonita79)
-	[`bonita:7.9.5`](#bonita795)
-	[`bonita:latest`](#bonitalatest)

## `bonita:7.10`

```console
$ docker pull bonita@sha256:801a79ae3d49c974727d8c615834d35774d1e440f110efaea7a4f624b18b8e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:ed56b3382c531fcad472135c5b5013d440b6719fc113396af13d6ff8c4ae3ad1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.3 MB (227258338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad0884bd9946aaa33e4bd3c30ec54194282359b3aec75a2d069078a637e4b5f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:19:38 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 02 Oct 2020 21:19:38 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 02 Oct 2020 21:19:39 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:19:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 02 Oct 2020 21:19:40 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:42 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:45 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:19:45 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:19:46 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 02 Oct 2020 21:19:46 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 02 Oct 2020 21:19:46 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:19:46 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e8c4364b7e29135cab8b3c39ee8fc8e1cb0a9b06abb413ad8be52e79505dee`  
		Last Modified: Fri, 02 Oct 2020 21:20:13 GMT  
		Size: 98.0 MB (97973905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a72cac0a439bfcc5517ba808040d66a32838c95dcf76008a949272fcec481a`  
		Last Modified: Fri, 02 Oct 2020 21:20:08 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d744d2f375764cb75665570a25321939441290d01ea744395b112f8db6d23c`  
		Last Modified: Fri, 02 Oct 2020 21:20:09 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:76bb18e84fc2f7f3c206f21312b8b3223adef6723435da9f970a0acbecd67c7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.3 MB (215268032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f267450df7e24f0754448717171817e5d8f399bb5935ee08c1d6abaec2bc6abb`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 20:40:05 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 02 Oct 2020 20:40:05 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 02 Oct 2020 20:40:06 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 20:40:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 02 Oct 2020 20:40:08 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 20:40:14 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:16 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 20:40:19 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 20:40:20 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 02 Oct 2020 20:40:21 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 02 Oct 2020 20:40:21 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 20:40:22 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c346a88bc52bca54f6745beb8185bea051f4fbfb40f8be6104ff8f5f757fe9`  
		Last Modified: Fri, 02 Oct 2020 20:41:08 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d303c1a3f9cda3cf829c5558f01dafcea7496782b4241db7769d69ae2234db`  
		Last Modified: Fri, 02 Oct 2020 20:41:01 GMT  
		Size: 7.7 KB (7650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f814c3268d1a01fee6e2b0a747c269ddf5ed4c1a8aee4b9f1c6bd5591d61dc`  
		Last Modified: Fri, 02 Oct 2020 20:41:04 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:ccda138193c6219e07c827cb18fb84e3f64ed51631191344aa0885f34d0ba462
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (223954482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53504672add2122833646f2ddb0798f976993198a3686bb3ab1ebe28f42d2d89`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:32:40 GMT
ARG BASE_URL
# Sat, 26 Sep 2020 03:32:44 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:18:25 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 02 Oct 2020 21:18:34 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 02 Oct 2020 21:18:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:18:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 02 Oct 2020 21:19:09 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:31 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:46 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:20:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:20:11 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:20:13 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 02 Oct 2020 21:20:17 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 02 Oct 2020 21:20:21 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:20:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a976f7a64af7c1ad0bd07fb507db383af946510dde0d9153227a59e13dc52`  
		Last Modified: Fri, 02 Oct 2020 21:23:30 GMT  
		Size: 98.0 MB (97973961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a853809ef5ddfb0f940a8cb762287fee5df363a3571236f16478ea0ede2605`  
		Last Modified: Fri, 02 Oct 2020 21:23:23 GMT  
		Size: 7.7 KB (7655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96585853cc722e35c073143958e441b5313c84bf83db33d9c9dfee2d792695`  
		Last Modified: Fri, 02 Oct 2020 21:23:23 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:801a79ae3d49c974727d8c615834d35774d1e440f110efaea7a4f624b18b8e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.6` - linux; amd64

```console
$ docker pull bonita@sha256:ed56b3382c531fcad472135c5b5013d440b6719fc113396af13d6ff8c4ae3ad1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.3 MB (227258338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad0884bd9946aaa33e4bd3c30ec54194282359b3aec75a2d069078a637e4b5f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:19:38 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 02 Oct 2020 21:19:38 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 02 Oct 2020 21:19:39 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:19:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 02 Oct 2020 21:19:40 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:42 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:45 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:19:45 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:19:46 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 02 Oct 2020 21:19:46 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 02 Oct 2020 21:19:46 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:19:46 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e8c4364b7e29135cab8b3c39ee8fc8e1cb0a9b06abb413ad8be52e79505dee`  
		Last Modified: Fri, 02 Oct 2020 21:20:13 GMT  
		Size: 98.0 MB (97973905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a72cac0a439bfcc5517ba808040d66a32838c95dcf76008a949272fcec481a`  
		Last Modified: Fri, 02 Oct 2020 21:20:08 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d744d2f375764cb75665570a25321939441290d01ea744395b112f8db6d23c`  
		Last Modified: Fri, 02 Oct 2020 21:20:09 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:76bb18e84fc2f7f3c206f21312b8b3223adef6723435da9f970a0acbecd67c7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.3 MB (215268032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f267450df7e24f0754448717171817e5d8f399bb5935ee08c1d6abaec2bc6abb`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 20:40:05 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 02 Oct 2020 20:40:05 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 02 Oct 2020 20:40:06 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 20:40:07 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 02 Oct 2020 20:40:08 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 20:40:14 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:16 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 20:40:19 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 20:40:20 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 02 Oct 2020 20:40:21 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 02 Oct 2020 20:40:21 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 20:40:22 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c346a88bc52bca54f6745beb8185bea051f4fbfb40f8be6104ff8f5f757fe9`  
		Last Modified: Fri, 02 Oct 2020 20:41:08 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d303c1a3f9cda3cf829c5558f01dafcea7496782b4241db7769d69ae2234db`  
		Last Modified: Fri, 02 Oct 2020 20:41:01 GMT  
		Size: 7.7 KB (7650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f814c3268d1a01fee6e2b0a747c269ddf5ed4c1a8aee4b9f1c6bd5591d61dc`  
		Last Modified: Fri, 02 Oct 2020 20:41:04 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; ppc64le

```console
$ docker pull bonita@sha256:ccda138193c6219e07c827cb18fb84e3f64ed51631191344aa0885f34d0ba462
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.0 MB (223954482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53504672add2122833646f2ddb0798f976993198a3686bb3ab1ebe28f42d2d89`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:32:40 GMT
ARG BASE_URL
# Sat, 26 Sep 2020 03:32:44 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:18:25 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 02 Oct 2020 21:18:34 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 02 Oct 2020 21:18:42 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:18:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 02 Oct 2020 21:19:09 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:31 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:46 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:20:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:20:11 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:20:13 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 02 Oct 2020 21:20:17 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 02 Oct 2020 21:20:21 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:20:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a976f7a64af7c1ad0bd07fb507db383af946510dde0d9153227a59e13dc52`  
		Last Modified: Fri, 02 Oct 2020 21:23:30 GMT  
		Size: 98.0 MB (97973961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a853809ef5ddfb0f940a8cb762287fee5df363a3571236f16478ea0ede2605`  
		Last Modified: Fri, 02 Oct 2020 21:23:23 GMT  
		Size: 7.7 KB (7655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96585853cc722e35c073143958e441b5313c84bf83db33d9c9dfee2d792695`  
		Last Modified: Fri, 02 Oct 2020 21:23:23 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:a8616dc69ca184cbae5107e4ba48251ebaa46554aa4c2105cb3eef775e4a4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:376671555521da6806a5e11951fe218b3b0ddd760a4092cb3a5a837ac71dbf97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.5 MB (242522734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1a40f20c0a015944dcc4ba5a2adcbff93889901cc10d18f775735d1ae13817`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 21:19:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:55 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:58 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:19:58 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:19:59 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 21:19:59 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 21:19:59 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:19:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ac3326e951d1d53ecf7cad866716505a23fb1dc1b17c70de08178ac9b1903e`  
		Last Modified: Fri, 02 Oct 2020 21:20:25 GMT  
		Size: 113.2 MB (113238242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c4eaf486f98a9872b45bf45f753fc5be3a62fd16e5b90c062f34d2f2ac281b`  
		Last Modified: Fri, 02 Oct 2020 21:20:20 GMT  
		Size: 7.6 KB (7625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaa1ddb1a8ca95e0e19b10dbe6268c09571e637bef82b8951ff636e0d38a0b5`  
		Last Modified: Fri, 02 Oct 2020 21:20:20 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b6374fd07eb45b7644a7566c4a5ac83d67318516a710b8c0a715909e50ce7d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2257eb4cafb620b51a988171e7f3fd28b8e917894a3f8ca105e906603ae24148`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 20:40:28 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 20:40:29 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 20:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 20:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 20:40:32 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 20:40:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:39 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:42 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 20:40:43 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 20:40:43 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 20:40:44 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 20:40:45 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 20:40:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedb2e90125341cb9fe6e49685815126b2c4a9d76501d150b69719c95e446d68`  
		Last Modified: Fri, 02 Oct 2020 20:41:26 GMT  
		Size: 113.2 MB (113238279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1526046640a78f9289463f92c42121ccd64e1f7957f4e3dfdabc3682ffff54`  
		Last Modified: Fri, 02 Oct 2020 20:41:16 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada16cf4505b7ea33bf331f89f99d2bd31c7cc71390f914eacec6228a3919d2c`  
		Last Modified: Fri, 02 Oct 2020 20:41:16 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:ad224a8bb29770bd7bd2f1cc15c1e826143aa81f4a0dc3735c10d98c15371673
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239218858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742115eac1b29d82ebed955d3f45663bb43de88da5db663ff27bebb26b864dc4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:32:40 GMT
ARG BASE_URL
# Sat, 26 Sep 2020 03:32:44 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:20:48 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 21:21:01 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 21:21:10 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:21:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 21:21:35 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:21:53 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:22:11 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:22:28 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:22:34 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:22:42 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 21:22:46 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 21:22:50 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:22:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb9a8374541e94b5f735d7f0fcf5dcb0847b2d4b4a2a9b71ceb42a3183c7920`  
		Last Modified: Fri, 02 Oct 2020 21:23:49 GMT  
		Size: 113.2 MB (113238282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2a0a4126af1d57a14a6f19cfe78d56ba7102784d25c0b6404dc3ed14dbac74`  
		Last Modified: Fri, 02 Oct 2020 21:23:42 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78625b5911c1a1fe3e37ee04c4494493a856db2698006f27481ad6b802a6ba4`  
		Last Modified: Fri, 02 Oct 2020 21:23:42 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.2`

```console
$ docker pull bonita@sha256:a8616dc69ca184cbae5107e4ba48251ebaa46554aa4c2105cb3eef775e4a4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.2` - linux; amd64

```console
$ docker pull bonita@sha256:376671555521da6806a5e11951fe218b3b0ddd760a4092cb3a5a837ac71dbf97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.5 MB (242522734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1a40f20c0a015944dcc4ba5a2adcbff93889901cc10d18f775735d1ae13817`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 21:19:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:55 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:58 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:19:58 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:19:59 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 21:19:59 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 21:19:59 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:19:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ac3326e951d1d53ecf7cad866716505a23fb1dc1b17c70de08178ac9b1903e`  
		Last Modified: Fri, 02 Oct 2020 21:20:25 GMT  
		Size: 113.2 MB (113238242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c4eaf486f98a9872b45bf45f753fc5be3a62fd16e5b90c062f34d2f2ac281b`  
		Last Modified: Fri, 02 Oct 2020 21:20:20 GMT  
		Size: 7.6 KB (7625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaa1ddb1a8ca95e0e19b10dbe6268c09571e637bef82b8951ff636e0d38a0b5`  
		Last Modified: Fri, 02 Oct 2020 21:20:20 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b6374fd07eb45b7644a7566c4a5ac83d67318516a710b8c0a715909e50ce7d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2257eb4cafb620b51a988171e7f3fd28b8e917894a3f8ca105e906603ae24148`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 20:40:28 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 20:40:29 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 20:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 20:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 20:40:32 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 20:40:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:39 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:42 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 20:40:43 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 20:40:43 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 20:40:44 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 20:40:45 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 20:40:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedb2e90125341cb9fe6e49685815126b2c4a9d76501d150b69719c95e446d68`  
		Last Modified: Fri, 02 Oct 2020 20:41:26 GMT  
		Size: 113.2 MB (113238279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1526046640a78f9289463f92c42121ccd64e1f7957f4e3dfdabc3682ffff54`  
		Last Modified: Fri, 02 Oct 2020 20:41:16 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada16cf4505b7ea33bf331f89f99d2bd31c7cc71390f914eacec6228a3919d2c`  
		Last Modified: Fri, 02 Oct 2020 20:41:16 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:ad224a8bb29770bd7bd2f1cc15c1e826143aa81f4a0dc3735c10d98c15371673
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239218858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742115eac1b29d82ebed955d3f45663bb43de88da5db663ff27bebb26b864dc4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:32:40 GMT
ARG BASE_URL
# Sat, 26 Sep 2020 03:32:44 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:20:48 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 21:21:01 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 21:21:10 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:21:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 21:21:35 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:21:53 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:22:11 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:22:28 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:22:34 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:22:42 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 21:22:46 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 21:22:50 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:22:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb9a8374541e94b5f735d7f0fcf5dcb0847b2d4b4a2a9b71ceb42a3183c7920`  
		Last Modified: Fri, 02 Oct 2020 21:23:49 GMT  
		Size: 113.2 MB (113238282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2a0a4126af1d57a14a6f19cfe78d56ba7102784d25c0b6404dc3ed14dbac74`  
		Last Modified: Fri, 02 Oct 2020 21:23:42 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78625b5911c1a1fe3e37ee04c4494493a856db2698006f27481ad6b802a6ba4`  
		Last Modified: Fri, 02 Oct 2020 21:23:42 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9`

```console
$ docker pull bonita@sha256:0267697a2f6faacd7e8cf4059dc49a9ac48676b643e98ee95d41d87e66001d20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9` - linux; amd64

```console
$ docker pull bonita@sha256:6dd7434048c6ce0d7cf65765c2ef6536533574903972e74aaacaa548913d924a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.3 MB (229309326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ba5fb2960dd0440f3128c99af425d16d930666ab8d578eb2e7dd17518bc77c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_URL
# Fri, 25 Sep 2020 23:41:51 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 25 Sep 2020 23:41:51 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 25 Sep 2020 23:41:51 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 25 Sep 2020 23:42:01 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:42:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:42:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 25 Sep 2020 23:42:04 GMT
VOLUME [/opt/bonita]
# Fri, 25 Sep 2020 23:42:04 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 25 Sep 2020 23:42:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 25 Sep 2020 23:42:04 GMT
EXPOSE 8080
# Fri, 25 Sep 2020 23:42:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df12a7f39d6849f5acbf70ea4ca165fc6b0f07477eddf53ae0b1207ab03245`  
		Last Modified: Fri, 25 Sep 2020 23:42:56 GMT  
		Size: 100.0 MB (100024954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e92a2e89fe94010b0cdad922da1433fbeb2b714f1ea82d598a6bf82bec2b28`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf3e10066052f2a8c3180843296f3faecef55cce051176c6ab2194862c974f7`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 1.6 KB (1627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:2b2b8fed33fbef0d3d8bdae8e9aad890ccb2035cbc00937d0eae544d125ea744
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217319007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6f7d0f9f98b33412ff678787befd2b209860cf88c9779620078fecf18bb728`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:15:43 GMT
ARG BONITA_URL
# Fri, 25 Sep 2020 23:15:43 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 25 Sep 2020 23:15:44 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 25 Sep 2020 23:15:44 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 25 Sep 2020 23:15:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:15:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:15:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 25 Sep 2020 23:16:00 GMT
VOLUME [/opt/bonita]
# Fri, 25 Sep 2020 23:16:01 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 25 Sep 2020 23:16:01 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 25 Sep 2020 23:16:02 GMT
EXPOSE 8080
# Fri, 25 Sep 2020 23:16:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba78f1892dd49488cd1e0379d04df4d330dd840a0e6a72c6d641b72056261850`  
		Last Modified: Fri, 25 Sep 2020 23:17:15 GMT  
		Size: 100.0 MB (100024998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928e8923f26cf76d52e539b56af1306b4c9ad8196e6c644b8ca542953e81cebf`  
		Last Modified: Fri, 25 Sep 2020 23:17:05 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5359086d34b0cdae532bb4c1b02984b1dd86c710f69956c7bcbfa17bdcb6af9a`  
		Last Modified: Fri, 25 Sep 2020 23:17:05 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; ppc64le

```console
$ docker pull bonita@sha256:fb96dcdef70970a0c3e0ab5901cf885c9ba983a23e7568e0e71098c23b2463dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226005453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41738009cf190898409332797a8509227b6a5983c82c0d73f8068b054f6b0449`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:30:56 GMT
ARG BONITA_URL
# Sat, 26 Sep 2020 03:31:03 GMT
ENV BONITA_VERSION=7.9.5
# Sat, 26 Sep 2020 03:31:08 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Sat, 26 Sep 2020 03:31:14 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Sat, 26 Sep 2020 03:31:45 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Sat, 26 Sep 2020 03:31:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Sat, 26 Sep 2020 03:32:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Sat, 26 Sep 2020 03:32:07 GMT
VOLUME [/opt/bonita]
# Sat, 26 Sep 2020 03:32:08 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Sat, 26 Sep 2020 03:32:09 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Sat, 26 Sep 2020 03:32:12 GMT
EXPOSE 8080
# Sat, 26 Sep 2020 03:32:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f13d3f9382602b6be6714234d241fc55503d84bd44510f2079b3780d407f12`  
		Last Modified: Sat, 26 Sep 2020 03:36:18 GMT  
		Size: 100.0 MB (100025000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e37c9bee6801e902a0424a33961cfa7f9a3d831242d28de47136f492f26f8d`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afe094faae2bb36b5cf8883854120c3003a2059e9fbe5401cd6de59fbbf2df4`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9.5`

```console
$ docker pull bonita@sha256:0267697a2f6faacd7e8cf4059dc49a9ac48676b643e98ee95d41d87e66001d20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9.5` - linux; amd64

```console
$ docker pull bonita@sha256:6dd7434048c6ce0d7cf65765c2ef6536533574903972e74aaacaa548913d924a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.3 MB (229309326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ba5fb2960dd0440f3128c99af425d16d930666ab8d578eb2e7dd17518bc77c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_URL
# Fri, 25 Sep 2020 23:41:51 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 25 Sep 2020 23:41:51 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 25 Sep 2020 23:41:51 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 25 Sep 2020 23:42:01 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:42:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:42:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 25 Sep 2020 23:42:04 GMT
VOLUME [/opt/bonita]
# Fri, 25 Sep 2020 23:42:04 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 25 Sep 2020 23:42:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 25 Sep 2020 23:42:04 GMT
EXPOSE 8080
# Fri, 25 Sep 2020 23:42:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df12a7f39d6849f5acbf70ea4ca165fc6b0f07477eddf53ae0b1207ab03245`  
		Last Modified: Fri, 25 Sep 2020 23:42:56 GMT  
		Size: 100.0 MB (100024954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e92a2e89fe94010b0cdad922da1433fbeb2b714f1ea82d598a6bf82bec2b28`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf3e10066052f2a8c3180843296f3faecef55cce051176c6ab2194862c974f7`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 1.6 KB (1627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:2b2b8fed33fbef0d3d8bdae8e9aad890ccb2035cbc00937d0eae544d125ea744
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217319007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6f7d0f9f98b33412ff678787befd2b209860cf88c9779620078fecf18bb728`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:15:43 GMT
ARG BONITA_URL
# Fri, 25 Sep 2020 23:15:43 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 25 Sep 2020 23:15:44 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 25 Sep 2020 23:15:44 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 25 Sep 2020 23:15:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:15:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 25 Sep 2020 23:15:59 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 25 Sep 2020 23:16:00 GMT
VOLUME [/opt/bonita]
# Fri, 25 Sep 2020 23:16:01 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 25 Sep 2020 23:16:01 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 25 Sep 2020 23:16:02 GMT
EXPOSE 8080
# Fri, 25 Sep 2020 23:16:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba78f1892dd49488cd1e0379d04df4d330dd840a0e6a72c6d641b72056261850`  
		Last Modified: Fri, 25 Sep 2020 23:17:15 GMT  
		Size: 100.0 MB (100024998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928e8923f26cf76d52e539b56af1306b4c9ad8196e6c644b8ca542953e81cebf`  
		Last Modified: Fri, 25 Sep 2020 23:17:05 GMT  
		Size: 7.6 KB (7585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5359086d34b0cdae532bb4c1b02984b1dd86c710f69956c7bcbfa17bdcb6af9a`  
		Last Modified: Fri, 25 Sep 2020 23:17:05 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; ppc64le

```console
$ docker pull bonita@sha256:fb96dcdef70970a0c3e0ab5901cf885c9ba983a23e7568e0e71098c23b2463dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (226005453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41738009cf190898409332797a8509227b6a5983c82c0d73f8068b054f6b0449`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:30:56 GMT
ARG BONITA_URL
# Sat, 26 Sep 2020 03:31:03 GMT
ENV BONITA_VERSION=7.9.5
# Sat, 26 Sep 2020 03:31:08 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Sat, 26 Sep 2020 03:31:14 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Sat, 26 Sep 2020 03:31:45 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Sat, 26 Sep 2020 03:31:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Sat, 26 Sep 2020 03:32:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Sat, 26 Sep 2020 03:32:07 GMT
VOLUME [/opt/bonita]
# Sat, 26 Sep 2020 03:32:08 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Sat, 26 Sep 2020 03:32:09 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Sat, 26 Sep 2020 03:32:12 GMT
EXPOSE 8080
# Sat, 26 Sep 2020 03:32:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f13d3f9382602b6be6714234d241fc55503d84bd44510f2079b3780d407f12`  
		Last Modified: Sat, 26 Sep 2020 03:36:18 GMT  
		Size: 100.0 MB (100025000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e37c9bee6801e902a0424a33961cfa7f9a3d831242d28de47136f492f26f8d`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afe094faae2bb36b5cf8883854120c3003a2059e9fbe5401cd6de59fbbf2df4`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:a8616dc69ca184cbae5107e4ba48251ebaa46554aa4c2105cb3eef775e4a4739
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:376671555521da6806a5e11951fe218b3b0ddd760a4092cb3a5a837ac71dbf97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.5 MB (242522734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1a40f20c0a015944dcc4ba5a2adcbff93889901cc10d18f775735d1ae13817`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:41:10 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:41:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:41:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:41:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:41:50 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:41:50 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:41:51 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:42:15 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:19:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 21:19:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:19:55 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:19:58 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:19:58 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:19:59 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 21:19:59 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 21:19:59 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:19:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b26225e2399009e0af570eebb768bfcbe84cb6c29b1904acdde559aa23f5ea`  
		Last Modified: Fri, 25 Sep 2020 23:43:07 GMT  
		Size: 102.0 MB (101998153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a756bb5a69747c3a85260b46c657b99989e66e321215246e71037a10243f35`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2a72327f28ef87b1a7d940367fe2bd4bde9b327a8efe0d35fd44b7d5c19ab6`  
		Last Modified: Fri, 25 Sep 2020 23:42:49 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf8ca91d922430c6fecd7439843b96ee71b8d1116fcf27a619ef4ff6b5b5f8e`  
		Last Modified: Fri, 25 Sep 2020 23:42:50 GMT  
		Size: 572.4 KB (572374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ac3326e951d1d53ecf7cad866716505a23fb1dc1b17c70de08178ac9b1903e`  
		Last Modified: Fri, 02 Oct 2020 21:20:25 GMT  
		Size: 113.2 MB (113238242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c4eaf486f98a9872b45bf45f753fc5be3a62fd16e5b90c062f34d2f2ac281b`  
		Last Modified: Fri, 02 Oct 2020 21:20:20 GMT  
		Size: 7.6 KB (7625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaa1ddb1a8ca95e0e19b10dbe6268c09571e637bef82b8951ff636e0d38a0b5`  
		Last Modified: Fri, 02 Oct 2020 21:20:20 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b6374fd07eb45b7644a7566c4a5ac83d67318516a710b8c0a715909e50ce7d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2257eb4cafb620b51a988171e7f3fd28b8e917894a3f8ca105e906603ae24148`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:14:35 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 25 Sep 2020 23:15:32 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:15:36 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 25 Sep 2020 23:15:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 25 Sep 2020 23:15:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 25 Sep 2020 23:15:41 GMT
ARG BONITA_VERSION
# Fri, 25 Sep 2020 23:15:42 GMT
ARG BONITA_SHA256
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BASE_URL
# Fri, 25 Sep 2020 23:16:09 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 20:40:28 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 20:40:29 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 20:40:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 20:40:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 20:40:32 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 20:40:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:39 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 20:40:42 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 20:40:43 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 20:40:43 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 20:40:44 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 20:40:45 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 20:40:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa1dfd15710a6e16b3f5fed6c59c0bdb0a7ba405f5ba3f7ff792b76ad7d3350`  
		Last Modified: Fri, 25 Sep 2020 23:17:31 GMT  
		Size: 93.0 MB (93016994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62720c7fb3413709158ccd43c2ca056a10127529b175f1117dd4ca5a750a776`  
		Last Modified: Fri, 25 Sep 2020 23:17:06 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c12fdedbbeedcbc7e7bb2d253a8d5ddddc45dba884ced5beda6368436be77a`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4504a1dcb9b969292970b3d7cb79bbb573c83ff79706fa346afae5e2e8996f3d`  
		Last Modified: Fri, 25 Sep 2020 23:17:04 GMT  
		Size: 541.8 KB (541812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedb2e90125341cb9fe6e49685815126b2c4a9d76501d150b69719c95e446d68`  
		Last Modified: Fri, 02 Oct 2020 20:41:26 GMT  
		Size: 113.2 MB (113238279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1526046640a78f9289463f92c42121ccd64e1f7957f4e3dfdabc3682ffff54`  
		Last Modified: Fri, 02 Oct 2020 20:41:16 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada16cf4505b7ea33bf331f89f99d2bd31c7cc71390f914eacec6228a3919d2c`  
		Last Modified: Fri, 02 Oct 2020 20:41:16 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:ad224a8bb29770bd7bd2f1cc15c1e826143aa81f4a0dc3735c10d98c15371673
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239218858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742115eac1b29d82ebed955d3f45663bb43de88da5db663ff27bebb26b864dc4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 03:25:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Sat, 26 Sep 2020 03:29:47 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 03:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Sat, 26 Sep 2020 03:30:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Sat, 26 Sep 2020 03:30:33 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Sat, 26 Sep 2020 03:30:41 GMT
ARG BONITA_VERSION
# Sat, 26 Sep 2020 03:30:48 GMT
ARG BONITA_SHA256
# Sat, 26 Sep 2020 03:32:40 GMT
ARG BASE_URL
# Sat, 26 Sep 2020 03:32:44 GMT
ARG BONITA_URL
# Fri, 02 Oct 2020 21:20:48 GMT
ENV BONITA_VERSION=7.11.2
# Fri, 02 Oct 2020 21:21:01 GMT
ENV BONITA_SHA256=36dca45fed326d700fddc52edc4efe2a14bc1111b2952fc0001047df9cf7a67a
# Fri, 02 Oct 2020 21:21:10 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 02 Oct 2020 21:21:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.2/BonitaCommunity-7.11.2.zip
# Fri, 02 Oct 2020 21:21:35 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 02 Oct 2020 21:21:53 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:22:11 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 02 Oct 2020 21:22:28 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 02 Oct 2020 21:22:34 GMT
VOLUME [/opt/bonita]
# Fri, 02 Oct 2020 21:22:42 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Fri, 02 Oct 2020 21:22:46 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Fri, 02 Oct 2020 21:22:50 GMT
EXPOSE 8080
# Fri, 02 Oct 2020 21:22:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36f615abc241aa46a9f641088be9733489aa54ecdd7656aabbebc59e8babff4`  
		Last Modified: Sat, 26 Sep 2020 03:36:32 GMT  
		Size: 95.0 MB (95018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815598247ab5a7495520c70706e93222c19f009b14fa035185abb72878b65fb`  
		Last Modified: Sat, 26 Sep 2020 03:36:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b957f0e55214fe990421d5d9157a1e2b99678772069be9e9b93204567ce98e8`  
		Last Modified: Sat, 26 Sep 2020 03:36:09 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55cf6fc034ce3ae81db3086f9f903bad18df306e4078a9c4a542cf09dcf0773`  
		Last Modified: Sat, 26 Sep 2020 03:36:10 GMT  
		Size: 541.5 KB (541548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb9a8374541e94b5f735d7f0fcf5dcb0847b2d4b4a2a9b71ceb42a3183c7920`  
		Last Modified: Fri, 02 Oct 2020 21:23:49 GMT  
		Size: 113.2 MB (113238282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2a0a4126af1d57a14a6f19cfe78d56ba7102784d25c0b6404dc3ed14dbac74`  
		Last Modified: Fri, 02 Oct 2020 21:23:42 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78625b5911c1a1fe3e37ee04c4494493a856db2698006f27481ad6b802a6ba4`  
		Last Modified: Fri, 02 Oct 2020 21:23:42 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
