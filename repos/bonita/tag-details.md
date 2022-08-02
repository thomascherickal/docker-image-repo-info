<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:2021.2`](#bonita20212)
-	[`bonita:2021.2-u0`](#bonita20212-u0)
-	[`bonita:2022.1`](#bonita20221)
-	[`bonita:2022.1-u0`](#bonita20221-u0)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.4`](#bonita7114)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:7.13`](#bonita713)
-	[`bonita:7.13.0`](#bonita7130)
-	[`bonita:7.14`](#bonita714)
-	[`bonita:7.14.0`](#bonita7140)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:8de9c856224a7306e8ac7b5d8e65a8d97bef3a7c8527f3a1f4407c9b45381d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:4c28435d9e29513ff0f7daecfec61544df34fa974e831e25f931c60d73940ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.5 MB (237485947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6cc15457b62c1ba8644edcb7278542a9f91ee4c2e6f59e0453a0b97647f392`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:45:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:45:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:45:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:45:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 02 Aug 2022 18:45:51 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 18:45:52 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 18:45:53 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:45:53 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 02 Aug 2022 18:45:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 02 Aug 2022 18:46:00 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 18:46:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 18:46:01 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:02 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d50e772b503a53e97f96f1c7602b04e6dee66044b4115a656657015cc8dd0b7`  
		Last Modified: Tue, 02 Aug 2022 18:47:21 GMT  
		Size: 93.8 MB (93843076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26eb43ae80cdb0d32344078dcc9a34e5168ec38544ca6ec2d6a570c0bd22c8`  
		Last Modified: Tue, 02 Aug 2022 18:47:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60cd03e6c4f2bb07959adeb37f665329f44d70461b01bb7e4a7f2e4a33c361`  
		Last Modified: Tue, 02 Aug 2022 18:47:08 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baeb6788537273b4b4ea7b4ca7add2abb8b81aca7a21c8f20cb5c658d097fe`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 506.4 KB (506350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139969e8126173a3227b1abe266a8119550d2a8bbb2d1a65c3ffe36da819411`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ca1df3999ff9027299abbcb37e390c0e998fedf8167460080fa1458573f53`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95336ada909617a31482b70af8d5f5e51498eb4e30afa6cbae66ca5e0049968`  
		Last Modified: Tue, 02 Aug 2022 18:47:37 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed438aef59d48263abab0591f1e5f4be92ead54ccb43b8c1c57c1b5facec9769`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7ab361015ccf742c9808e14ce5c2ab028dbfb1bad421c6795bcb5fdae34952d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226598269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30a614d1db72283c5a882db79ce17c54eb505b86100630ee7af353c98f25c4a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:41:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:41:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:41:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:41:17 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:41:17 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:41:47 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:41:48 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:41:49 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:41:50 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:41:51 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 02 Aug 2022 17:41:52 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 02 Aug 2022 17:41:53 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 02 Aug 2022 17:41:54 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 17:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:41:56 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 17:41:57 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 17:41:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:42:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 02 Aug 2022 17:42:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 02 Aug 2022 17:42:06 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 17:42:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 17:42:08 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:42:10 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:42:10 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:42:11 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439589d8fce29b6ddaeaa0d2c2fb68eb16c9f8135829466ddf899922c2c78488`  
		Last Modified: Tue, 02 Aug 2022 17:44:08 GMT  
		Size: 86.0 MB (85961696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca434dad4975c4402f953151563ec4581df90bd8b9f4e3bd670e8fd614ff4b4`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a53a5b66d93db8abb050b7d143e86ef10bae890206b1365d673172628f9e1`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8d82da748df549da0b2ede71952a9099c9ee290d5c22dc38ba1e76b34d2b0`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 475.8 KB (475760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f5e764b86512346f24b36dc95ba83759a1899e2a9b045ee3ec06489ba8f86`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a0280f786f1176a696f1de7847cb62d4bc218e1f5af961737ccf4f5d1d8b1b`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 6.9 KB (6917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6cdcd42d0bf3bf3ef933054227953a11e8579bdad50c64499c65b79a8a5f3c`  
		Last Modified: Tue, 02 Aug 2022 17:44:27 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1677b323555e6b1285259ac735523908155d92868b55464a79dd6d0f5489056`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:b56b3ae5fd5e336c93594767ecae7a32026f87bf5ffd09a13f55c8d45123f978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233951178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9fec1db19fcffd6ebef6c9cae4f880271ccbbfa9600fc7146eeb41f40158d6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:08:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:08:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:08:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:08:42 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:10:29 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:10:30 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:10:32 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:10:35 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:10:38 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 07 Jun 2022 10:10:41 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 07 Jun 2022 10:10:44 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 07 Jun 2022 10:10:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 07 Jun 2022 10:10:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:10:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 07 Jun 2022 10:10:55 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 07 Jun 2022 10:11:01 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:11:02 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 07 Jun 2022 10:11:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 07 Jun 2022 10:11:19 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 07 Jun 2022 10:11:26 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 07 Jun 2022 10:11:30 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:11:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:11:33 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:11:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932cab289b2b2a387d18cfb709811f1a652f05e78ced57c596e0e3a7136ca8f`  
		Last Modified: Tue, 07 Jun 2022 10:16:56 GMT  
		Size: 86.6 MB (86606720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99318a085a88c3b7eefb71e0fb1851bbc6f00b8b9b350cd5f611e0e3294356`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128478c35447ca89ff14fbf5c1a1a2936a18e0012a7f08f2db12e421b6d46159`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4873185aa919a50c4fad4b47828805af6df63bc92c8143b5268a777fade09b6`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 475.3 KB (475347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eceaedc2b9083c2b4baf061ec3fad71b09f51e83d5e7ae2b07aa70e01bc60d3`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba561c4766c632072d54ee899d6956320cc379ead197e70321d06a5936402f0c`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b5afedaeef8dad41a823655dbe702900e9f84fbb2f98bbf9f560534a33c0c9`  
		Last Modified: Tue, 07 Jun 2022 10:17:22 GMT  
		Size: 116.4 MB (116415403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56f59b30a77def4359279676b77dc14e03c625eb67a39ae191af44d2125d0f`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:62920f7249d56ff492ecd65601feca678d819335d76b4cae04dfb0ec2090d6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:1388ad814f4f35bf67df229b9c51eec3bf07ceed47d60e9bc299c9440f61150a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235221886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a04f6ce33e1510259cfe5c41c4375e8860cd6bf9eab5745ba885d600b90cd0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:46:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:46:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:46:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:46:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 18:46:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:46:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:33 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:46:33 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 18:46:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 18:46:43 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 18:46:43 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:44 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec60a66b5ad49a9fc5ae72d2d837c3ead083a79a8cd775cd816ffcd70f66262a`  
		Last Modified: Tue, 02 Aug 2022 18:48:04 GMT  
		Size: 93.8 MB (93846025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48581e1ff3b8c4cc198e8a64401742ad31d1974f84b6787966cc26dcc8f0ce`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad1f5d5e2b55f54ef10f24a0743b24d7acabb3694ba9063fcbabae51b7db121`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483cc6170e8dc85ef8cf416062b65510b66e77cd0a095fca1860fbba19afcaa5`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 930.5 KB (930474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b3f18eb96ef9c253503172278278db98c924179a86195ca8709ad357a672d0`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfacd6f1616f2ee9ac5804a9f2a77020d21adabf4951755fecc916f939cf03f6`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec6677533059e6e25a9e3104dd0244cf6414f60ad33469ed5f5211f591ed151`  
		Last Modified: Tue, 02 Aug 2022 18:47:56 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef62cc2ef2cfab90a2571aa6ca98cd9f41131681af5d812aa2ef10b2745b4d57`  
		Last Modified: Tue, 02 Aug 2022 18:47:49 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c5a0992056eef2b9aeb7b9023169b6561f41058f415ed1c9aaaf0de603e18f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224290844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01446a7647207db9dcef3a6a688fe82790586b7738d010034ee50b9368c9f7ed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:42:42 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:42:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:42:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:42:47 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:42:48 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:42:49 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:42:50 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:42:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:42:52 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 17:42:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 17:42:54 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 17:42:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:42:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:43:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 17:43:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 17:43:09 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 17:43:11 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:43:12 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1ca2ca8943857085e06d4b425c045a8b3ee3a3d7fe89ac23f84d180773b96`  
		Last Modified: Tue, 02 Aug 2022 17:44:56 GMT  
		Size: 86.0 MB (85961602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a55de22dada9082ec7a3a593b8cd232748af4efcbc59db840905b831b28bf54`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab2e3ad9bf163d68612b159389317d504561ce353dbbf27cccbad037d50594`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d78327ccb2861bccf31add43c64cff76a765bf0b997b06e3738bb08eef2ef9`  
		Last Modified: Tue, 02 Aug 2022 17:44:43 GMT  
		Size: 859.5 KB (859533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc204ca899ea0a81ff2df00810e1f2367f4473436fb8901e4dde42c4f225aff0`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f2f83eeba8861334e02971316a51f87680e6783a18bcd1faa9e88640330733`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 3.3 KB (3310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf6c9a5ae30c1986b673c3e50d9b39a0f3971a7e1c2d01efc816afb4149fd0`  
		Last Modified: Tue, 02 Aug 2022 17:45:02 GMT  
		Size: 113.7 MB (113727907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496e82ba59853989856478c938a72a23dce5951e98090ebf251385616cd463fb`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:b60dcfbbd19ee916cfe82496a0a3ec32704fb02d7ef614a462a8c26b419f33ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231616671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5c514531c3d593534bda4827d79ab938f9b69604af9911b69e50720c9c5a6c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:14:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:14:21 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:14:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:14:35 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:14:37 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:14:42 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:14:44 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:14:46 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:14:50 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 07 Jun 2022 10:14:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 07 Jun 2022 10:14:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 07 Jun 2022 10:15:00 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:15:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:14 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:15:15 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 07 Jun 2022 10:15:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 07 Jun 2022 10:15:36 GMT
ENV HTTP_API=false
# Tue, 07 Jun 2022 10:15:42 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:15:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:15:51 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:15:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331e660ead68d382742f61a8656c41551cb44956552a658c4a7b744bface060`  
		Last Modified: Tue, 07 Jun 2022 10:17:56 GMT  
		Size: 86.6 MB (86607112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a213b14ccc59baf8fae328306aad1c663e545d1071ae41070ca2f4b8407c3ce1`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849223db8c9360d39904a129a16fcab82cc75ed0440f6b216c84181e8eaf3a9d`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cbc038830160e8447b4c94a591d38b99d4212b0cf63674dc8d0512708ccc57`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 831.6 KB (831568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b68ec78a742cf1aa2513ae7a692d0fe38f63e39b8360ae6358423caa08434`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa847ac20a1fea971cba2a4054299001b79527c44c7aee950a97916aa8a7bfb`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a42bd5762b185dffd9c65896d1caace35c218bc37c33dc07dd6f212844fbcb1`  
		Last Modified: Tue, 07 Jun 2022 10:17:49 GMT  
		Size: 113.7 MB (113727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94e67f1cc5eec539069c00057c5a4de04b37c4fd1b7077caca27601fc9b130`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:62920f7249d56ff492ecd65601feca678d819335d76b4cae04dfb0ec2090d6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:1388ad814f4f35bf67df229b9c51eec3bf07ceed47d60e9bc299c9440f61150a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235221886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a04f6ce33e1510259cfe5c41c4375e8860cd6bf9eab5745ba885d600b90cd0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:46:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:46:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:46:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:46:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 18:46:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:46:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:33 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:46:33 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 18:46:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 18:46:43 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 18:46:43 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:44 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec60a66b5ad49a9fc5ae72d2d837c3ead083a79a8cd775cd816ffcd70f66262a`  
		Last Modified: Tue, 02 Aug 2022 18:48:04 GMT  
		Size: 93.8 MB (93846025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48581e1ff3b8c4cc198e8a64401742ad31d1974f84b6787966cc26dcc8f0ce`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad1f5d5e2b55f54ef10f24a0743b24d7acabb3694ba9063fcbabae51b7db121`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483cc6170e8dc85ef8cf416062b65510b66e77cd0a095fca1860fbba19afcaa5`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 930.5 KB (930474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b3f18eb96ef9c253503172278278db98c924179a86195ca8709ad357a672d0`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfacd6f1616f2ee9ac5804a9f2a77020d21adabf4951755fecc916f939cf03f6`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec6677533059e6e25a9e3104dd0244cf6414f60ad33469ed5f5211f591ed151`  
		Last Modified: Tue, 02 Aug 2022 18:47:56 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef62cc2ef2cfab90a2571aa6ca98cd9f41131681af5d812aa2ef10b2745b4d57`  
		Last Modified: Tue, 02 Aug 2022 18:47:49 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c5a0992056eef2b9aeb7b9023169b6561f41058f415ed1c9aaaf0de603e18f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224290844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01446a7647207db9dcef3a6a688fe82790586b7738d010034ee50b9368c9f7ed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:42:42 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:42:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:42:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:42:47 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:42:48 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:42:49 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:42:50 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:42:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:42:52 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 17:42:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 17:42:54 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 17:42:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:42:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:43:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 17:43:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 17:43:09 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 17:43:11 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:43:12 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1ca2ca8943857085e06d4b425c045a8b3ee3a3d7fe89ac23f84d180773b96`  
		Last Modified: Tue, 02 Aug 2022 17:44:56 GMT  
		Size: 86.0 MB (85961602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a55de22dada9082ec7a3a593b8cd232748af4efcbc59db840905b831b28bf54`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab2e3ad9bf163d68612b159389317d504561ce353dbbf27cccbad037d50594`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d78327ccb2861bccf31add43c64cff76a765bf0b997b06e3738bb08eef2ef9`  
		Last Modified: Tue, 02 Aug 2022 17:44:43 GMT  
		Size: 859.5 KB (859533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc204ca899ea0a81ff2df00810e1f2367f4473436fb8901e4dde42c4f225aff0`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f2f83eeba8861334e02971316a51f87680e6783a18bcd1faa9e88640330733`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 3.3 KB (3310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf6c9a5ae30c1986b673c3e50d9b39a0f3971a7e1c2d01efc816afb4149fd0`  
		Last Modified: Tue, 02 Aug 2022 17:45:02 GMT  
		Size: 113.7 MB (113727907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496e82ba59853989856478c938a72a23dce5951e98090ebf251385616cd463fb`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:b60dcfbbd19ee916cfe82496a0a3ec32704fb02d7ef614a462a8c26b419f33ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231616671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5c514531c3d593534bda4827d79ab938f9b69604af9911b69e50720c9c5a6c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:14:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:14:21 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:14:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:14:35 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:14:37 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:14:42 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:14:44 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:14:46 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:14:50 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 07 Jun 2022 10:14:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 07 Jun 2022 10:14:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 07 Jun 2022 10:15:00 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:15:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:14 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:15:15 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 07 Jun 2022 10:15:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 07 Jun 2022 10:15:36 GMT
ENV HTTP_API=false
# Tue, 07 Jun 2022 10:15:42 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:15:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:15:51 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:15:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331e660ead68d382742f61a8656c41551cb44956552a658c4a7b744bface060`  
		Last Modified: Tue, 07 Jun 2022 10:17:56 GMT  
		Size: 86.6 MB (86607112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a213b14ccc59baf8fae328306aad1c663e545d1071ae41070ca2f4b8407c3ce1`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849223db8c9360d39904a129a16fcab82cc75ed0440f6b216c84181e8eaf3a9d`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cbc038830160e8447b4c94a591d38b99d4212b0cf63674dc8d0512708ccc57`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 831.6 KB (831568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b68ec78a742cf1aa2513ae7a692d0fe38f63e39b8360ae6358423caa08434`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa847ac20a1fea971cba2a4054299001b79527c44c7aee950a97916aa8a7bfb`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a42bd5762b185dffd9c65896d1caace35c218bc37c33dc07dd6f212844fbcb1`  
		Last Modified: Tue, 07 Jun 2022 10:17:49 GMT  
		Size: 113.7 MB (113727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94e67f1cc5eec539069c00057c5a4de04b37c4fd1b7077caca27601fc9b130`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:1b28c73bbcde8ad017f3c5f5a0c06bc4edae15eb63135489125002fcf84a3fba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:8ba7080a1dfe944cfa3aef310a80d85721b63bec01b8e828b4efa3720b6eb958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180308041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859da686fb4ba8fbb20e2bfab0b384a8efea93b24a5a7b1671330434e0a3a4a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:13:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:13:19 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:13:20 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:13:21 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:13:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:13:22 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:13:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:13:30 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:13:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:13:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:13:31 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:13:31 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:13:32 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:13:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:13:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6d302c572c7936a2c535df7e3665e4cea12109804d7db2e17c2350483f5c6`  
		Last Modified: Tue, 19 Jul 2022 23:14:04 GMT  
		Size: 60.8 MB (60792590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acef1e43a082930ac2a59ac750fcc44e89eee0d2ee2663ea15276a30a761c112`  
		Last Modified: Tue, 19 Jul 2022 23:13:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753d9cad27595f77612d22db5aff3bf2dd14371b997d3fd09692e97837874620`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59792a17a7735b2bbce017b4e9d56c1eb02cc888a64de33a280730e0c1acc4`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a3b0241dac6de74f098fc124ba52ca8c4950e9b58a750f986190c73b50250b`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f50a37fcc52dae6eaf265933b27d626a5e38dc2eca7b657a3062e4225083d`  
		Last Modified: Tue, 19 Jul 2022 23:14:00 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1095e1b328bb6dfb64e3bc183b9c35afad21a80811146c52cabd8c1251db7`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b14e49b5ca541afa03c868b7617ac3f8bf2dca1217013940b3511bb53ac0fcfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179532890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550d20a8d0a49aaa3f2a866b84e75f0470fc28aa3f2723eabb7f4b7762991f6d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:18:49 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:18:53 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:18:54 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:18:55 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:18:56 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:18:57 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:18:58 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:18:59 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:19:00 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:19:01 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:19:02 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:19:03 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:19:04 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:19:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:07 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:19:09 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:19:20 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:19:21 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:19:22 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:19:23 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:19:24 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:19:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:19:26 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:19:27 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:19:28 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:19:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:19:30 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:19:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:19:32 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:19:34 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:19:34 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:19:35 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:19:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a830a9157109fda713d4c8868452f009b89f5a0aa23e35b64a9fd8ffcbeb248e`  
		Last Modified: Tue, 19 Jul 2022 23:20:35 GMT  
		Size: 60.1 MB (60117412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a219e1f74381cab8fbf4b2158f0e0c8cccf2822e3693f1d8bd13ca27bec084`  
		Last Modified: Tue, 19 Jul 2022 23:20:27 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3153e8cd70c473bb49cd1568765d6399083f8655ace89dcb743660377256711`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448fd19395d15f1dff4ee9d541ee4a4789a87a8902684e4abe9aec78f7c80696`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932c91b8ca10c2ff283945c7998d94267040c160f86b043a84e8a794c4d09a3a`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 3.0 KB (2999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a76d6481ad87c0f65cbd5bf6740c81fbcf6a2b23c530554ec66556c1515ef34`  
		Last Modified: Tue, 19 Jul 2022 23:20:34 GMT  
		Size: 116.7 MB (116688726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdff38d20f7bc060a65e11bf956a87d603ef22aeceda94be739ea3f0f13bd1c`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:6aa40b6458a0b5942abb0cae63ac5d6cd491c5cab4369d5d12de2ebfe3ff2d76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0ae6c2630b8698141ad2b826af32382c0033d6e188becc025982a73e9327d8`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:26:26 GMT
ADD file:fee9d1c50a43d2072ff528133302b3e4d565d1853e14a7d56be9f4532a330841 in / 
# Tue, 19 Jul 2022 22:26:28 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:19:52 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:20:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:20:29 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:20:46 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:20:52 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:20:59 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:21:02 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:21:08 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:21:14 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:21:20 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:21:26 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:21:30 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:21:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:21:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:53 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:21:54 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:22:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:22:25 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:22:40 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:23:01 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:23:07 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:23:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:23:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:23:27 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:23:32 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:23:35 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:23:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:23:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:23:46 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:23:49 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:23:50 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:23:52 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:23:56 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:24:02 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a340aa0651fe455d7a9f4dba0b2b8048ef90ce173a72ac17cf04b9b6af34a2a9`  
		Last Modified: Tue, 19 Jul 2022 22:27:55 GMT  
		Size: 2.8 MB (2811642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0407fa4feb9b7977c80ec2b5ac36e8252a9701c33fb7200fd650a7670fb05bb`  
		Last Modified: Tue, 19 Jul 2022 23:25:13 GMT  
		Size: 56.6 MB (56619857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e50080ba130f5d06da1e2204114d6914f1e86616e352499efccf7b2f91d81f`  
		Last Modified: Tue, 19 Jul 2022 23:25:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74ad31d688802cdd37f41c7f3272a5eb4fd9f2589c0bf3dba4924cc6b7b9eb`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6ab14b03fe37cba7903aa09f0f8d6eb76086d5e0d74230c8816361719fbf8`  
		Last Modified: Tue, 19 Jul 2022 23:25:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665c44209121633da6010cf0aba1f64314d89fca03cd4c667bc331638f17874`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a94295fcd75be4c6ea68c3b2f076d012eec95766121579e8834a5da6806af73`  
		Last Modified: Tue, 19 Jul 2022 23:25:10 GMT  
		Size: 116.7 MB (116690811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2d30730b3cd0901bb65ccabcf1d2e8455dbafb8af1caae6e59207dfc8103d`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:1b28c73bbcde8ad017f3c5f5a0c06bc4edae15eb63135489125002fcf84a3fba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:8ba7080a1dfe944cfa3aef310a80d85721b63bec01b8e828b4efa3720b6eb958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180308041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859da686fb4ba8fbb20e2bfab0b384a8efea93b24a5a7b1671330434e0a3a4a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:13:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:13:19 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:13:20 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:13:21 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:13:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:13:22 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:13:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:13:30 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:13:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:13:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:13:31 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:13:31 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:13:32 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:13:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:13:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6d302c572c7936a2c535df7e3665e4cea12109804d7db2e17c2350483f5c6`  
		Last Modified: Tue, 19 Jul 2022 23:14:04 GMT  
		Size: 60.8 MB (60792590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acef1e43a082930ac2a59ac750fcc44e89eee0d2ee2663ea15276a30a761c112`  
		Last Modified: Tue, 19 Jul 2022 23:13:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753d9cad27595f77612d22db5aff3bf2dd14371b997d3fd09692e97837874620`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59792a17a7735b2bbce017b4e9d56c1eb02cc888a64de33a280730e0c1acc4`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a3b0241dac6de74f098fc124ba52ca8c4950e9b58a750f986190c73b50250b`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f50a37fcc52dae6eaf265933b27d626a5e38dc2eca7b657a3062e4225083d`  
		Last Modified: Tue, 19 Jul 2022 23:14:00 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1095e1b328bb6dfb64e3bc183b9c35afad21a80811146c52cabd8c1251db7`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b14e49b5ca541afa03c868b7617ac3f8bf2dca1217013940b3511bb53ac0fcfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179532890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550d20a8d0a49aaa3f2a866b84e75f0470fc28aa3f2723eabb7f4b7762991f6d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:18:49 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:18:53 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:18:54 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:18:55 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:18:56 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:18:57 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:18:58 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:18:59 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:19:00 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:19:01 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:19:02 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:19:03 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:19:04 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:19:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:07 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:19:09 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:19:20 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:19:21 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:19:22 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:19:23 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:19:24 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:19:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:19:26 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:19:27 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:19:28 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:19:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:19:30 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:19:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:19:32 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:19:34 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:19:34 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:19:35 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:19:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a830a9157109fda713d4c8868452f009b89f5a0aa23e35b64a9fd8ffcbeb248e`  
		Last Modified: Tue, 19 Jul 2022 23:20:35 GMT  
		Size: 60.1 MB (60117412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a219e1f74381cab8fbf4b2158f0e0c8cccf2822e3693f1d8bd13ca27bec084`  
		Last Modified: Tue, 19 Jul 2022 23:20:27 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3153e8cd70c473bb49cd1568765d6399083f8655ace89dcb743660377256711`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448fd19395d15f1dff4ee9d541ee4a4789a87a8902684e4abe9aec78f7c80696`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932c91b8ca10c2ff283945c7998d94267040c160f86b043a84e8a794c4d09a3a`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 3.0 KB (2999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a76d6481ad87c0f65cbd5bf6740c81fbcf6a2b23c530554ec66556c1515ef34`  
		Last Modified: Tue, 19 Jul 2022 23:20:34 GMT  
		Size: 116.7 MB (116688726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdff38d20f7bc060a65e11bf956a87d603ef22aeceda94be739ea3f0f13bd1c`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:6aa40b6458a0b5942abb0cae63ac5d6cd491c5cab4369d5d12de2ebfe3ff2d76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0ae6c2630b8698141ad2b826af32382c0033d6e188becc025982a73e9327d8`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:26:26 GMT
ADD file:fee9d1c50a43d2072ff528133302b3e4d565d1853e14a7d56be9f4532a330841 in / 
# Tue, 19 Jul 2022 22:26:28 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:19:52 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:20:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:20:29 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:20:46 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:20:52 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:20:59 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:21:02 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:21:08 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:21:14 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:21:20 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:21:26 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:21:30 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:21:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:21:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:53 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:21:54 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:22:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:22:25 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:22:40 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:23:01 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:23:07 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:23:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:23:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:23:27 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:23:32 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:23:35 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:23:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:23:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:23:46 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:23:49 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:23:50 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:23:52 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:23:56 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:24:02 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a340aa0651fe455d7a9f4dba0b2b8048ef90ce173a72ac17cf04b9b6af34a2a9`  
		Last Modified: Tue, 19 Jul 2022 22:27:55 GMT  
		Size: 2.8 MB (2811642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0407fa4feb9b7977c80ec2b5ac36e8252a9701c33fb7200fd650a7670fb05bb`  
		Last Modified: Tue, 19 Jul 2022 23:25:13 GMT  
		Size: 56.6 MB (56619857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e50080ba130f5d06da1e2204114d6914f1e86616e352499efccf7b2f91d81f`  
		Last Modified: Tue, 19 Jul 2022 23:25:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74ad31d688802cdd37f41c7f3272a5eb4fd9f2589c0bf3dba4924cc6b7b9eb`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6ab14b03fe37cba7903aa09f0f8d6eb76086d5e0d74230c8816361719fbf8`  
		Last Modified: Tue, 19 Jul 2022 23:25:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665c44209121633da6010cf0aba1f64314d89fca03cd4c667bc331638f17874`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a94295fcd75be4c6ea68c3b2f076d012eec95766121579e8834a5da6806af73`  
		Last Modified: Tue, 19 Jul 2022 23:25:10 GMT  
		Size: 116.7 MB (116690811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2d30730b3cd0901bb65ccabcf1d2e8455dbafb8af1caae6e59207dfc8103d`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:2aa1c31852ada047773e8162bf4ffa9477d68a981870819729ece391dc8b12b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:02c25843148941a2b16711ab605ab4952d7c1852901981edc10a50c92dbdd132
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.4 MB (234418320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06915655aba02e781626a3b39e648d7a1b9501a76f1efb8206eacdd938a4fad0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:45:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:45:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:45:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:45:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:45:32 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 02 Aug 2022 18:45:32 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 02 Aug 2022 18:45:32 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 18:45:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:45:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 18:45:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 18:45:34 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:45:34 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 02 Aug 2022 18:45:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 02 Aug 2022 18:45:42 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 18:45:43 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 18:45:43 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:45:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:45:43 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:45:43 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d50e772b503a53e97f96f1c7602b04e6dee66044b4115a656657015cc8dd0b7`  
		Last Modified: Tue, 02 Aug 2022 18:47:21 GMT  
		Size: 93.8 MB (93843076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26eb43ae80cdb0d32344078dcc9a34e5168ec38544ca6ec2d6a570c0bd22c8`  
		Last Modified: Tue, 02 Aug 2022 18:47:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60cd03e6c4f2bb07959adeb37f665329f44d70461b01bb7e4a7f2e4a33c361`  
		Last Modified: Tue, 02 Aug 2022 18:47:08 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baeb6788537273b4b4ea7b4ca7add2abb8b81aca7a21c8f20cb5c658d097fe`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 506.4 KB (506350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed2d1cc863c23ea8586d2c6539c20cc81c2eb1902d1828f21e31596ca0d0805`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0866043632c88df795dcadb6becec0ed8033f63e8beac4c2e8efab3dfd1baa`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 6.9 KB (6896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5867343bf3768ae661845f5c164588dd7cd33b40c66447517199c6ff8ff18b59`  
		Last Modified: Tue, 02 Aug 2022 18:47:11 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0818f06db5477f06b6fa1c112b1c9f90ab1feb76255549f24602e506ac70337`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e8a118dff4de791d93f6c11e94b08c9a1164d7181f64c797acf2d91de067a090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223530644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:646571e35ae1a4d11e8d547c9a5860e82aefbca8adddfea403ef44603cbac11c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:41:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:41:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:41:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:41:17 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:41:17 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:41:18 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:41:19 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:41:20 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:41:21 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 02 Aug 2022 17:41:22 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 02 Aug 2022 17:41:23 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 17:41:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:41:25 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 17:41:26 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 17:41:27 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:41:29 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 02 Aug 2022 17:41:33 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 02 Aug 2022 17:41:35 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 17:41:36 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 17:41:36 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:41:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:41:38 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:41:39 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439589d8fce29b6ddaeaa0d2c2fb68eb16c9f8135829466ddf899922c2c78488`  
		Last Modified: Tue, 02 Aug 2022 17:44:08 GMT  
		Size: 86.0 MB (85961696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca434dad4975c4402f953151563ec4581df90bd8b9f4e3bd670e8fd614ff4b4`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a53a5b66d93db8abb050b7d143e86ef10bae890206b1365d673172628f9e1`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8d82da748df549da0b2ede71952a9099c9ee290d5c22dc38ba1e76b34d2b0`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 475.8 KB (475760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50631eb49c8f19312feae82197b8c84c7acda252a4d27c2ee52deb5531d3cc`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03f352bba50f5659567c93213547f0571de628a75a84ffd8ff6d7cc7806fd98`  
		Last Modified: Tue, 02 Aug 2022 17:43:53 GMT  
		Size: 6.9 KB (6867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6320208c13dc7f0655e4ee6d692280f7cabac4e50f1edb8f7243d23813baaf6`  
		Last Modified: Tue, 02 Aug 2022 17:44:00 GMT  
		Size: 113.3 MB (113347829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cde75c267c8cce58f6c22396d464208efe6533f6ffe92f17cfe14954b72b00`  
		Last Modified: Tue, 02 Aug 2022 17:43:53 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:42015c88f159169c44924f419d339b2b7808e0de3efda20d6b518f7abd57b64a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230883546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb1beed798a8424e06ab63bfa05049f88aa24104bad94ab900a6a86c5487b29f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:08:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:08:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:08:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:08:42 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:08:44 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:08:50 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:08:53 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:08:59 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 07 Jun 2022 10:09:02 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 07 Jun 2022 10:09:05 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 07 Jun 2022 10:09:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:09:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 07 Jun 2022 10:09:18 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 07 Jun 2022 10:09:24 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:09:27 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 07 Jun 2022 10:09:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 07 Jun 2022 10:09:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 07 Jun 2022 10:09:56 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 07 Jun 2022 10:09:59 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:10:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:10:03 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:10:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932cab289b2b2a387d18cfb709811f1a652f05e78ced57c596e0e3a7136ca8f`  
		Last Modified: Tue, 07 Jun 2022 10:16:56 GMT  
		Size: 86.6 MB (86606720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99318a085a88c3b7eefb71e0fb1851bbc6f00b8b9b350cd5f611e0e3294356`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128478c35447ca89ff14fbf5c1a1a2936a18e0012a7f08f2db12e421b6d46159`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4873185aa919a50c4fad4b47828805af6df63bc92c8143b5268a777fade09b6`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 475.3 KB (475347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc9dd2be22b30ab96107306d3decb7df1bdafed73b547ca9f50c89681528132`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acd8f5bfe97b576b0d76542fe23769024f6342f29204f006a93e252577d91ff`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 6.9 KB (6896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555aab78bd51927009b5cff45506381876e0d93e3f958331eb0bf1aafe16b35f`  
		Last Modified: Tue, 07 Jun 2022 10:16:47 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bf4efa22c46743f8d6a52f1c7f11ff4c18a9682323e302959e76679447be74`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:2aa1c31852ada047773e8162bf4ffa9477d68a981870819729ece391dc8b12b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:02c25843148941a2b16711ab605ab4952d7c1852901981edc10a50c92dbdd132
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.4 MB (234418320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06915655aba02e781626a3b39e648d7a1b9501a76f1efb8206eacdd938a4fad0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:45:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:45:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:45:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:45:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:45:32 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 02 Aug 2022 18:45:32 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 02 Aug 2022 18:45:32 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 18:45:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:45:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 18:45:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 18:45:34 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:45:34 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 02 Aug 2022 18:45:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 02 Aug 2022 18:45:42 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 18:45:43 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 18:45:43 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:45:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:45:43 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:45:43 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d50e772b503a53e97f96f1c7602b04e6dee66044b4115a656657015cc8dd0b7`  
		Last Modified: Tue, 02 Aug 2022 18:47:21 GMT  
		Size: 93.8 MB (93843076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26eb43ae80cdb0d32344078dcc9a34e5168ec38544ca6ec2d6a570c0bd22c8`  
		Last Modified: Tue, 02 Aug 2022 18:47:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60cd03e6c4f2bb07959adeb37f665329f44d70461b01bb7e4a7f2e4a33c361`  
		Last Modified: Tue, 02 Aug 2022 18:47:08 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baeb6788537273b4b4ea7b4ca7add2abb8b81aca7a21c8f20cb5c658d097fe`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 506.4 KB (506350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed2d1cc863c23ea8586d2c6539c20cc81c2eb1902d1828f21e31596ca0d0805`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0866043632c88df795dcadb6becec0ed8033f63e8beac4c2e8efab3dfd1baa`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 6.9 KB (6896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5867343bf3768ae661845f5c164588dd7cd33b40c66447517199c6ff8ff18b59`  
		Last Modified: Tue, 02 Aug 2022 18:47:11 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0818f06db5477f06b6fa1c112b1c9f90ab1feb76255549f24602e506ac70337`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e8a118dff4de791d93f6c11e94b08c9a1164d7181f64c797acf2d91de067a090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.5 MB (223530644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:646571e35ae1a4d11e8d547c9a5860e82aefbca8adddfea403ef44603cbac11c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:41:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:41:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:41:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:41:17 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:41:17 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:41:18 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:41:19 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:41:20 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:41:21 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 02 Aug 2022 17:41:22 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 02 Aug 2022 17:41:23 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 17:41:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:41:25 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 02 Aug 2022 17:41:26 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 17:41:27 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:41:29 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 02 Aug 2022 17:41:33 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 02 Aug 2022 17:41:35 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 17:41:36 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 17:41:36 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:41:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:41:38 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:41:39 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439589d8fce29b6ddaeaa0d2c2fb68eb16c9f8135829466ddf899922c2c78488`  
		Last Modified: Tue, 02 Aug 2022 17:44:08 GMT  
		Size: 86.0 MB (85961696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca434dad4975c4402f953151563ec4581df90bd8b9f4e3bd670e8fd614ff4b4`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a53a5b66d93db8abb050b7d143e86ef10bae890206b1365d673172628f9e1`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8d82da748df549da0b2ede71952a9099c9ee290d5c22dc38ba1e76b34d2b0`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 475.8 KB (475760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50631eb49c8f19312feae82197b8c84c7acda252a4d27c2ee52deb5531d3cc`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03f352bba50f5659567c93213547f0571de628a75a84ffd8ff6d7cc7806fd98`  
		Last Modified: Tue, 02 Aug 2022 17:43:53 GMT  
		Size: 6.9 KB (6867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6320208c13dc7f0655e4ee6d692280f7cabac4e50f1edb8f7243d23813baaf6`  
		Last Modified: Tue, 02 Aug 2022 17:44:00 GMT  
		Size: 113.3 MB (113347829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cde75c267c8cce58f6c22396d464208efe6533f6ffe92f17cfe14954b72b00`  
		Last Modified: Tue, 02 Aug 2022 17:43:53 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:42015c88f159169c44924f419d339b2b7808e0de3efda20d6b518f7abd57b64a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230883546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb1beed798a8424e06ab63bfa05049f88aa24104bad94ab900a6a86c5487b29f`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:08:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:08:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:08:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:08:42 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:08:44 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:08:50 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:08:53 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:08:59 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 07 Jun 2022 10:09:02 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 07 Jun 2022 10:09:05 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 07 Jun 2022 10:09:08 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:09:11 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 07 Jun 2022 10:09:18 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 07 Jun 2022 10:09:24 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:09:27 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 07 Jun 2022 10:09:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 07 Jun 2022 10:09:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 07 Jun 2022 10:09:56 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 07 Jun 2022 10:09:59 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:10:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:10:03 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:10:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932cab289b2b2a387d18cfb709811f1a652f05e78ced57c596e0e3a7136ca8f`  
		Last Modified: Tue, 07 Jun 2022 10:16:56 GMT  
		Size: 86.6 MB (86606720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99318a085a88c3b7eefb71e0fb1851bbc6f00b8b9b350cd5f611e0e3294356`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128478c35447ca89ff14fbf5c1a1a2936a18e0012a7f08f2db12e421b6d46159`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4873185aa919a50c4fad4b47828805af6df63bc92c8143b5268a777fade09b6`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 475.3 KB (475347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc9dd2be22b30ab96107306d3decb7df1bdafed73b547ca9f50c89681528132`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acd8f5bfe97b576b0d76542fe23769024f6342f29204f006a93e252577d91ff`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 6.9 KB (6896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555aab78bd51927009b5cff45506381876e0d93e3f958331eb0bf1aafe16b35f`  
		Last Modified: Tue, 07 Jun 2022 10:16:47 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bf4efa22c46743f8d6a52f1c7f11ff4c18a9682323e302959e76679447be74`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:8de9c856224a7306e8ac7b5d8e65a8d97bef3a7c8527f3a1f4407c9b45381d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:4c28435d9e29513ff0f7daecfec61544df34fa974e831e25f931c60d73940ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.5 MB (237485947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6cc15457b62c1ba8644edcb7278542a9f91ee4c2e6f59e0453a0b97647f392`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:45:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:45:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:45:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:45:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 02 Aug 2022 18:45:51 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 18:45:52 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 18:45:53 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:45:53 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 02 Aug 2022 18:45:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 02 Aug 2022 18:46:00 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 18:46:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 18:46:01 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:02 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d50e772b503a53e97f96f1c7602b04e6dee66044b4115a656657015cc8dd0b7`  
		Last Modified: Tue, 02 Aug 2022 18:47:21 GMT  
		Size: 93.8 MB (93843076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26eb43ae80cdb0d32344078dcc9a34e5168ec38544ca6ec2d6a570c0bd22c8`  
		Last Modified: Tue, 02 Aug 2022 18:47:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60cd03e6c4f2bb07959adeb37f665329f44d70461b01bb7e4a7f2e4a33c361`  
		Last Modified: Tue, 02 Aug 2022 18:47:08 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baeb6788537273b4b4ea7b4ca7add2abb8b81aca7a21c8f20cb5c658d097fe`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 506.4 KB (506350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139969e8126173a3227b1abe266a8119550d2a8bbb2d1a65c3ffe36da819411`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ca1df3999ff9027299abbcb37e390c0e998fedf8167460080fa1458573f53`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95336ada909617a31482b70af8d5f5e51498eb4e30afa6cbae66ca5e0049968`  
		Last Modified: Tue, 02 Aug 2022 18:47:37 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed438aef59d48263abab0591f1e5f4be92ead54ccb43b8c1c57c1b5facec9769`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7ab361015ccf742c9808e14ce5c2ab028dbfb1bad421c6795bcb5fdae34952d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226598269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30a614d1db72283c5a882db79ce17c54eb505b86100630ee7af353c98f25c4a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:41:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:41:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:41:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:41:17 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:41:17 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:41:47 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:41:48 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:41:49 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:41:50 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:41:51 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 02 Aug 2022 17:41:52 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 02 Aug 2022 17:41:53 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 02 Aug 2022 17:41:54 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 17:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:41:56 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 17:41:57 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 17:41:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:42:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 02 Aug 2022 17:42:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 02 Aug 2022 17:42:06 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 17:42:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 17:42:08 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:42:10 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:42:10 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:42:11 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439589d8fce29b6ddaeaa0d2c2fb68eb16c9f8135829466ddf899922c2c78488`  
		Last Modified: Tue, 02 Aug 2022 17:44:08 GMT  
		Size: 86.0 MB (85961696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca434dad4975c4402f953151563ec4581df90bd8b9f4e3bd670e8fd614ff4b4`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a53a5b66d93db8abb050b7d143e86ef10bae890206b1365d673172628f9e1`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8d82da748df549da0b2ede71952a9099c9ee290d5c22dc38ba1e76b34d2b0`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 475.8 KB (475760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f5e764b86512346f24b36dc95ba83759a1899e2a9b045ee3ec06489ba8f86`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a0280f786f1176a696f1de7847cb62d4bc218e1f5af961737ccf4f5d1d8b1b`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 6.9 KB (6917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6cdcd42d0bf3bf3ef933054227953a11e8579bdad50c64499c65b79a8a5f3c`  
		Last Modified: Tue, 02 Aug 2022 17:44:27 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1677b323555e6b1285259ac735523908155d92868b55464a79dd6d0f5489056`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:b56b3ae5fd5e336c93594767ecae7a32026f87bf5ffd09a13f55c8d45123f978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233951178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9fec1db19fcffd6ebef6c9cae4f880271ccbbfa9600fc7146eeb41f40158d6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:08:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:08:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:08:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:08:42 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:10:29 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:10:30 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:10:32 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:10:35 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:10:38 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 07 Jun 2022 10:10:41 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 07 Jun 2022 10:10:44 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 07 Jun 2022 10:10:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 07 Jun 2022 10:10:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:10:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 07 Jun 2022 10:10:55 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 07 Jun 2022 10:11:01 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:11:02 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 07 Jun 2022 10:11:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 07 Jun 2022 10:11:19 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 07 Jun 2022 10:11:26 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 07 Jun 2022 10:11:30 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:11:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:11:33 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:11:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932cab289b2b2a387d18cfb709811f1a652f05e78ced57c596e0e3a7136ca8f`  
		Last Modified: Tue, 07 Jun 2022 10:16:56 GMT  
		Size: 86.6 MB (86606720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99318a085a88c3b7eefb71e0fb1851bbc6f00b8b9b350cd5f611e0e3294356`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128478c35447ca89ff14fbf5c1a1a2936a18e0012a7f08f2db12e421b6d46159`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4873185aa919a50c4fad4b47828805af6df63bc92c8143b5268a777fade09b6`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 475.3 KB (475347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eceaedc2b9083c2b4baf061ec3fad71b09f51e83d5e7ae2b07aa70e01bc60d3`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba561c4766c632072d54ee899d6956320cc379ead197e70321d06a5936402f0c`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b5afedaeef8dad41a823655dbe702900e9f84fbb2f98bbf9f560534a33c0c9`  
		Last Modified: Tue, 07 Jun 2022 10:17:22 GMT  
		Size: 116.4 MB (116415403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56f59b30a77def4359279676b77dc14e03c625eb67a39ae191af44d2125d0f`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:8de9c856224a7306e8ac7b5d8e65a8d97bef3a7c8527f3a1f4407c9b45381d62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:4c28435d9e29513ff0f7daecfec61544df34fa974e831e25f931c60d73940ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.5 MB (237485947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6cc15457b62c1ba8644edcb7278542a9f91ee4c2e6f59e0453a0b97647f392`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:45:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:45:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:45:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:45:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:45:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:45:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 02 Aug 2022 18:45:51 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:45:51 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 18:45:52 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 18:45:53 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:45:53 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 02 Aug 2022 18:45:59 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 02 Aug 2022 18:46:00 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 18:46:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 18:46:01 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:02 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d50e772b503a53e97f96f1c7602b04e6dee66044b4115a656657015cc8dd0b7`  
		Last Modified: Tue, 02 Aug 2022 18:47:21 GMT  
		Size: 93.8 MB (93843076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad26eb43ae80cdb0d32344078dcc9a34e5168ec38544ca6ec2d6a570c0bd22c8`  
		Last Modified: Tue, 02 Aug 2022 18:47:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60cd03e6c4f2bb07959adeb37f665329f44d70461b01bb7e4a7f2e4a33c361`  
		Last Modified: Tue, 02 Aug 2022 18:47:08 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3baeb6788537273b4b4ea7b4ca7add2abb8b81aca7a21c8f20cb5c658d097fe`  
		Last Modified: Tue, 02 Aug 2022 18:47:06 GMT  
		Size: 506.4 KB (506350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139969e8126173a3227b1abe266a8119550d2a8bbb2d1a65c3ffe36da819411`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ca1df3999ff9027299abbcb37e390c0e998fedf8167460080fa1458573f53`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95336ada909617a31482b70af8d5f5e51498eb4e30afa6cbae66ca5e0049968`  
		Last Modified: Tue, 02 Aug 2022 18:47:37 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed438aef59d48263abab0591f1e5f4be92ead54ccb43b8c1c57c1b5facec9769`  
		Last Modified: Tue, 02 Aug 2022 18:47:31 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:7ab361015ccf742c9808e14ce5c2ab028dbfb1bad421c6795bcb5fdae34952d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226598269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30a614d1db72283c5a882db79ce17c54eb505b86100630ee7af353c98f25c4a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:41:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:41:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:41:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:41:17 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:41:17 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:41:47 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:41:48 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:41:49 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:41:50 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:41:51 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 02 Aug 2022 17:41:52 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 02 Aug 2022 17:41:53 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 02 Aug 2022 17:41:54 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 17:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:41:56 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 02 Aug 2022 17:41:57 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 02 Aug 2022 17:41:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:42:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 02 Aug 2022 17:42:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 02 Aug 2022 17:42:06 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 02 Aug 2022 17:42:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 02 Aug 2022 17:42:08 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:42:10 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:42:10 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:42:11 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439589d8fce29b6ddaeaa0d2c2fb68eb16c9f8135829466ddf899922c2c78488`  
		Last Modified: Tue, 02 Aug 2022 17:44:08 GMT  
		Size: 86.0 MB (85961696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca434dad4975c4402f953151563ec4581df90bd8b9f4e3bd670e8fd614ff4b4`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a53a5b66d93db8abb050b7d143e86ef10bae890206b1365d673172628f9e1`  
		Last Modified: Tue, 02 Aug 2022 17:43:56 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8d82da748df549da0b2ede71952a9099c9ee290d5c22dc38ba1e76b34d2b0`  
		Last Modified: Tue, 02 Aug 2022 17:43:54 GMT  
		Size: 475.8 KB (475760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f5e764b86512346f24b36dc95ba83759a1899e2a9b045ee3ec06489ba8f86`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a0280f786f1176a696f1de7847cb62d4bc218e1f5af961737ccf4f5d1d8b1b`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 6.9 KB (6917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6cdcd42d0bf3bf3ef933054227953a11e8579bdad50c64499c65b79a8a5f3c`  
		Last Modified: Tue, 02 Aug 2022 17:44:27 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1677b323555e6b1285259ac735523908155d92868b55464a79dd6d0f5489056`  
		Last Modified: Tue, 02 Aug 2022 17:44:20 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:b56b3ae5fd5e336c93594767ecae7a32026f87bf5ffd09a13f55c8d45123f978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233951178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9fec1db19fcffd6ebef6c9cae4f880271ccbbfa9600fc7146eeb41f40158d6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:08:18 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:08:26 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:08:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:08:42 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:10:29 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:10:30 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:10:32 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:10:35 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:10:38 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 07 Jun 2022 10:10:41 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 07 Jun 2022 10:10:44 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 07 Jun 2022 10:10:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 07 Jun 2022 10:10:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:10:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 07 Jun 2022 10:10:55 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 07 Jun 2022 10:11:01 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:11:02 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 07 Jun 2022 10:11:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 07 Jun 2022 10:11:19 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 07 Jun 2022 10:11:26 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 07 Jun 2022 10:11:30 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:11:31 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:11:33 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:11:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932cab289b2b2a387d18cfb709811f1a652f05e78ced57c596e0e3a7136ca8f`  
		Last Modified: Tue, 07 Jun 2022 10:16:56 GMT  
		Size: 86.6 MB (86606720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99318a085a88c3b7eefb71e0fb1851bbc6f00b8b9b350cd5f611e0e3294356`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128478c35447ca89ff14fbf5c1a1a2936a18e0012a7f08f2db12e421b6d46159`  
		Last Modified: Tue, 07 Jun 2022 10:16:42 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4873185aa919a50c4fad4b47828805af6df63bc92c8143b5268a777fade09b6`  
		Last Modified: Tue, 07 Jun 2022 10:16:39 GMT  
		Size: 475.3 KB (475347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eceaedc2b9083c2b4baf061ec3fad71b09f51e83d5e7ae2b07aa70e01bc60d3`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba561c4766c632072d54ee899d6956320cc379ead197e70321d06a5936402f0c`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b5afedaeef8dad41a823655dbe702900e9f84fbb2f98bbf9f560534a33c0c9`  
		Last Modified: Tue, 07 Jun 2022 10:17:22 GMT  
		Size: 116.4 MB (116415403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56f59b30a77def4359279676b77dc14e03c625eb67a39ae191af44d2125d0f`  
		Last Modified: Tue, 07 Jun 2022 10:17:09 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:62920f7249d56ff492ecd65601feca678d819335d76b4cae04dfb0ec2090d6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:1388ad814f4f35bf67df229b9c51eec3bf07ceed47d60e9bc299c9440f61150a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235221886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a04f6ce33e1510259cfe5c41c4375e8860cd6bf9eab5745ba885d600b90cd0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:46:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:46:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:46:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:46:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 18:46:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:46:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:33 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:46:33 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 18:46:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 18:46:43 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 18:46:43 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:44 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec60a66b5ad49a9fc5ae72d2d837c3ead083a79a8cd775cd816ffcd70f66262a`  
		Last Modified: Tue, 02 Aug 2022 18:48:04 GMT  
		Size: 93.8 MB (93846025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48581e1ff3b8c4cc198e8a64401742ad31d1974f84b6787966cc26dcc8f0ce`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad1f5d5e2b55f54ef10f24a0743b24d7acabb3694ba9063fcbabae51b7db121`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483cc6170e8dc85ef8cf416062b65510b66e77cd0a095fca1860fbba19afcaa5`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 930.5 KB (930474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b3f18eb96ef9c253503172278278db98c924179a86195ca8709ad357a672d0`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfacd6f1616f2ee9ac5804a9f2a77020d21adabf4951755fecc916f939cf03f6`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec6677533059e6e25a9e3104dd0244cf6414f60ad33469ed5f5211f591ed151`  
		Last Modified: Tue, 02 Aug 2022 18:47:56 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef62cc2ef2cfab90a2571aa6ca98cd9f41131681af5d812aa2ef10b2745b4d57`  
		Last Modified: Tue, 02 Aug 2022 18:47:49 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c5a0992056eef2b9aeb7b9023169b6561f41058f415ed1c9aaaf0de603e18f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224290844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01446a7647207db9dcef3a6a688fe82790586b7738d010034ee50b9368c9f7ed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:42:42 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:42:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:42:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:42:47 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:42:48 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:42:49 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:42:50 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:42:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:42:52 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 17:42:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 17:42:54 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 17:42:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:42:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:43:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 17:43:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 17:43:09 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 17:43:11 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:43:12 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1ca2ca8943857085e06d4b425c045a8b3ee3a3d7fe89ac23f84d180773b96`  
		Last Modified: Tue, 02 Aug 2022 17:44:56 GMT  
		Size: 86.0 MB (85961602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a55de22dada9082ec7a3a593b8cd232748af4efcbc59db840905b831b28bf54`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab2e3ad9bf163d68612b159389317d504561ce353dbbf27cccbad037d50594`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d78327ccb2861bccf31add43c64cff76a765bf0b997b06e3738bb08eef2ef9`  
		Last Modified: Tue, 02 Aug 2022 17:44:43 GMT  
		Size: 859.5 KB (859533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc204ca899ea0a81ff2df00810e1f2367f4473436fb8901e4dde42c4f225aff0`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f2f83eeba8861334e02971316a51f87680e6783a18bcd1faa9e88640330733`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 3.3 KB (3310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf6c9a5ae30c1986b673c3e50d9b39a0f3971a7e1c2d01efc816afb4149fd0`  
		Last Modified: Tue, 02 Aug 2022 17:45:02 GMT  
		Size: 113.7 MB (113727907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496e82ba59853989856478c938a72a23dce5951e98090ebf251385616cd463fb`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:b60dcfbbd19ee916cfe82496a0a3ec32704fb02d7ef614a462a8c26b419f33ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231616671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5c514531c3d593534bda4827d79ab938f9b69604af9911b69e50720c9c5a6c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:14:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:14:21 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:14:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:14:35 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:14:37 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:14:42 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:14:44 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:14:46 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:14:50 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 07 Jun 2022 10:14:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 07 Jun 2022 10:14:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 07 Jun 2022 10:15:00 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:15:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:14 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:15:15 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 07 Jun 2022 10:15:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 07 Jun 2022 10:15:36 GMT
ENV HTTP_API=false
# Tue, 07 Jun 2022 10:15:42 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:15:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:15:51 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:15:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331e660ead68d382742f61a8656c41551cb44956552a658c4a7b744bface060`  
		Last Modified: Tue, 07 Jun 2022 10:17:56 GMT  
		Size: 86.6 MB (86607112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a213b14ccc59baf8fae328306aad1c663e545d1071ae41070ca2f4b8407c3ce1`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849223db8c9360d39904a129a16fcab82cc75ed0440f6b216c84181e8eaf3a9d`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cbc038830160e8447b4c94a591d38b99d4212b0cf63674dc8d0512708ccc57`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 831.6 KB (831568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b68ec78a742cf1aa2513ae7a692d0fe38f63e39b8360ae6358423caa08434`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa847ac20a1fea971cba2a4054299001b79527c44c7aee950a97916aa8a7bfb`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a42bd5762b185dffd9c65896d1caace35c218bc37c33dc07dd6f212844fbcb1`  
		Last Modified: Tue, 07 Jun 2022 10:17:49 GMT  
		Size: 113.7 MB (113727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94e67f1cc5eec539069c00057c5a4de04b37c4fd1b7077caca27601fc9b130`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:62920f7249d56ff492ecd65601feca678d819335d76b4cae04dfb0ec2090d6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:1388ad814f4f35bf67df229b9c51eec3bf07ceed47d60e9bc299c9440f61150a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235221886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a04f6ce33e1510259cfe5c41c4375e8860cd6bf9eab5745ba885d600b90cd0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 18:43:42 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 18:46:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 18:46:28 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 18:46:29 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 18:46:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 18:46:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 18:46:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 18:46:33 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 18:46:33 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 18:46:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 18:46:43 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 18:46:43 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 18:46:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 18:46:44 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 18:46:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec60a66b5ad49a9fc5ae72d2d837c3ead083a79a8cd775cd816ffcd70f66262a`  
		Last Modified: Tue, 02 Aug 2022 18:48:04 GMT  
		Size: 93.8 MB (93846025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48581e1ff3b8c4cc198e8a64401742ad31d1974f84b6787966cc26dcc8f0ce`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad1f5d5e2b55f54ef10f24a0743b24d7acabb3694ba9063fcbabae51b7db121`  
		Last Modified: Tue, 02 Aug 2022 18:47:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483cc6170e8dc85ef8cf416062b65510b66e77cd0a095fca1860fbba19afcaa5`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 930.5 KB (930474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b3f18eb96ef9c253503172278278db98c924179a86195ca8709ad357a672d0`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfacd6f1616f2ee9ac5804a9f2a77020d21adabf4951755fecc916f939cf03f6`  
		Last Modified: Tue, 02 Aug 2022 18:47:50 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec6677533059e6e25a9e3104dd0244cf6414f60ad33469ed5f5211f591ed151`  
		Last Modified: Tue, 02 Aug 2022 18:47:56 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef62cc2ef2cfab90a2571aa6ca98cd9f41131681af5d812aa2ef10b2745b4d57`  
		Last Modified: Tue, 02 Aug 2022 18:47:49 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c5a0992056eef2b9aeb7b9023169b6561f41058f415ed1c9aaaf0de603e18f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224290844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01446a7647207db9dcef3a6a688fe82790586b7738d010034ee50b9368c9f7ed`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:40:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 02 Aug 2022 17:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:42:42 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 02 Aug 2022 17:42:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 02 Aug 2022 17:42:46 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 02 Aug 2022 17:42:47 GMT
ARG BONITA_VERSION
# Tue, 02 Aug 2022 17:42:48 GMT
ARG BRANDING_VERSION
# Tue, 02 Aug 2022 17:42:49 GMT
ARG BONITA_SHA256
# Tue, 02 Aug 2022 17:42:50 GMT
ARG BASE_URL
# Tue, 02 Aug 2022 17:42:51 GMT
ARG BONITA_URL
# Tue, 02 Aug 2022 17:42:52 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 02 Aug 2022 17:42:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 02 Aug 2022 17:42:54 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 02 Aug 2022 17:42:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 02 Aug 2022 17:42:57 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 02 Aug 2022 17:42:58 GMT
RUN mkdir /opt/files
# Tue, 02 Aug 2022 17:43:00 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 02 Aug 2022 17:43:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 02 Aug 2022 17:43:09 GMT
ENV HTTP_API=false
# Tue, 02 Aug 2022 17:43:11 GMT
VOLUME [/opt/bonita]
# Tue, 02 Aug 2022 17:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 02 Aug 2022 17:43:12 GMT
EXPOSE 8080
# Tue, 02 Aug 2022 17:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1ca2ca8943857085e06d4b425c045a8b3ee3a3d7fe89ac23f84d180773b96`  
		Last Modified: Tue, 02 Aug 2022 17:44:56 GMT  
		Size: 86.0 MB (85961602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a55de22dada9082ec7a3a593b8cd232748af4efcbc59db840905b831b28bf54`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab2e3ad9bf163d68612b159389317d504561ce353dbbf27cccbad037d50594`  
		Last Modified: Tue, 02 Aug 2022 17:44:45 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d78327ccb2861bccf31add43c64cff76a765bf0b997b06e3738bb08eef2ef9`  
		Last Modified: Tue, 02 Aug 2022 17:44:43 GMT  
		Size: 859.5 KB (859533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc204ca899ea0a81ff2df00810e1f2367f4473436fb8901e4dde42c4f225aff0`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f2f83eeba8861334e02971316a51f87680e6783a18bcd1faa9e88640330733`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 3.3 KB (3310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf6c9a5ae30c1986b673c3e50d9b39a0f3971a7e1c2d01efc816afb4149fd0`  
		Last Modified: Tue, 02 Aug 2022 17:45:02 GMT  
		Size: 113.7 MB (113727907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496e82ba59853989856478c938a72a23dce5951e98090ebf251385616cd463fb`  
		Last Modified: Tue, 02 Aug 2022 17:44:42 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:b60dcfbbd19ee916cfe82496a0a3ec32704fb02d7ef614a462a8c26b419f33ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231616671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5c514531c3d593534bda4827d79ab938f9b69604af9911b69e50720c9c5a6c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:06:17 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 07 Jun 2022 10:14:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 07 Jun 2022 10:14:21 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 07 Jun 2022 10:14:32 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 07 Jun 2022 10:14:35 GMT
ARG BONITA_VERSION
# Tue, 07 Jun 2022 10:14:37 GMT
ARG BRANDING_VERSION
# Tue, 07 Jun 2022 10:14:42 GMT
ARG BONITA_SHA256
# Tue, 07 Jun 2022 10:14:44 GMT
ARG BASE_URL
# Tue, 07 Jun 2022 10:14:46 GMT
ARG BONITA_URL
# Tue, 07 Jun 2022 10:14:50 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 07 Jun 2022 10:14:53 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 07 Jun 2022 10:14:57 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 07 Jun 2022 10:15:00 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 07 Jun 2022 10:15:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 07 Jun 2022 10:15:14 GMT
RUN mkdir /opt/files
# Tue, 07 Jun 2022 10:15:15 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 07 Jun 2022 10:15:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 07 Jun 2022 10:15:36 GMT
ENV HTTP_API=false
# Tue, 07 Jun 2022 10:15:42 GMT
VOLUME [/opt/bonita]
# Tue, 07 Jun 2022 10:15:45 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 07 Jun 2022 10:15:51 GMT
EXPOSE 8080
# Tue, 07 Jun 2022 10:15:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a331e660ead68d382742f61a8656c41551cb44956552a658c4a7b744bface060`  
		Last Modified: Tue, 07 Jun 2022 10:17:56 GMT  
		Size: 86.6 MB (86607112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a213b14ccc59baf8fae328306aad1c663e545d1071ae41070ca2f4b8407c3ce1`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849223db8c9360d39904a129a16fcab82cc75ed0440f6b216c84181e8eaf3a9d`  
		Last Modified: Tue, 07 Jun 2022 10:17:41 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cbc038830160e8447b4c94a591d38b99d4212b0cf63674dc8d0512708ccc57`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 831.6 KB (831568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b68ec78a742cf1aa2513ae7a692d0fe38f63e39b8360ae6358423caa08434`  
		Last Modified: Tue, 07 Jun 2022 10:17:39 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa847ac20a1fea971cba2a4054299001b79527c44c7aee950a97916aa8a7bfb`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a42bd5762b185dffd9c65896d1caace35c218bc37c33dc07dd6f212844fbcb1`  
		Last Modified: Tue, 07 Jun 2022 10:17:49 GMT  
		Size: 113.7 MB (113727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94e67f1cc5eec539069c00057c5a4de04b37c4fd1b7077caca27601fc9b130`  
		Last Modified: Tue, 07 Jun 2022 10:17:38 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:1b28c73bbcde8ad017f3c5f5a0c06bc4edae15eb63135489125002fcf84a3fba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:8ba7080a1dfe944cfa3aef310a80d85721b63bec01b8e828b4efa3720b6eb958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180308041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859da686fb4ba8fbb20e2bfab0b384a8efea93b24a5a7b1671330434e0a3a4a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:13:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:13:19 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:13:20 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:13:21 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:13:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:13:22 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:13:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:13:30 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:13:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:13:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:13:31 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:13:31 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:13:32 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:13:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:13:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6d302c572c7936a2c535df7e3665e4cea12109804d7db2e17c2350483f5c6`  
		Last Modified: Tue, 19 Jul 2022 23:14:04 GMT  
		Size: 60.8 MB (60792590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acef1e43a082930ac2a59ac750fcc44e89eee0d2ee2663ea15276a30a761c112`  
		Last Modified: Tue, 19 Jul 2022 23:13:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753d9cad27595f77612d22db5aff3bf2dd14371b997d3fd09692e97837874620`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59792a17a7735b2bbce017b4e9d56c1eb02cc888a64de33a280730e0c1acc4`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a3b0241dac6de74f098fc124ba52ca8c4950e9b58a750f986190c73b50250b`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f50a37fcc52dae6eaf265933b27d626a5e38dc2eca7b657a3062e4225083d`  
		Last Modified: Tue, 19 Jul 2022 23:14:00 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1095e1b328bb6dfb64e3bc183b9c35afad21a80811146c52cabd8c1251db7`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b14e49b5ca541afa03c868b7617ac3f8bf2dca1217013940b3511bb53ac0fcfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179532890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550d20a8d0a49aaa3f2a866b84e75f0470fc28aa3f2723eabb7f4b7762991f6d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:18:49 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:18:53 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:18:54 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:18:55 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:18:56 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:18:57 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:18:58 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:18:59 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:19:00 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:19:01 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:19:02 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:19:03 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:19:04 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:19:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:07 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:19:09 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:19:20 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:19:21 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:19:22 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:19:23 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:19:24 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:19:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:19:26 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:19:27 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:19:28 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:19:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:19:30 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:19:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:19:32 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:19:34 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:19:34 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:19:35 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:19:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a830a9157109fda713d4c8868452f009b89f5a0aa23e35b64a9fd8ffcbeb248e`  
		Last Modified: Tue, 19 Jul 2022 23:20:35 GMT  
		Size: 60.1 MB (60117412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a219e1f74381cab8fbf4b2158f0e0c8cccf2822e3693f1d8bd13ca27bec084`  
		Last Modified: Tue, 19 Jul 2022 23:20:27 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3153e8cd70c473bb49cd1568765d6399083f8655ace89dcb743660377256711`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448fd19395d15f1dff4ee9d541ee4a4789a87a8902684e4abe9aec78f7c80696`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932c91b8ca10c2ff283945c7998d94267040c160f86b043a84e8a794c4d09a3a`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 3.0 KB (2999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a76d6481ad87c0f65cbd5bf6740c81fbcf6a2b23c530554ec66556c1515ef34`  
		Last Modified: Tue, 19 Jul 2022 23:20:34 GMT  
		Size: 116.7 MB (116688726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdff38d20f7bc060a65e11bf956a87d603ef22aeceda94be739ea3f0f13bd1c`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:6aa40b6458a0b5942abb0cae63ac5d6cd491c5cab4369d5d12de2ebfe3ff2d76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0ae6c2630b8698141ad2b826af32382c0033d6e188becc025982a73e9327d8`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:26:26 GMT
ADD file:fee9d1c50a43d2072ff528133302b3e4d565d1853e14a7d56be9f4532a330841 in / 
# Tue, 19 Jul 2022 22:26:28 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:19:52 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:20:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:20:29 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:20:46 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:20:52 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:20:59 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:21:02 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:21:08 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:21:14 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:21:20 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:21:26 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:21:30 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:21:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:21:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:53 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:21:54 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:22:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:22:25 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:22:40 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:23:01 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:23:07 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:23:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:23:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:23:27 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:23:32 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:23:35 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:23:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:23:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:23:46 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:23:49 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:23:50 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:23:52 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:23:56 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:24:02 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a340aa0651fe455d7a9f4dba0b2b8048ef90ce173a72ac17cf04b9b6af34a2a9`  
		Last Modified: Tue, 19 Jul 2022 22:27:55 GMT  
		Size: 2.8 MB (2811642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0407fa4feb9b7977c80ec2b5ac36e8252a9701c33fb7200fd650a7670fb05bb`  
		Last Modified: Tue, 19 Jul 2022 23:25:13 GMT  
		Size: 56.6 MB (56619857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e50080ba130f5d06da1e2204114d6914f1e86616e352499efccf7b2f91d81f`  
		Last Modified: Tue, 19 Jul 2022 23:25:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74ad31d688802cdd37f41c7f3272a5eb4fd9f2589c0bf3dba4924cc6b7b9eb`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6ab14b03fe37cba7903aa09f0f8d6eb76086d5e0d74230c8816361719fbf8`  
		Last Modified: Tue, 19 Jul 2022 23:25:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665c44209121633da6010cf0aba1f64314d89fca03cd4c667bc331638f17874`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a94295fcd75be4c6ea68c3b2f076d012eec95766121579e8834a5da6806af73`  
		Last Modified: Tue, 19 Jul 2022 23:25:10 GMT  
		Size: 116.7 MB (116690811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2d30730b3cd0901bb65ccabcf1d2e8455dbafb8af1caae6e59207dfc8103d`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:1b28c73bbcde8ad017f3c5f5a0c06bc4edae15eb63135489125002fcf84a3fba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:8ba7080a1dfe944cfa3aef310a80d85721b63bec01b8e828b4efa3720b6eb958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180308041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859da686fb4ba8fbb20e2bfab0b384a8efea93b24a5a7b1671330434e0a3a4a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:13:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:13:19 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:13:20 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:13:21 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:13:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:13:22 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:13:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:13:30 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:13:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:13:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:13:31 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:13:31 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:13:32 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:13:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:13:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6d302c572c7936a2c535df7e3665e4cea12109804d7db2e17c2350483f5c6`  
		Last Modified: Tue, 19 Jul 2022 23:14:04 GMT  
		Size: 60.8 MB (60792590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acef1e43a082930ac2a59ac750fcc44e89eee0d2ee2663ea15276a30a761c112`  
		Last Modified: Tue, 19 Jul 2022 23:13:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753d9cad27595f77612d22db5aff3bf2dd14371b997d3fd09692e97837874620`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59792a17a7735b2bbce017b4e9d56c1eb02cc888a64de33a280730e0c1acc4`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a3b0241dac6de74f098fc124ba52ca8c4950e9b58a750f986190c73b50250b`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f50a37fcc52dae6eaf265933b27d626a5e38dc2eca7b657a3062e4225083d`  
		Last Modified: Tue, 19 Jul 2022 23:14:00 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1095e1b328bb6dfb64e3bc183b9c35afad21a80811146c52cabd8c1251db7`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b14e49b5ca541afa03c868b7617ac3f8bf2dca1217013940b3511bb53ac0fcfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179532890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550d20a8d0a49aaa3f2a866b84e75f0470fc28aa3f2723eabb7f4b7762991f6d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:18:49 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:18:53 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:18:54 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:18:55 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:18:56 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:18:57 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:18:58 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:18:59 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:19:00 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:19:01 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:19:02 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:19:03 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:19:04 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:19:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:07 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:19:09 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:19:20 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:19:21 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:19:22 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:19:23 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:19:24 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:19:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:19:26 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:19:27 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:19:28 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:19:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:19:30 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:19:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:19:32 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:19:34 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:19:34 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:19:35 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:19:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a830a9157109fda713d4c8868452f009b89f5a0aa23e35b64a9fd8ffcbeb248e`  
		Last Modified: Tue, 19 Jul 2022 23:20:35 GMT  
		Size: 60.1 MB (60117412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a219e1f74381cab8fbf4b2158f0e0c8cccf2822e3693f1d8bd13ca27bec084`  
		Last Modified: Tue, 19 Jul 2022 23:20:27 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3153e8cd70c473bb49cd1568765d6399083f8655ace89dcb743660377256711`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448fd19395d15f1dff4ee9d541ee4a4789a87a8902684e4abe9aec78f7c80696`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932c91b8ca10c2ff283945c7998d94267040c160f86b043a84e8a794c4d09a3a`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 3.0 KB (2999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a76d6481ad87c0f65cbd5bf6740c81fbcf6a2b23c530554ec66556c1515ef34`  
		Last Modified: Tue, 19 Jul 2022 23:20:34 GMT  
		Size: 116.7 MB (116688726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdff38d20f7bc060a65e11bf956a87d603ef22aeceda94be739ea3f0f13bd1c`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:6aa40b6458a0b5942abb0cae63ac5d6cd491c5cab4369d5d12de2ebfe3ff2d76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0ae6c2630b8698141ad2b826af32382c0033d6e188becc025982a73e9327d8`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:26:26 GMT
ADD file:fee9d1c50a43d2072ff528133302b3e4d565d1853e14a7d56be9f4532a330841 in / 
# Tue, 19 Jul 2022 22:26:28 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:19:52 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:20:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:20:29 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:20:46 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:20:52 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:20:59 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:21:02 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:21:08 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:21:14 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:21:20 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:21:26 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:21:30 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:21:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:21:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:53 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:21:54 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:22:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:22:25 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:22:40 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:23:01 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:23:07 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:23:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:23:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:23:27 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:23:32 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:23:35 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:23:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:23:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:23:46 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:23:49 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:23:50 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:23:52 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:23:56 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:24:02 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a340aa0651fe455d7a9f4dba0b2b8048ef90ce173a72ac17cf04b9b6af34a2a9`  
		Last Modified: Tue, 19 Jul 2022 22:27:55 GMT  
		Size: 2.8 MB (2811642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0407fa4feb9b7977c80ec2b5ac36e8252a9701c33fb7200fd650a7670fb05bb`  
		Last Modified: Tue, 19 Jul 2022 23:25:13 GMT  
		Size: 56.6 MB (56619857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e50080ba130f5d06da1e2204114d6914f1e86616e352499efccf7b2f91d81f`  
		Last Modified: Tue, 19 Jul 2022 23:25:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74ad31d688802cdd37f41c7f3272a5eb4fd9f2589c0bf3dba4924cc6b7b9eb`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6ab14b03fe37cba7903aa09f0f8d6eb76086d5e0d74230c8816361719fbf8`  
		Last Modified: Tue, 19 Jul 2022 23:25:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665c44209121633da6010cf0aba1f64314d89fca03cd4c667bc331638f17874`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a94295fcd75be4c6ea68c3b2f076d012eec95766121579e8834a5da6806af73`  
		Last Modified: Tue, 19 Jul 2022 23:25:10 GMT  
		Size: 116.7 MB (116690811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2d30730b3cd0901bb65ccabcf1d2e8455dbafb8af1caae6e59207dfc8103d`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:1b28c73bbcde8ad017f3c5f5a0c06bc4edae15eb63135489125002fcf84a3fba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:8ba7080a1dfe944cfa3aef310a80d85721b63bec01b8e828b4efa3720b6eb958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180308041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859da686fb4ba8fbb20e2bfab0b384a8efea93b24a5a7b1671330434e0a3a4a`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:13:15 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:13:19 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:13:20 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:13:21 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:13:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:13:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:13:22 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:13:22 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:13:22 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:13:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:13:30 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:13:30 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:13:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:13:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:13:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:13:31 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:13:31 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:13:32 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:13:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:13:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6d302c572c7936a2c535df7e3665e4cea12109804d7db2e17c2350483f5c6`  
		Last Modified: Tue, 19 Jul 2022 23:14:04 GMT  
		Size: 60.8 MB (60792590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acef1e43a082930ac2a59ac750fcc44e89eee0d2ee2663ea15276a30a761c112`  
		Last Modified: Tue, 19 Jul 2022 23:13:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753d9cad27595f77612d22db5aff3bf2dd14371b997d3fd09692e97837874620`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59792a17a7735b2bbce017b4e9d56c1eb02cc888a64de33a280730e0c1acc4`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a3b0241dac6de74f098fc124ba52ca8c4950e9b58a750f986190c73b50250b`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f50a37fcc52dae6eaf265933b27d626a5e38dc2eca7b657a3062e4225083d`  
		Last Modified: Tue, 19 Jul 2022 23:14:00 GMT  
		Size: 116.7 MB (116690791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1095e1b328bb6dfb64e3bc183b9c35afad21a80811146c52cabd8c1251db7`  
		Last Modified: Tue, 19 Jul 2022 23:13:53 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b14e49b5ca541afa03c868b7617ac3f8bf2dca1217013940b3511bb53ac0fcfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179532890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550d20a8d0a49aaa3f2a866b84e75f0470fc28aa3f2723eabb7f4b7762991f6d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:18:49 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:18:53 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:18:54 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:18:55 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:18:56 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:18:57 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:18:58 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:18:59 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:19:00 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:19:01 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:19:02 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:19:03 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:19:04 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:19:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:19:07 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:19:09 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:19:20 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:19:20 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:19:21 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:19:22 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:19:23 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:19:24 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:19:25 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:19:26 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:19:27 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:19:28 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:19:29 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:19:30 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:19:31 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:19:32 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:19:34 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:19:34 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:19:35 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:19:36 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a830a9157109fda713d4c8868452f009b89f5a0aa23e35b64a9fd8ffcbeb248e`  
		Last Modified: Tue, 19 Jul 2022 23:20:35 GMT  
		Size: 60.1 MB (60117412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a219e1f74381cab8fbf4b2158f0e0c8cccf2822e3693f1d8bd13ca27bec084`  
		Last Modified: Tue, 19 Jul 2022 23:20:27 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3153e8cd70c473bb49cd1568765d6399083f8655ace89dcb743660377256711`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448fd19395d15f1dff4ee9d541ee4a4789a87a8902684e4abe9aec78f7c80696`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932c91b8ca10c2ff283945c7998d94267040c160f86b043a84e8a794c4d09a3a`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 3.0 KB (2999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a76d6481ad87c0f65cbd5bf6740c81fbcf6a2b23c530554ec66556c1515ef34`  
		Last Modified: Tue, 19 Jul 2022 23:20:34 GMT  
		Size: 116.7 MB (116688726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdff38d20f7bc060a65e11bf956a87d603ef22aeceda94be739ea3f0f13bd1c`  
		Last Modified: Tue, 19 Jul 2022 23:20:25 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:6aa40b6458a0b5942abb0cae63ac5d6cd491c5cab4369d5d12de2ebfe3ff2d76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176132332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0ae6c2630b8698141ad2b826af32382c0033d6e188becc025982a73e9327d8`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 19 Jul 2022 22:26:26 GMT
ADD file:fee9d1c50a43d2072ff528133302b3e4d565d1853e14a7d56be9f4532a330841 in / 
# Tue, 19 Jul 2022 22:26:28 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:19:52 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 19 Jul 2022 23:20:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 19 Jul 2022 23:20:29 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 19 Jul 2022 23:20:46 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 19 Jul 2022 23:20:52 GMT
ARG BONITA_VERSION
# Tue, 19 Jul 2022 23:20:59 GMT
ARG BRANDING_VERSION
# Tue, 19 Jul 2022 23:21:02 GMT
ARG BONITA_SHA256
# Tue, 19 Jul 2022 23:21:08 GMT
ARG BASE_URL
# Tue, 19 Jul 2022 23:21:14 GMT
ARG BONITA_URL
# Tue, 19 Jul 2022 23:21:20 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 19 Jul 2022 23:21:26 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 19 Jul 2022 23:21:30 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 19 Jul 2022 23:21:34 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 19 Jul 2022 23:21:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 19 Jul 2022 23:21:53 GMT
RUN mkdir /opt/files
# Tue, 19 Jul 2022 23:21:54 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 19 Jul 2022 23:22:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 19 Jul 2022 23:22:25 GMT
ENV HTTP_API=false
# Tue, 19 Jul 2022 23:22:40 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 19 Jul 2022 23:23:01 GMT
ENV HTTP_API_PASSWORD=
# Tue, 19 Jul 2022 23:23:07 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 19 Jul 2022 23:23:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 19 Jul 2022 23:23:23 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 19 Jul 2022 23:23:27 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 19 Jul 2022 23:23:32 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 19 Jul 2022 23:23:35 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 19 Jul 2022 23:23:39 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 19 Jul 2022 23:23:42 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 19 Jul 2022 23:23:46 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 19 Jul 2022 23:23:49 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 19 Jul 2022 23:23:50 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 19 Jul 2022 23:23:52 GMT
EXPOSE 8080 9000
# Tue, 19 Jul 2022 23:23:56 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 19 Jul 2022 23:24:02 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a340aa0651fe455d7a9f4dba0b2b8048ef90ce173a72ac17cf04b9b6af34a2a9`  
		Last Modified: Tue, 19 Jul 2022 22:27:55 GMT  
		Size: 2.8 MB (2811642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0407fa4feb9b7977c80ec2b5ac36e8252a9701c33fb7200fd650a7670fb05bb`  
		Last Modified: Tue, 19 Jul 2022 23:25:13 GMT  
		Size: 56.6 MB (56619857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e50080ba130f5d06da1e2204114d6914f1e86616e352499efccf7b2f91d81f`  
		Last Modified: Tue, 19 Jul 2022 23:25:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74ad31d688802cdd37f41c7f3272a5eb4fd9f2589c0bf3dba4924cc6b7b9eb`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6ab14b03fe37cba7903aa09f0f8d6eb76086d5e0d74230c8816361719fbf8`  
		Last Modified: Tue, 19 Jul 2022 23:25:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665c44209121633da6010cf0aba1f64314d89fca03cd4c667bc331638f17874`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a94295fcd75be4c6ea68c3b2f076d012eec95766121579e8834a5da6806af73`  
		Last Modified: Tue, 19 Jul 2022 23:25:10 GMT  
		Size: 116.7 MB (116690811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2d30730b3cd0901bb65ccabcf1d2e8455dbafb8af1caae6e59207dfc8103d`  
		Last Modified: Tue, 19 Jul 2022 23:24:59 GMT  
		Size: 5.4 KB (5421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
