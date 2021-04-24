<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.6`](#bonita7106)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.4`](#bonita7114)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:7a898f79f528c65b32c2f2efe45f9d3b375d33c6174bdd7a2e7825758322e520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:2b44a1fef45d8c7fa37e2bde2d9bffec29d081e9ff243894f3aedccb42185d78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238886419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3e6a88c70ea31055d8626f0ee4d662fa8ef933a2c36fcb0a0683ef0d3d0390`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:06:34 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:06:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:06:53 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:54 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:06:55 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:06:55 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:06:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:07:01 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:07:02 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:07:03 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:07:03 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:07:03 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:07:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cca847a8b05d7da360a1d9cd9936d3d11cf71ab6ee6ca81d2a6b3b7e1581b5`  
		Last Modified: Fri, 23 Apr 2021 23:08:13 GMT  
		Size: 95.2 MB (95189100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bd7055bc50801a03128c5c19cea14dc35d99567bf57ffc779d2a17f30ef7e`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffe8038a23d7684a1948a804d17710b02b4053144462247e888219f8ae8424`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c025e7864e4e9fba2e27f2014f6ac937ac94541c64e8e666b0523db2738d9b`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 573.0 KB (573015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630bdb910bdd0b9c22bbc8e96b1ea35fa207958df34322c862937566576c933`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931106ba7d137c4ddd7dd56d88e7b37bb4a21cdc170b189ffcbad89134803827`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be079bb58053329dca39d1c353d5ebd8468cf4ce08c65533fe48ff1f8168e73`  
		Last Modified: Fri, 23 Apr 2021 23:08:30 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27f2853c123aa99fc49cf6d38387a4ca694ead3d055670224a92d6226e5f2d5`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:af8a53bfb6e27ea3650f74f0f48540db0172afb3a8260c08b25dbc27a2f26fad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226958327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62236c7ad820a96e306c554a13af8e61054e155ff39341d627948654499f540b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:08:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:09:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:45 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:10:27 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:10:28 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:10:29 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:10:31 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:10:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:10:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:10:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:40 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:41 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:10:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:10:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:10:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:10:52 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:10:53 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:10:53 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:10:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91d362d9177afd00abb955d78a76fff12de8d4da99719b4c95de5e86f2c651`  
		Last Modified: Fri, 23 Apr 2021 23:12:13 GMT  
		Size: 86.3 MB (86284829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aed24c5b81ddcfdfdee086882280bb4c910ef3088aaadb9d5d6e60416799f0`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6403bff0a498d1e1dbe22a2af41e22068542bed3b7a44d63d05773b6d8aeedf`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0b8ab388d1b000bbfff698e6e3aec3ebd0de9033f578f47002358a1845ee17`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 542.5 KB (542508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b341c638df0344ae3024f6784445edae52d27085235d6ae8e25911eb84987fa0`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84092c64bcb45836d0210fcd0348b41270b7fb0e241f49c2892279ca86cff829`  
		Last Modified: Fri, 23 Apr 2021 23:12:23 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee7152fe70e9554894db394aa2586d986217f1f2a497ff327710251045e898`  
		Last Modified: Fri, 23 Apr 2021 23:12:33 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0acba7f00f440a0028357aaf3ea55bf9615ad33dcba412a0bdc37a960d4cb5`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:d8bb343fbbf7f37ff4c595b19f273348060d87e525784ae32672c5c6ce972aca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234573340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae2d6e3a34404165f5f50a8bca19f5e13072fd3f2b703811d038984ba331c5e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:08:41 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:01 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:19 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:11:58 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:12:03 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:12:07 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:12:12 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:12:21 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:12:28 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:12:33 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:12:38 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:12:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:13:14 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:13:16 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:13:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:13:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:14:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:14:13 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:14:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:14:26 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:14:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be047d3e2479ae18017944ed11cbf6933cc7049d3a6275a41aa154e03f66213`  
		Last Modified: Fri, 23 Apr 2021 23:16:01 GMT  
		Size: 87.2 MB (87196882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1da83d633f87e31b26ec983a03db1f1ed3394b54eed1a1cb2d8bf4993a2afc`  
		Last Modified: Fri, 23 Apr 2021 23:15:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a42fdde13a6ea190d518a6c35327b88ded7d977fa8cc426c118e63e543ee2`  
		Last Modified: Fri, 23 Apr 2021 23:15:43 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5b115faca16d102a7005faadc25cd3816dde193ea23d84f0622fa1ecb3fae6`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 541.9 KB (541853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f1591731eb4be4107bf95c9ef8af08e17906479d79797e43b93db4991254b`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f90b8052e076b0a193463b0021d4c38c21c64c85d4d7f395ea6bdf62931ce1`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737763ae68b13a2b8306d61e6c96f66cac249744e801693ede607aeed70c6f8e`  
		Last Modified: Fri, 23 Apr 2021 23:16:23 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e025d1ff4e9d49f29bf2d455fa421a7664fcf9463e03501e5e2c6015eba3905`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10`

```console
$ docker pull bonita@sha256:6dc3b932a7bed8d4791543be80068c632dbcf454ecd7e6e28fb7524bc680a641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:c1890073f6855584d98741865778b9f2d953cf02927258da0bb8343d1c6cad09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.0 MB (243973095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0550b29fb89c9b4a82945856fcaa6ab6caa1f94528bdb86c4faeb261ac3e70e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 23 Apr 2021 23:05:43 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:05:44 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:05:45 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:05:48 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 23 Apr 2021 23:05:50 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 23 Apr 2021 23:05:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:05:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:05:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 23 Apr 2021 23:05:57 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:05:57 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 23 Apr 2021 23:05:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 23 Apr 2021 23:05:57 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:05:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c05388d554e2ba999306e0453b83204907efdfbcbed6122ab03ee4537bd4649`  
		Last Modified: Fri, 23 Apr 2021 23:07:44 GMT  
		Size: 118.7 MB (118716702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348f31515cbd1431d983f9e88053e69d9b5a6264576165da5ff9c0ad66405490`  
		Last Modified: Fri, 23 Apr 2021 23:07:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9d453fe0953f71ef4f57527c169c8cfc44dc8129fd8582282b20ab571562b`  
		Last Modified: Fri, 23 Apr 2021 23:07:18 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ac40c7476e7657369805fda2e5339b51b497c6dc8508ebece3c729f0462349`  
		Last Modified: Fri, 23 Apr 2021 23:07:19 GMT  
		Size: 573.0 KB (573014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1b047c6ed93d0ce260d2b936c8de12c552e96dab53b7d061fd767ca6f73f94`  
		Last Modified: Fri, 23 Apr 2021 23:07:24 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9790dca6b1b99ae56e4bb8328276d364c3897f1e1f1dc9b2ac5074a59b935266`  
		Last Modified: Fri, 23 Apr 2021 23:07:18 GMT  
		Size: 7.7 KB (7652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583e631431a05a8f444ffd266bb9be8ecb9fdc55f0b52e7fec00cc3856e80797`  
		Last Modified: Fri, 23 Apr 2021 23:07:18 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ccfc750d77ac5e9d2cd946ad6be7cbbd3cc29f6060d12aede9bcdcee461f0121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231672048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1a0f88436971be178c2d2ac916da190a69106814b1e216a414669f28edd00c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 23 Apr 2021 23:07:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:07:45 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:07:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:07:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:07:55 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:07:56 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:07:58 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:07:59 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:08:00 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 23 Apr 2021 23:08:01 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 23 Apr 2021 23:08:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:08:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 23 Apr 2021 23:08:06 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 23 Apr 2021 23:08:11 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:08:15 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:08:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 23 Apr 2021 23:08:25 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:08:26 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 23 Apr 2021 23:08:27 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 23 Apr 2021 23:08:28 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:08:29 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade57e5738d2f72e51bb2270249ebbba88a1c649870281329bdc2134a80b0ae4`  
		Last Modified: Fri, 23 Apr 2021 23:11:42 GMT  
		Size: 109.4 MB (109439489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7640832cbcf0a87ddcc02c0232c62a56eb8fd8015f5082411571f598bdc23454`  
		Last Modified: Fri, 23 Apr 2021 23:11:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d1367ad4fb48840f0064c8d503e7998771e91a0391d3a2cc66a70561cec7b`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a202a086d830febba35833a424a4723677ffb345bd24cebea2dd8961d5969b12`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 542.5 KB (542485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cbd50c70597e1449d88f8927365171a28a8c24a14770d72b2e5a1faece4191`  
		Last Modified: Fri, 23 Apr 2021 23:11:23 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b307f8eccaa7ca563f8d4d7961af6756017be820742589fa461b92ec72c745a`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373a6b74274e0a00afa66d9fcc980ca14cc7d9da344cc5fa5da128dddbf83d0`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:3864262bf6c0537074de1584326fbed5ea7ce8780bd9eba03828cba9d3a90daf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241064085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ca71b6c57c0a0c495783123b74ddcb84f325ca8721c11142471dcb22d3f380`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:53:58 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 23 Apr 2021 23:01:33 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:01:47 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:02:00 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:02:15 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:02:26 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:02:30 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:02:35 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:02:41 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:02:47 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 23 Apr 2021 23:02:54 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 23 Apr 2021 23:03:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:03:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 23 Apr 2021 23:03:12 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 23 Apr 2021 23:03:28 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:03:40 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:03:50 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 23 Apr 2021 23:03:56 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:03:59 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 23 Apr 2021 23:04:00 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 23 Apr 2021 23:04:06 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:04:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884cf1bd718065522382c4060870e6fe79b45e8f803af94c2eadf23560ab371e`  
		Last Modified: Fri, 23 Apr 2021 23:15:29 GMT  
		Size: 112.1 MB (112128523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e7e4f470a8cd48cea4491e9e518418f78a62927750adfe5f10e1bdefe9a30d`  
		Last Modified: Fri, 23 Apr 2021 23:15:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69b320007e1e27452426b0dee7a17fc0779b25902d3dc15bd2bc27382f20fc4`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 1.9 KB (1925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ce2fb56b119ab6a39ce0f8f6a55d00268978d2504395a955a1af2cae75c89`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 541.9 KB (541869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72820ce7fb63b137efdc75c94608f6dba76d38e15a3ed5448ba677657606cce`  
		Last Modified: Fri, 23 Apr 2021 23:15:14 GMT  
		Size: 98.0 MB (97973962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5214713e173232398b2938d3a51424d1e00d9c67a6d08ea11072828fcae35c`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e4618f6c1b651a763923a994b5b07cf25e86f3ed098dd375d3618dcb919564`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:6dc3b932a7bed8d4791543be80068c632dbcf454ecd7e6e28fb7524bc680a641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.6` - linux; amd64

```console
$ docker pull bonita@sha256:c1890073f6855584d98741865778b9f2d953cf02927258da0bb8343d1c6cad09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.0 MB (243973095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0550b29fb89c9b4a82945856fcaa6ab6caa1f94528bdb86c4faeb261ac3e70e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 23 Apr 2021 23:05:43 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:05:44 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:05:45 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:05:48 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:05:48 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:05:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 23 Apr 2021 23:05:50 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 23 Apr 2021 23:05:54 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:05:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:05:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 23 Apr 2021 23:05:57 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:05:57 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 23 Apr 2021 23:05:57 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 23 Apr 2021 23:05:57 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:05:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c05388d554e2ba999306e0453b83204907efdfbcbed6122ab03ee4537bd4649`  
		Last Modified: Fri, 23 Apr 2021 23:07:44 GMT  
		Size: 118.7 MB (118716702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348f31515cbd1431d983f9e88053e69d9b5a6264576165da5ff9c0ad66405490`  
		Last Modified: Fri, 23 Apr 2021 23:07:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9d453fe0953f71ef4f57527c169c8cfc44dc8129fd8582282b20ab571562b`  
		Last Modified: Fri, 23 Apr 2021 23:07:18 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ac40c7476e7657369805fda2e5339b51b497c6dc8508ebece3c729f0462349`  
		Last Modified: Fri, 23 Apr 2021 23:07:19 GMT  
		Size: 573.0 KB (573014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1b047c6ed93d0ce260d2b936c8de12c552e96dab53b7d061fd767ca6f73f94`  
		Last Modified: Fri, 23 Apr 2021 23:07:24 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9790dca6b1b99ae56e4bb8328276d364c3897f1e1f1dc9b2ac5074a59b935266`  
		Last Modified: Fri, 23 Apr 2021 23:07:18 GMT  
		Size: 7.7 KB (7652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583e631431a05a8f444ffd266bb9be8ecb9fdc55f0b52e7fec00cc3856e80797`  
		Last Modified: Fri, 23 Apr 2021 23:07:18 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ccfc750d77ac5e9d2cd946ad6be7cbbd3cc29f6060d12aede9bcdcee461f0121
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231672048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1a0f88436971be178c2d2ac916da190a69106814b1e216a414669f28edd00c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:34 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 23 Apr 2021 23:07:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:07:45 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:07:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:07:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:07:55 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:07:56 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:07:58 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:07:59 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:08:00 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 23 Apr 2021 23:08:01 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 23 Apr 2021 23:08:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:08:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 23 Apr 2021 23:08:06 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 23 Apr 2021 23:08:11 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:08:15 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:08:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 23 Apr 2021 23:08:25 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:08:26 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 23 Apr 2021 23:08:27 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 23 Apr 2021 23:08:28 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:08:29 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade57e5738d2f72e51bb2270249ebbba88a1c649870281329bdc2134a80b0ae4`  
		Last Modified: Fri, 23 Apr 2021 23:11:42 GMT  
		Size: 109.4 MB (109439489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7640832cbcf0a87ddcc02c0232c62a56eb8fd8015f5082411571f598bdc23454`  
		Last Modified: Fri, 23 Apr 2021 23:11:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d1367ad4fb48840f0064c8d503e7998771e91a0391d3a2cc66a70561cec7b`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a202a086d830febba35833a424a4723677ffb345bd24cebea2dd8961d5969b12`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 542.5 KB (542485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cbd50c70597e1449d88f8927365171a28a8c24a14770d72b2e5a1faece4191`  
		Last Modified: Fri, 23 Apr 2021 23:11:23 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b307f8eccaa7ca563f8d4d7961af6756017be820742589fa461b92ec72c745a`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373a6b74274e0a00afa66d9fcc980ca14cc7d9da344cc5fa5da128dddbf83d0`  
		Last Modified: Fri, 23 Apr 2021 23:11:15 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; ppc64le

```console
$ docker pull bonita@sha256:3864262bf6c0537074de1584326fbed5ea7ce8780bd9eba03828cba9d3a90daf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241064085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ca71b6c57c0a0c495783123b74ddcb84f325ca8721c11142471dcb22d3f380`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:53:58 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 23 Apr 2021 23:01:33 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:01:47 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:02:00 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:02:15 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:02:26 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:02:30 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:02:35 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:02:41 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:02:47 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 23 Apr 2021 23:02:54 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 23 Apr 2021 23:03:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:03:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 23 Apr 2021 23:03:12 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 23 Apr 2021 23:03:28 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:03:40 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 23 Apr 2021 23:03:50 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 23 Apr 2021 23:03:56 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:03:59 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 23 Apr 2021 23:04:00 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 23 Apr 2021 23:04:06 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:04:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884cf1bd718065522382c4060870e6fe79b45e8f803af94c2eadf23560ab371e`  
		Last Modified: Fri, 23 Apr 2021 23:15:29 GMT  
		Size: 112.1 MB (112128523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e7e4f470a8cd48cea4491e9e518418f78a62927750adfe5f10e1bdefe9a30d`  
		Last Modified: Fri, 23 Apr 2021 23:15:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69b320007e1e27452426b0dee7a17fc0779b25902d3dc15bd2bc27382f20fc4`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 1.9 KB (1925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0ce2fb56b119ab6a39ce0f8f6a55d00268978d2504395a955a1af2cae75c89`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 541.9 KB (541869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72820ce7fb63b137efdc75c94608f6dba76d38e15a3ed5448ba677657606cce`  
		Last Modified: Fri, 23 Apr 2021 23:15:14 GMT  
		Size: 98.0 MB (97973962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5214713e173232398b2938d3a51424d1e00d9c67a6d08ea11072828fcae35c`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e4618f6c1b651a763923a994b5b07cf25e86f3ed098dd375d3618dcb919564`  
		Last Modified: Fri, 23 Apr 2021 23:15:05 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:dc6e0fe075f058c14a15031a0c0de5c94c3ee44d6284e54be51f86370ec01d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:3a8fad216b7f96f9bcc5d655952c780bbe32306ad45422deaae4a671bcbb204f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235818777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d62457912be2de2bb3d40844fad3d3130ecde37c2f5603decbb92b47aa0176f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:06:34 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:06:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:06:36 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 23 Apr 2021 23:06:36 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 23 Apr 2021 23:06:37 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:06:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:06:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:06:38 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:06:39 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:06:39 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 23 Apr 2021 23:06:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:06:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:06:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:06:46 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:06:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:06:47 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:06:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cca847a8b05d7da360a1d9cd9936d3d11cf71ab6ee6ca81d2a6b3b7e1581b5`  
		Last Modified: Fri, 23 Apr 2021 23:08:13 GMT  
		Size: 95.2 MB (95189100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bd7055bc50801a03128c5c19cea14dc35d99567bf57ffc779d2a17f30ef7e`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffe8038a23d7684a1948a804d17710b02b4053144462247e888219f8ae8424`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c025e7864e4e9fba2e27f2014f6ac937ac94541c64e8e666b0523db2738d9b`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 573.0 KB (573015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8895c3eb7436f0070e16c1df897c8f270c16cff36b4aac50565fee4cc389188a`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab92cdf4b9c019a1433ea988c0ef5f0f84dc299c3ff8e698e2be676e7297b193`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49b2b391a49306841f70f1e6c7b92e2943013395ffc51719b82c5220be83e`  
		Last Modified: Fri, 23 Apr 2021 23:08:03 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b34ea17f421d691d9597f37b58ddb29231905685d915228a845eaf2b0a8ac84`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7611c269cf48767612b8aae5fb52644c70dcf4e23a3360fa9418235ce54ab317
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223890694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1c53561fb93fb9f9c6005319a9952d0eac4eae2d7e8341e3ce94be05bbbdc5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:08:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:09:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:45 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:09:46 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:09:46 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:09:47 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:09:48 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 23 Apr 2021 23:09:49 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 23 Apr 2021 23:09:50 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:09:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:09:53 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:09:58 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:01 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:02 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 23 Apr 2021 23:10:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:10:11 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:10:14 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:10:15 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:10:16 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:10:17 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:10:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91d362d9177afd00abb955d78a76fff12de8d4da99719b4c95de5e86f2c651`  
		Last Modified: Fri, 23 Apr 2021 23:12:13 GMT  
		Size: 86.3 MB (86284829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aed24c5b81ddcfdfdee086882280bb4c910ef3088aaadb9d5d6e60416799f0`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6403bff0a498d1e1dbe22a2af41e22068542bed3b7a44d63d05773b6d8aeedf`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0b8ab388d1b000bbfff698e6e3aec3ebd0de9033f578f47002358a1845ee17`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 542.5 KB (542508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920bdfed2b086058691908a0c0f56e21498c0f359a529a66aa3f869ebaa16af6`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe1377e6db0788bf29b827e661cd84f79725404669a8858118edabde7a38917`  
		Last Modified: Fri, 23 Apr 2021 23:11:50 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315059e213cefb8b4a5d3485df76455434eb4d970f9db9eb443266f7ec173e14`  
		Last Modified: Fri, 23 Apr 2021 23:12:00 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468221140670b4afa95daf8476b3d3c22bc752de34eb4c1a338b49d8ef650758`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:ced1c099ee748c164f4f5a79ed8bce3f54aee80602d69e8c8ea81491b57e5f7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231505712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f57a71fca3bb7d92664f8aa7ae8e9aea62ec791115e5ea5eaa08c245a55ffc0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:08:41 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:01 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:19 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:09:25 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:09:30 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:09:36 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:09:41 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 23 Apr 2021 23:09:48 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 23 Apr 2021 23:09:54 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:09:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:10:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:10:14 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:26 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:29 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 23 Apr 2021 23:10:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:11:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:11:22 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:11:26 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:11:27 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:11:31 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:11:38 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be047d3e2479ae18017944ed11cbf6933cc7049d3a6275a41aa154e03f66213`  
		Last Modified: Fri, 23 Apr 2021 23:16:01 GMT  
		Size: 87.2 MB (87196882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1da83d633f87e31b26ec983a03db1f1ed3394b54eed1a1cb2d8bf4993a2afc`  
		Last Modified: Fri, 23 Apr 2021 23:15:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a42fdde13a6ea190d518a6c35327b88ded7d977fa8cc426c118e63e543ee2`  
		Last Modified: Fri, 23 Apr 2021 23:15:43 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5b115faca16d102a7005faadc25cd3816dde193ea23d84f0622fa1ecb3fae6`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 541.9 KB (541853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce031f5313f01747a6a4259eb5663193f8e72386809c7720d7c7c06c944fbc1`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da789b67fb38d4bc3991148f24d8dfd739d8753aaa33441324891615e8a3a2e`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 6.9 KB (6897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6504a811d73024ccc9fb3d654b3ca320706a5a66fd6b87cd72dcadd61939665`  
		Last Modified: Fri, 23 Apr 2021 23:15:52 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5f4b10d6a7cb8eb7ab6cfba102f70ea45320bdee02c77f835fb8ec2c3e844d`  
		Last Modified: Fri, 23 Apr 2021 23:15:42 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:dc6e0fe075f058c14a15031a0c0de5c94c3ee44d6284e54be51f86370ec01d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:3a8fad216b7f96f9bcc5d655952c780bbe32306ad45422deaae4a671bcbb204f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235818777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d62457912be2de2bb3d40844fad3d3130ecde37c2f5603decbb92b47aa0176f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:06:34 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:06:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:06:36 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 23 Apr 2021 23:06:36 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 23 Apr 2021 23:06:37 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:06:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:06:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:06:38 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:06:39 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:06:39 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 23 Apr 2021 23:06:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:06:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:06:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:06:46 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:06:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:06:47 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:06:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cca847a8b05d7da360a1d9cd9936d3d11cf71ab6ee6ca81d2a6b3b7e1581b5`  
		Last Modified: Fri, 23 Apr 2021 23:08:13 GMT  
		Size: 95.2 MB (95189100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bd7055bc50801a03128c5c19cea14dc35d99567bf57ffc779d2a17f30ef7e`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffe8038a23d7684a1948a804d17710b02b4053144462247e888219f8ae8424`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c025e7864e4e9fba2e27f2014f6ac937ac94541c64e8e666b0523db2738d9b`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 573.0 KB (573015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8895c3eb7436f0070e16c1df897c8f270c16cff36b4aac50565fee4cc389188a`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab92cdf4b9c019a1433ea988c0ef5f0f84dc299c3ff8e698e2be676e7297b193`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd49b2b391a49306841f70f1e6c7b92e2943013395ffc51719b82c5220be83e`  
		Last Modified: Fri, 23 Apr 2021 23:08:03 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b34ea17f421d691d9597f37b58ddb29231905685d915228a845eaf2b0a8ac84`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7611c269cf48767612b8aae5fb52644c70dcf4e23a3360fa9418235ce54ab317
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223890694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1c53561fb93fb9f9c6005319a9952d0eac4eae2d7e8341e3ce94be05bbbdc5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:08:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:09:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:45 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:09:46 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:09:46 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:09:47 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:09:48 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 23 Apr 2021 23:09:49 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 23 Apr 2021 23:09:50 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:09:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:09:53 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:09:58 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:01 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:02 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 23 Apr 2021 23:10:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:10:11 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:10:14 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:10:15 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:10:16 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:10:17 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:10:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91d362d9177afd00abb955d78a76fff12de8d4da99719b4c95de5e86f2c651`  
		Last Modified: Fri, 23 Apr 2021 23:12:13 GMT  
		Size: 86.3 MB (86284829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aed24c5b81ddcfdfdee086882280bb4c910ef3088aaadb9d5d6e60416799f0`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6403bff0a498d1e1dbe22a2af41e22068542bed3b7a44d63d05773b6d8aeedf`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0b8ab388d1b000bbfff698e6e3aec3ebd0de9033f578f47002358a1845ee17`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 542.5 KB (542508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920bdfed2b086058691908a0c0f56e21498c0f359a529a66aa3f869ebaa16af6`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe1377e6db0788bf29b827e661cd84f79725404669a8858118edabde7a38917`  
		Last Modified: Fri, 23 Apr 2021 23:11:50 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315059e213cefb8b4a5d3485df76455434eb4d970f9db9eb443266f7ec173e14`  
		Last Modified: Fri, 23 Apr 2021 23:12:00 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468221140670b4afa95daf8476b3d3c22bc752de34eb4c1a338b49d8ef650758`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:ced1c099ee748c164f4f5a79ed8bce3f54aee80602d69e8c8ea81491b57e5f7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231505712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f57a71fca3bb7d92664f8aa7ae8e9aea62ec791115e5ea5eaa08c245a55ffc0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:08:41 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:01 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:19 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:09:25 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:09:30 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:09:36 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:09:41 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 23 Apr 2021 23:09:48 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 23 Apr 2021 23:09:54 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:09:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:10:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 23 Apr 2021 23:10:14 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:26 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:29 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 23 Apr 2021 23:10:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:11:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:11:22 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:11:26 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:11:27 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:11:31 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:11:38 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be047d3e2479ae18017944ed11cbf6933cc7049d3a6275a41aa154e03f66213`  
		Last Modified: Fri, 23 Apr 2021 23:16:01 GMT  
		Size: 87.2 MB (87196882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1da83d633f87e31b26ec983a03db1f1ed3394b54eed1a1cb2d8bf4993a2afc`  
		Last Modified: Fri, 23 Apr 2021 23:15:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a42fdde13a6ea190d518a6c35327b88ded7d977fa8cc426c118e63e543ee2`  
		Last Modified: Fri, 23 Apr 2021 23:15:43 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5b115faca16d102a7005faadc25cd3816dde193ea23d84f0622fa1ecb3fae6`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 541.9 KB (541853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce031f5313f01747a6a4259eb5663193f8e72386809c7720d7c7c06c944fbc1`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da789b67fb38d4bc3991148f24d8dfd739d8753aaa33441324891615e8a3a2e`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 6.9 KB (6897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6504a811d73024ccc9fb3d654b3ca320706a5a66fd6b87cd72dcadd61939665`  
		Last Modified: Fri, 23 Apr 2021 23:15:52 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5f4b10d6a7cb8eb7ab6cfba102f70ea45320bdee02c77f835fb8ec2c3e844d`  
		Last Modified: Fri, 23 Apr 2021 23:15:42 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:7a898f79f528c65b32c2f2efe45f9d3b375d33c6174bdd7a2e7825758322e520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:2b44a1fef45d8c7fa37e2bde2d9bffec29d081e9ff243894f3aedccb42185d78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238886419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3e6a88c70ea31055d8626f0ee4d662fa8ef933a2c36fcb0a0683ef0d3d0390`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:06:34 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:06:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:06:53 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:54 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:06:55 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:06:55 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:06:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:07:01 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:07:02 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:07:03 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:07:03 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:07:03 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:07:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cca847a8b05d7da360a1d9cd9936d3d11cf71ab6ee6ca81d2a6b3b7e1581b5`  
		Last Modified: Fri, 23 Apr 2021 23:08:13 GMT  
		Size: 95.2 MB (95189100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bd7055bc50801a03128c5c19cea14dc35d99567bf57ffc779d2a17f30ef7e`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffe8038a23d7684a1948a804d17710b02b4053144462247e888219f8ae8424`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c025e7864e4e9fba2e27f2014f6ac937ac94541c64e8e666b0523db2738d9b`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 573.0 KB (573015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630bdb910bdd0b9c22bbc8e96b1ea35fa207958df34322c862937566576c933`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931106ba7d137c4ddd7dd56d88e7b37bb4a21cdc170b189ffcbad89134803827`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be079bb58053329dca39d1c353d5ebd8468cf4ce08c65533fe48ff1f8168e73`  
		Last Modified: Fri, 23 Apr 2021 23:08:30 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27f2853c123aa99fc49cf6d38387a4ca694ead3d055670224a92d6226e5f2d5`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:af8a53bfb6e27ea3650f74f0f48540db0172afb3a8260c08b25dbc27a2f26fad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226958327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62236c7ad820a96e306c554a13af8e61054e155ff39341d627948654499f540b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:08:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:09:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:45 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:10:27 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:10:28 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:10:29 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:10:31 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:10:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:10:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:10:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:40 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:41 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:10:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:10:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:10:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:10:52 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:10:53 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:10:53 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:10:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91d362d9177afd00abb955d78a76fff12de8d4da99719b4c95de5e86f2c651`  
		Last Modified: Fri, 23 Apr 2021 23:12:13 GMT  
		Size: 86.3 MB (86284829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aed24c5b81ddcfdfdee086882280bb4c910ef3088aaadb9d5d6e60416799f0`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6403bff0a498d1e1dbe22a2af41e22068542bed3b7a44d63d05773b6d8aeedf`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0b8ab388d1b000bbfff698e6e3aec3ebd0de9033f578f47002358a1845ee17`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 542.5 KB (542508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b341c638df0344ae3024f6784445edae52d27085235d6ae8e25911eb84987fa0`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84092c64bcb45836d0210fcd0348b41270b7fb0e241f49c2892279ca86cff829`  
		Last Modified: Fri, 23 Apr 2021 23:12:23 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee7152fe70e9554894db394aa2586d986217f1f2a497ff327710251045e898`  
		Last Modified: Fri, 23 Apr 2021 23:12:33 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0acba7f00f440a0028357aaf3ea55bf9615ad33dcba412a0bdc37a960d4cb5`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:d8bb343fbbf7f37ff4c595b19f273348060d87e525784ae32672c5c6ce972aca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234573340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae2d6e3a34404165f5f50a8bca19f5e13072fd3f2b703811d038984ba331c5e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:08:41 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:01 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:19 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:11:58 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:12:03 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:12:07 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:12:12 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:12:21 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:12:28 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:12:33 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:12:38 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:12:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:13:14 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:13:16 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:13:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:13:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:14:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:14:13 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:14:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:14:26 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:14:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be047d3e2479ae18017944ed11cbf6933cc7049d3a6275a41aa154e03f66213`  
		Last Modified: Fri, 23 Apr 2021 23:16:01 GMT  
		Size: 87.2 MB (87196882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1da83d633f87e31b26ec983a03db1f1ed3394b54eed1a1cb2d8bf4993a2afc`  
		Last Modified: Fri, 23 Apr 2021 23:15:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a42fdde13a6ea190d518a6c35327b88ded7d977fa8cc426c118e63e543ee2`  
		Last Modified: Fri, 23 Apr 2021 23:15:43 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5b115faca16d102a7005faadc25cd3816dde193ea23d84f0622fa1ecb3fae6`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 541.9 KB (541853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f1591731eb4be4107bf95c9ef8af08e17906479d79797e43b93db4991254b`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f90b8052e076b0a193463b0021d4c38c21c64c85d4d7f395ea6bdf62931ce1`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737763ae68b13a2b8306d61e6c96f66cac249744e801693ede607aeed70c6f8e`  
		Last Modified: Fri, 23 Apr 2021 23:16:23 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e025d1ff4e9d49f29bf2d455fa421a7664fcf9463e03501e5e2c6015eba3905`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:7a898f79f528c65b32c2f2efe45f9d3b375d33c6174bdd7a2e7825758322e520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:2b44a1fef45d8c7fa37e2bde2d9bffec29d081e9ff243894f3aedccb42185d78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238886419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3e6a88c70ea31055d8626f0ee4d662fa8ef933a2c36fcb0a0683ef0d3d0390`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:06:34 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:06:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:06:53 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:54 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:06:55 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:06:55 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:06:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:07:01 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:07:02 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:07:03 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:07:03 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:07:03 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:07:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cca847a8b05d7da360a1d9cd9936d3d11cf71ab6ee6ca81d2a6b3b7e1581b5`  
		Last Modified: Fri, 23 Apr 2021 23:08:13 GMT  
		Size: 95.2 MB (95189100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bd7055bc50801a03128c5c19cea14dc35d99567bf57ffc779d2a17f30ef7e`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffe8038a23d7684a1948a804d17710b02b4053144462247e888219f8ae8424`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c025e7864e4e9fba2e27f2014f6ac937ac94541c64e8e666b0523db2738d9b`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 573.0 KB (573015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630bdb910bdd0b9c22bbc8e96b1ea35fa207958df34322c862937566576c933`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931106ba7d137c4ddd7dd56d88e7b37bb4a21cdc170b189ffcbad89134803827`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be079bb58053329dca39d1c353d5ebd8468cf4ce08c65533fe48ff1f8168e73`  
		Last Modified: Fri, 23 Apr 2021 23:08:30 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27f2853c123aa99fc49cf6d38387a4ca694ead3d055670224a92d6226e5f2d5`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:af8a53bfb6e27ea3650f74f0f48540db0172afb3a8260c08b25dbc27a2f26fad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226958327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62236c7ad820a96e306c554a13af8e61054e155ff39341d627948654499f540b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:08:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:09:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:45 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:10:27 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:10:28 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:10:29 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:10:31 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:10:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:10:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:10:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:40 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:41 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:10:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:10:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:10:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:10:52 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:10:53 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:10:53 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:10:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91d362d9177afd00abb955d78a76fff12de8d4da99719b4c95de5e86f2c651`  
		Last Modified: Fri, 23 Apr 2021 23:12:13 GMT  
		Size: 86.3 MB (86284829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aed24c5b81ddcfdfdee086882280bb4c910ef3088aaadb9d5d6e60416799f0`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6403bff0a498d1e1dbe22a2af41e22068542bed3b7a44d63d05773b6d8aeedf`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0b8ab388d1b000bbfff698e6e3aec3ebd0de9033f578f47002358a1845ee17`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 542.5 KB (542508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b341c638df0344ae3024f6784445edae52d27085235d6ae8e25911eb84987fa0`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84092c64bcb45836d0210fcd0348b41270b7fb0e241f49c2892279ca86cff829`  
		Last Modified: Fri, 23 Apr 2021 23:12:23 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee7152fe70e9554894db394aa2586d986217f1f2a497ff327710251045e898`  
		Last Modified: Fri, 23 Apr 2021 23:12:33 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0acba7f00f440a0028357aaf3ea55bf9615ad33dcba412a0bdc37a960d4cb5`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:d8bb343fbbf7f37ff4c595b19f273348060d87e525784ae32672c5c6ce972aca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234573340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae2d6e3a34404165f5f50a8bca19f5e13072fd3f2b703811d038984ba331c5e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:08:41 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:01 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:19 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:11:58 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:12:03 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:12:07 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:12:12 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:12:21 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:12:28 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:12:33 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:12:38 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:12:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:13:14 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:13:16 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:13:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:13:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:14:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:14:13 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:14:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:14:26 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:14:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be047d3e2479ae18017944ed11cbf6933cc7049d3a6275a41aa154e03f66213`  
		Last Modified: Fri, 23 Apr 2021 23:16:01 GMT  
		Size: 87.2 MB (87196882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1da83d633f87e31b26ec983a03db1f1ed3394b54eed1a1cb2d8bf4993a2afc`  
		Last Modified: Fri, 23 Apr 2021 23:15:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a42fdde13a6ea190d518a6c35327b88ded7d977fa8cc426c118e63e543ee2`  
		Last Modified: Fri, 23 Apr 2021 23:15:43 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5b115faca16d102a7005faadc25cd3816dde193ea23d84f0622fa1ecb3fae6`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 541.9 KB (541853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f1591731eb4be4107bf95c9ef8af08e17906479d79797e43b93db4991254b`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f90b8052e076b0a193463b0021d4c38c21c64c85d4d7f395ea6bdf62931ce1`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737763ae68b13a2b8306d61e6c96f66cac249744e801693ede607aeed70c6f8e`  
		Last Modified: Fri, 23 Apr 2021 23:16:23 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e025d1ff4e9d49f29bf2d455fa421a7664fcf9463e03501e5e2c6015eba3905`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:7a898f79f528c65b32c2f2efe45f9d3b375d33c6174bdd7a2e7825758322e520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:2b44a1fef45d8c7fa37e2bde2d9bffec29d081e9ff243894f3aedccb42185d78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238886419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3e6a88c70ea31055d8626f0ee4d662fa8ef933a2c36fcb0a0683ef0d3d0390`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:06:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:06:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:06:33 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:06:34 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:06:35 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:06:36 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:06:51 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:06:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:06:53 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:06:54 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:06:55 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:06:55 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:06:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:07:01 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:07:02 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:07:03 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:07:03 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:07:03 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:07:03 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cca847a8b05d7da360a1d9cd9936d3d11cf71ab6ee6ca81d2a6b3b7e1581b5`  
		Last Modified: Fri, 23 Apr 2021 23:08:13 GMT  
		Size: 95.2 MB (95189100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bd7055bc50801a03128c5c19cea14dc35d99567bf57ffc779d2a17f30ef7e`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffe8038a23d7684a1948a804d17710b02b4053144462247e888219f8ae8424`  
		Last Modified: Fri, 23 Apr 2021 23:07:58 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c025e7864e4e9fba2e27f2014f6ac937ac94541c64e8e666b0523db2738d9b`  
		Last Modified: Fri, 23 Apr 2021 23:07:56 GMT  
		Size: 573.0 KB (573015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4630bdb910bdd0b9c22bbc8e96b1ea35fa207958df34322c862937566576c933`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931106ba7d137c4ddd7dd56d88e7b37bb4a21cdc170b189ffcbad89134803827`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be079bb58053329dca39d1c353d5ebd8468cf4ce08c65533fe48ff1f8168e73`  
		Last Modified: Fri, 23 Apr 2021 23:08:30 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27f2853c123aa99fc49cf6d38387a4ca694ead3d055670224a92d6226e5f2d5`  
		Last Modified: Fri, 23 Apr 2021 23:08:25 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:af8a53bfb6e27ea3650f74f0f48540db0172afb3a8260c08b25dbc27a2f26fad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226958327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62236c7ad820a96e306c554a13af8e61054e155ff39341d627948654499f540b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:08:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:09:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:09:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:40 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:45 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:10:27 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:10:28 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:10:29 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:10:30 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:10:31 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:10:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:10:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:10:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:10:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:10:40 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:10:41 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:10:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:10:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:10:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:10:52 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:10:53 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:10:53 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:10:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91d362d9177afd00abb955d78a76fff12de8d4da99719b4c95de5e86f2c651`  
		Last Modified: Fri, 23 Apr 2021 23:12:13 GMT  
		Size: 86.3 MB (86284829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aed24c5b81ddcfdfdee086882280bb4c910ef3088aaadb9d5d6e60416799f0`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6403bff0a498d1e1dbe22a2af41e22068542bed3b7a44d63d05773b6d8aeedf`  
		Last Modified: Fri, 23 Apr 2021 23:11:52 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0b8ab388d1b000bbfff698e6e3aec3ebd0de9033f578f47002358a1845ee17`  
		Last Modified: Fri, 23 Apr 2021 23:11:51 GMT  
		Size: 542.5 KB (542508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b341c638df0344ae3024f6784445edae52d27085235d6ae8e25911eb84987fa0`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84092c64bcb45836d0210fcd0348b41270b7fb0e241f49c2892279ca86cff829`  
		Last Modified: Fri, 23 Apr 2021 23:12:23 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee7152fe70e9554894db394aa2586d986217f1f2a497ff327710251045e898`  
		Last Modified: Fri, 23 Apr 2021 23:12:33 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0acba7f00f440a0028357aaf3ea55bf9615ad33dcba412a0bdc37a960d4cb5`  
		Last Modified: Fri, 23 Apr 2021 23:12:22 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:d8bb343fbbf7f37ff4c595b19f273348060d87e525784ae32672c5c6ce972aca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234573340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae2d6e3a34404165f5f50a8bca19f5e13072fd3f2b703811d038984ba331c5e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:04:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 23 Apr 2021 23:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:08:41 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 23 Apr 2021 23:09:01 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 23 Apr 2021 23:09:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 23 Apr 2021 23:09:19 GMT
ARG BONITA_VERSION
# Fri, 23 Apr 2021 23:11:58 GMT
ARG BRANDING_VERSION
# Fri, 23 Apr 2021 23:12:03 GMT
ARG BONITA_SHA256
# Fri, 23 Apr 2021 23:12:07 GMT
ARG BASE_URL
# Fri, 23 Apr 2021 23:12:12 GMT
ARG BONITA_URL
# Fri, 23 Apr 2021 23:12:21 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 23 Apr 2021 23:12:28 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 23 Apr 2021 23:12:33 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 23 Apr 2021 23:12:38 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 23 Apr 2021 23:12:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 23 Apr 2021 23:12:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 23 Apr 2021 23:13:14 GMT
RUN mkdir /opt/files
# Fri, 23 Apr 2021 23:13:16 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 23 Apr 2021 23:13:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 23 Apr 2021 23:13:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 23 Apr 2021 23:14:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 23 Apr 2021 23:14:13 GMT
VOLUME [/opt/bonita]
# Fri, 23 Apr 2021 23:14:17 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 23 Apr 2021 23:14:26 GMT
EXPOSE 8080
# Fri, 23 Apr 2021 23:14:32 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be047d3e2479ae18017944ed11cbf6933cc7049d3a6275a41aa154e03f66213`  
		Last Modified: Fri, 23 Apr 2021 23:16:01 GMT  
		Size: 87.2 MB (87196882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1da83d633f87e31b26ec983a03db1f1ed3394b54eed1a1cb2d8bf4993a2afc`  
		Last Modified: Fri, 23 Apr 2021 23:15:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a42fdde13a6ea190d518a6c35327b88ded7d977fa8cc426c118e63e543ee2`  
		Last Modified: Fri, 23 Apr 2021 23:15:43 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5b115faca16d102a7005faadc25cd3816dde193ea23d84f0622fa1ecb3fae6`  
		Last Modified: Fri, 23 Apr 2021 23:15:41 GMT  
		Size: 541.9 KB (541853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f1591731eb4be4107bf95c9ef8af08e17906479d79797e43b93db4991254b`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f90b8052e076b0a193463b0021d4c38c21c64c85d4d7f395ea6bdf62931ce1`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737763ae68b13a2b8306d61e6c96f66cac249744e801693ede607aeed70c6f8e`  
		Last Modified: Fri, 23 Apr 2021 23:16:23 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e025d1ff4e9d49f29bf2d455fa421a7664fcf9463e03501e5e2c6015eba3905`  
		Last Modified: Fri, 23 Apr 2021 23:16:14 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
