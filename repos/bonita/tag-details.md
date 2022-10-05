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
$ docker pull bonita@sha256:691ff7623776b9fa26d5182b64aca8817acecc61aed4463c34e83ba50d0d4bd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:83a7eb49f01c7970d90962f5a6fef3d93192289f698dbba8f90b6b1de1cfc080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235160337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c503f25199a574cfa675b33155eceb41434132490972e0a5a0765c06cc13217`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:40:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:40:35 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:40:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:40:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:40:58 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 16:40:59 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 16:41:00 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 16:41:00 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 16:41:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 16:41:25 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 16:41:26 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 16:41:26 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:41:27 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:41:27 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:41:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846dabaff722db569392a1efe89906e8e1ca4bc84eb96c932aa0fbf02b7dd941`  
		Last Modified: Wed, 05 Oct 2022 16:42:51 GMT  
		Size: 91.5 MB (91515892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5863d1846e2eb78cb6e80fb44f74e1c0179933bb0f7b40c7b7b10af5911024`  
		Last Modified: Wed, 05 Oct 2022 16:42:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1edab7ef68eced67b60c7ff55958e4e40c5b8ec62c3add85114e35deeadb39`  
		Last Modified: Wed, 05 Oct 2022 16:42:38 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882f5e7941b5ac80878951fcb09869c96a0f721b0a20cdf2e6b9103a74718e`  
		Last Modified: Wed, 05 Oct 2022 16:42:37 GMT  
		Size: 506.3 KB (506348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8505d8ac5aa6e6e302b2a3fa2676da59ff3de8a66015d0ed0279df31c345e9`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ed97260ab1975c0d533bdc3cfd748704f12eb45d90117b40a04835f1d16ab`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccead183ac9f9e670441caefd2ea2c88a3fb5b60e46535c9f2627f530ffd17e`  
		Last Modified: Wed, 05 Oct 2022 16:43:07 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6206e1d2404f61d4c1d2849f3021d68da1f31329b64844aab294f40db564c2b`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d9a2e56af738175919ed40f2189881893afde3ad11606ab6a3db5ffe68be7e67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226636573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b9444896f965ea2b7b77331ed3333e56feed9c273f7b3c2684090933148470`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:33:49 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:33:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:33:52 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:33:53 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:34:24 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:34:25 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:34:26 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:34:27 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:34:28 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 15:34:29 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 15:34:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 15:34:31 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 15:34:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:34:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 15:34:34 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 15:34:35 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:34:37 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 15:34:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 15:34:46 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 15:34:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 15:34:48 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:34:50 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:34:50 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:34:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789bea80b428314a47eb7f4e17067a7bd9db24885b5c5678854054cc711cba8`  
		Last Modified: Wed, 05 Oct 2022 15:36:51 GMT  
		Size: 86.0 MB (86000108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690f8bafffc486d75674722c1d017aee4bddee69ec50d79d8f87077977446129`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c367ff864f5661029592d7a3bed330a2f79c16ce8102c035f28569aca191f05`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b45882e84f63cfd2040fa0e6139d9f4d0c49a5d431bec207a03048db5ce60`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 475.8 KB (475769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c3debee7cd70b67cc8265ac994d5b42e08ab5cb229174795f690ab8ed183d2`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1a0ec9d5c14889c075f0f20576c64e38a4a97b5bfc382f96da787249ef61d`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 6.9 KB (6916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf45c7651b4f1955972e94fce182ce9ab439a2eb7b97055d8a4d6fdddd0209e`  
		Last Modified: Wed, 05 Oct 2022 15:37:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd240e24317f66ce11b07ed042033468c24e3fd2e212493379b85691a89bd73`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:c5b4bae0ef2b1ec8f103c848976e76fe80a5a2c3eb57f1c9daf4faf5ecbf12a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234122262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a6153bc410cd56aae703ccffe920fc09827e5dc7d834af4491fafcaa23f90c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:57:53 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:57:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:57:58 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:58:30 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:58:31 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 06 Sep 2022 19:58:32 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 06 Sep 2022 19:58:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 06 Sep 2022 19:58:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 06 Sep 2022 19:58:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:58:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 06 Sep 2022 19:58:34 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 06 Sep 2022 19:58:35 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:58:35 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 06 Sep 2022 19:58:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 06 Sep 2022 19:58:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 06 Sep 2022 19:58:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 06 Sep 2022 19:58:47 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 19:58:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 19:58:48 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 19:58:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a45342cde40ee9bcc2b9d6f7f6b62c7d1a4ba167ba88e21cf76cdfcb1930`  
		Last Modified: Tue, 06 Sep 2022 20:01:20 GMT  
		Size: 86.8 MB (86779043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1c6721b8a1b2545f7ef0e233b0e15ca14a93e43ab409a5f353b3248f6cc74`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8a0e71f3ffc18a3a03cdd9a0c9f5e29daf5f7967d9660272c3150b2406fd7d`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f3529e9719325e350a51fd6326415f40a1a4816d1d8592045cb6fc2a754b4a`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 475.3 KB (475346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a177c133e7fc6e6a67c4b0c85ce03b15ba3f9066762af8f52b7901bd5f87b5c`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf9790806ab46f768dc484f57e39f9722a3c8189267402a1cf44427978213d9`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3591cdb3085035cae7990a6e9575e7600a3d7d0b76ee4754c4cfd67f9756222f`  
		Last Modified: Tue, 06 Sep 2022 20:01:40 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027c634b9ed975106083869c1a6bc728a99d18c5bb108b1f24e03d821ee62e5`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:ed6c5727dd691c93038d1c8eaf07c90ad8f94c80ae5029ba79f15fc77d11ae74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:5ec6cc285fdd2c5013a4369f539b46329b5abeb2f1ea8ee591a54dbee3f0c8ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232893306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935adb03164d1e08e5ac2411f80f0931671303b2eff0ce6e156f31921f87222e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:41:50 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:41:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:41:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 16:41:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:56 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:56 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 16:42:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 16:42:12 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 16:42:12 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:42:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:42:13 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:42:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55d7e27952550c878e39574ef5f7a687a84ee82af84b960475204994cc7b85`  
		Last Modified: Wed, 05 Oct 2022 16:43:33 GMT  
		Size: 91.5 MB (91515847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1417570fe4b9dc321fc36aa7ea824a4e3498fefc251bd8e58b5afd6d745f54`  
		Last Modified: Wed, 05 Oct 2022 16:43:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b68d2a3976336fad6abc36156e12c32e2a401e6e607dc91a5479259a3198a`  
		Last Modified: Wed, 05 Oct 2022 16:43:21 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266dc110117494e92f7b58387ff4d29670c803c37b0c99b0944dda29baea03`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 930.5 KB (930478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d2dff73b8f9b94aa905063c5704022fa9bb64a01a42d36975c235cf64ac8e`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7172813e2adc9a591a81a69db70059e410c9f36cc368481f252416963677601`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641657ee8ee5d0c68da40cbc72a00b625aa122301bc1caa0723344aee03bba03`  
		Last Modified: Wed, 05 Oct 2022 16:43:25 GMT  
		Size: 113.7 MB (113727928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c8a65aef90753ab97f3e21b73e29f9107a47f4c5bc6e88ecb5f03cc75d8b17`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4773b624c4630105a570178dd8e67ca28227921b769935c3fa7f569489e4bd5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224329170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f7f3ff412e8b3c99cdebdf6a3ef77bc68166ac6d9e1406bf6573111ec1a874`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:35:26 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:35:27 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:35:30 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:35:31 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:35:32 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:35:33 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:35:34 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:35:35 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:35:36 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 15:35:37 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 15:35:38 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 15:35:39 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:35:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:42 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:35:44 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 15:35:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 15:35:53 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 15:35:54 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:35:56 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:35:56 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:35:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2502bdaa7fb7beb25b710ccd1790cd1b2809e27c3dd5c46d4c4dba83d203db`  
		Last Modified: Wed, 05 Oct 2022 15:37:37 GMT  
		Size: 86.0 MB (86000050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec5e7938cf270930204c8ffd250f418f2e236a2e68f5ea5d82ab69df3001bd`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f631755389173aaf52aa72ba42646f457f3b67dcf29eac1c306f69945513485`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab611dddc527ad69c9cfa9e09313fb3c2a1ca7e1ce8252fade1d2f75b25815f1`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 859.5 KB (859530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615141c9b889b095f1947bb0315866344021a09635b522538754fc1c35412f98`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7ac7a764faba6ce254b68df36034e0ecf93b7018d31a0ba939a2bf368d86e9`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a799ecc2f3331250c473855a103f9cec1e4f28c436f4080f65df40888fb9cd1a`  
		Last Modified: Wed, 05 Oct 2022 15:37:35 GMT  
		Size: 113.7 MB (113727905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1a80e7cbbb2d6e6dcb35691ffaaae1cd720257b868f8ef1cf257f630346a7b`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:1e6578d8b4c3d62db481d25359b9f79d05166773f772ab86ea525bdac7bb3b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231787296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61bd4165a10292b247997ab6b1c2cf889953636d85084e7a366afcff2bc9a398`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:35 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:59:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:59:40 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 06 Sep 2022 19:59:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:44 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:59:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 06 Sep 2022 19:59:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 06 Sep 2022 19:59:59 GMT
ENV HTTP_API=false
# Tue, 06 Sep 2022 20:00:00 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 20:00:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 20:00:03 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 20:00:04 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8548f8c22e40d7e54097152f5b0da59a6ab2706ce9c294478a909de6a50782b7`  
		Last Modified: Tue, 06 Sep 2022 20:02:17 GMT  
		Size: 86.8 MB (86778981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa2696d5bc76b7b6f73c8606192002ed308d337fa1b2df7c169dca132344e6`  
		Last Modified: Tue, 06 Sep 2022 20:01:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a945ad1159d41018f6988b4621b18077f63b648fa86e2b3555e41848ad9490`  
		Last Modified: Tue, 06 Sep 2022 20:01:59 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca18b4ec34bc35ab22334b49712435c6120b552f4872d350742a7b60adb6cb2`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 831.6 KB (831571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8624f8cc60c44790f133f9525a2c3463c48a0f35b3434aa646c4faf8e0c1c4c5`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f26edf16545b401a0ccc43e3e284c45cbe8fe6ad064b919b43af69b4ccd563`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9095349011839ef32cdac2a80bb5534c76ab9ff79f419bae57abf6f2dcdff0cd`  
		Last Modified: Tue, 06 Sep 2022 20:02:07 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe1b0502c594aa53c8e26b703ce82124e11cf7a76f11d29000d385bb4eace9d`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:ed6c5727dd691c93038d1c8eaf07c90ad8f94c80ae5029ba79f15fc77d11ae74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:5ec6cc285fdd2c5013a4369f539b46329b5abeb2f1ea8ee591a54dbee3f0c8ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232893306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935adb03164d1e08e5ac2411f80f0931671303b2eff0ce6e156f31921f87222e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:41:50 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:41:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:41:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 16:41:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:56 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:56 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 16:42:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 16:42:12 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 16:42:12 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:42:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:42:13 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:42:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55d7e27952550c878e39574ef5f7a687a84ee82af84b960475204994cc7b85`  
		Last Modified: Wed, 05 Oct 2022 16:43:33 GMT  
		Size: 91.5 MB (91515847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1417570fe4b9dc321fc36aa7ea824a4e3498fefc251bd8e58b5afd6d745f54`  
		Last Modified: Wed, 05 Oct 2022 16:43:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b68d2a3976336fad6abc36156e12c32e2a401e6e607dc91a5479259a3198a`  
		Last Modified: Wed, 05 Oct 2022 16:43:21 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266dc110117494e92f7b58387ff4d29670c803c37b0c99b0944dda29baea03`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 930.5 KB (930478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d2dff73b8f9b94aa905063c5704022fa9bb64a01a42d36975c235cf64ac8e`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7172813e2adc9a591a81a69db70059e410c9f36cc368481f252416963677601`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641657ee8ee5d0c68da40cbc72a00b625aa122301bc1caa0723344aee03bba03`  
		Last Modified: Wed, 05 Oct 2022 16:43:25 GMT  
		Size: 113.7 MB (113727928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c8a65aef90753ab97f3e21b73e29f9107a47f4c5bc6e88ecb5f03cc75d8b17`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4773b624c4630105a570178dd8e67ca28227921b769935c3fa7f569489e4bd5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224329170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f7f3ff412e8b3c99cdebdf6a3ef77bc68166ac6d9e1406bf6573111ec1a874`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:35:26 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:35:27 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:35:30 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:35:31 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:35:32 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:35:33 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:35:34 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:35:35 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:35:36 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 15:35:37 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 15:35:38 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 15:35:39 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:35:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:42 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:35:44 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 15:35:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 15:35:53 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 15:35:54 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:35:56 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:35:56 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:35:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2502bdaa7fb7beb25b710ccd1790cd1b2809e27c3dd5c46d4c4dba83d203db`  
		Last Modified: Wed, 05 Oct 2022 15:37:37 GMT  
		Size: 86.0 MB (86000050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec5e7938cf270930204c8ffd250f418f2e236a2e68f5ea5d82ab69df3001bd`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f631755389173aaf52aa72ba42646f457f3b67dcf29eac1c306f69945513485`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab611dddc527ad69c9cfa9e09313fb3c2a1ca7e1ce8252fade1d2f75b25815f1`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 859.5 KB (859530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615141c9b889b095f1947bb0315866344021a09635b522538754fc1c35412f98`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7ac7a764faba6ce254b68df36034e0ecf93b7018d31a0ba939a2bf368d86e9`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a799ecc2f3331250c473855a103f9cec1e4f28c436f4080f65df40888fb9cd1a`  
		Last Modified: Wed, 05 Oct 2022 15:37:35 GMT  
		Size: 113.7 MB (113727905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1a80e7cbbb2d6e6dcb35691ffaaae1cd720257b868f8ef1cf257f630346a7b`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1e6578d8b4c3d62db481d25359b9f79d05166773f772ab86ea525bdac7bb3b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231787296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61bd4165a10292b247997ab6b1c2cf889953636d85084e7a366afcff2bc9a398`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:35 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:59:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:59:40 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 06 Sep 2022 19:59:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:44 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:59:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 06 Sep 2022 19:59:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 06 Sep 2022 19:59:59 GMT
ENV HTTP_API=false
# Tue, 06 Sep 2022 20:00:00 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 20:00:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 20:00:03 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 20:00:04 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8548f8c22e40d7e54097152f5b0da59a6ab2706ce9c294478a909de6a50782b7`  
		Last Modified: Tue, 06 Sep 2022 20:02:17 GMT  
		Size: 86.8 MB (86778981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa2696d5bc76b7b6f73c8606192002ed308d337fa1b2df7c169dca132344e6`  
		Last Modified: Tue, 06 Sep 2022 20:01:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a945ad1159d41018f6988b4621b18077f63b648fa86e2b3555e41848ad9490`  
		Last Modified: Tue, 06 Sep 2022 20:01:59 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca18b4ec34bc35ab22334b49712435c6120b552f4872d350742a7b60adb6cb2`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 831.6 KB (831571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8624f8cc60c44790f133f9525a2c3463c48a0f35b3434aa646c4faf8e0c1c4c5`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f26edf16545b401a0ccc43e3e284c45cbe8fe6ad064b919b43af69b4ccd563`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9095349011839ef32cdac2a80bb5534c76ab9ff79f419bae57abf6f2dcdff0cd`  
		Last Modified: Tue, 06 Sep 2022 20:02:07 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe1b0502c594aa53c8e26b703ce82124e11cf7a76f11d29000d385bb4eace9d`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:977f4e8862be31d76a5a463b0238a58fcd4af483ea1c6d6cb1ed75a1447c0d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:08cde8fece645d8b60bc13cf85691f0a092238a270c1a95554fc71714cd25237
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b7a73741c772da78e05b71140aeaa6e2838bcfef7277b7af94e3813db00ebb`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:15:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:15:47 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:15:48 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:15:49 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:50 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:15:50 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:16:01 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:16:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:16:03 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:16:03 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:16:03 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:16:03 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:16:03 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e40e66c88000cdcf6a5f303ff471b71908973b42e6d2c853ebafc528c1f58d`  
		Last Modified: Tue, 09 Aug 2022 18:16:38 GMT  
		Size: 60.8 MB (60808791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8517b429307545f8abc13fc0b37faa4607093e758af1d721cd166a9c9d59ec60`  
		Last Modified: Tue, 09 Aug 2022 18:16:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a90d8fa310d2a6ea37f38a5d6783134999b8e41a9a6cea96f56c35fef2514e`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7082e206c7455f0f4b81da210af350e50379ccb7f4d413868083cb6bd93fb7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afa20c272a36d9fffe827f8ce399a488ef133030401d5e3892cb8f30b9ab2c7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9086b05d70c72cfe77142c9829855c34c099504b88df663d5d954537502aef`  
		Last Modified: Tue, 09 Aug 2022 18:16:34 GMT  
		Size: 116.7 MB (116690829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153200db9a09f679584a791a878014d3dcdf52d99869e37107b43db18c4d9cc3`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9659f7730d354083e732097fd3656a47ab26b8c4f2010683fc2fbe6358cd9dad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30779f62863399675fedee53f8a02f2a0fea94360bde10754580989873e9ef13`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:18:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:18:36 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:18:36 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:18:37 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:18:38 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:18:39 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:18:40 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:18:41 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:18:42 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:18:43 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:18:44 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:18:45 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:18:46 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:18:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:49 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:18:51 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:19:04 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:19:05 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:19:06 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:19:07 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:19:08 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:19:09 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:19:10 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:19:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:19:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:19:13 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:19:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:19:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:19:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:19:17 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:19:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:19:19 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:19:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc88915541d6f4421b66a886f25f68b9655dc1dee732760c3086d5e8b3304a4a`  
		Last Modified: Tue, 09 Aug 2022 18:20:24 GMT  
		Size: 60.1 MB (60129514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bc8304739386ec9aab2a1dcd52eb85ca85059ce787cc536f24934bb6907c1`  
		Last Modified: Tue, 09 Aug 2022 18:20:16 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f5f51932f11b34b80147eec1268be25c87b241a595d18adb836b09480ebee6`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec51c34c596f0fcdf1cc75e2c3154642dc1e041ed2d502ad3468cbf5ee7633a`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccaa414eaa82b83c723b3217df9302e719890e1ceacda1452c141980ae6f5d`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 3.0 KB (3002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334448ededff63c05c8efe4578487e4b1ad071d95373c4c39515f1c33472d788`  
		Last Modified: Tue, 09 Aug 2022 18:20:17 GMT  
		Size: 116.7 MB (116688789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61a4040e3817598cff22a8fae45d9f16a5d5f8703e2acef71454e5df2d9889`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:905376aad5c6b1828a693ea6913e13ee18e890176d32e306d9f9d015ddd0b228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7c95b1e8662e1c67b791b144f27360f33bf8c5a12aa9beb134ef618268006`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:57:05 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 10 Aug 2022 02:57:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 10 Aug 2022 02:57:16 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 10 Aug 2022 02:57:18 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BRANDING_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_SHA256
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BASE_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ARG BONITA_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 10 Aug 2022 02:57:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:23 GMT
RUN mkdir /opt/files
# Wed, 10 Aug 2022 02:57:23 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 10 Aug 2022 02:57:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API=false
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 10 Aug 2022 02:57:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 10 Aug 2022 02:57:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 10 Aug 2022 02:57:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 10 Aug 2022 02:57:44 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 10 Aug 2022 02:57:44 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 10 Aug 2022 02:57:44 GMT
EXPOSE 8080 9000
# Wed, 10 Aug 2022 02:57:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 10 Aug 2022 02:57:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd0e6368901462206ecfbedd1db3517fe94f68bc7b57918c328df47fbdbbf3`  
		Last Modified: Wed, 10 Aug 2022 02:58:51 GMT  
		Size: 56.6 MB (56628364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2f41beebf7247171a5b275e0598e9ed16be2ad6ffa16ad4c9c8f036f8800f1`  
		Last Modified: Wed, 10 Aug 2022 02:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d583bf09d162033ea6a52f524d3142e51ab87f5ce8e1c17c918e8c47527016c`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593fae9e149af994c09345a3dcb015f0959fed2dd20e229f5fafea90d08f429b`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96057fb9286d4d93de5c991d820e3b03be1923bec7ea58592b8417b9f69368bc`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77133cc538711ede4f9dda1c5d44ea027f26326760bb0136c00411045f62d0d`  
		Last Modified: Wed, 10 Aug 2022 02:58:47 GMT  
		Size: 116.7 MB (116690853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933c622a69b13e9df15b3809c6323b98b3a6e697a0ce37025afde53920527a41`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:977f4e8862be31d76a5a463b0238a58fcd4af483ea1c6d6cb1ed75a1447c0d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:08cde8fece645d8b60bc13cf85691f0a092238a270c1a95554fc71714cd25237
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b7a73741c772da78e05b71140aeaa6e2838bcfef7277b7af94e3813db00ebb`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:15:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:15:47 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:15:48 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:15:49 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:50 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:15:50 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:16:01 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:16:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:16:03 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:16:03 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:16:03 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:16:03 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:16:03 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e40e66c88000cdcf6a5f303ff471b71908973b42e6d2c853ebafc528c1f58d`  
		Last Modified: Tue, 09 Aug 2022 18:16:38 GMT  
		Size: 60.8 MB (60808791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8517b429307545f8abc13fc0b37faa4607093e758af1d721cd166a9c9d59ec60`  
		Last Modified: Tue, 09 Aug 2022 18:16:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a90d8fa310d2a6ea37f38a5d6783134999b8e41a9a6cea96f56c35fef2514e`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7082e206c7455f0f4b81da210af350e50379ccb7f4d413868083cb6bd93fb7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afa20c272a36d9fffe827f8ce399a488ef133030401d5e3892cb8f30b9ab2c7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9086b05d70c72cfe77142c9829855c34c099504b88df663d5d954537502aef`  
		Last Modified: Tue, 09 Aug 2022 18:16:34 GMT  
		Size: 116.7 MB (116690829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153200db9a09f679584a791a878014d3dcdf52d99869e37107b43db18c4d9cc3`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9659f7730d354083e732097fd3656a47ab26b8c4f2010683fc2fbe6358cd9dad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30779f62863399675fedee53f8a02f2a0fea94360bde10754580989873e9ef13`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:18:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:18:36 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:18:36 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:18:37 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:18:38 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:18:39 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:18:40 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:18:41 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:18:42 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:18:43 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:18:44 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:18:45 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:18:46 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:18:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:49 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:18:51 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:19:04 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:19:05 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:19:06 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:19:07 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:19:08 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:19:09 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:19:10 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:19:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:19:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:19:13 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:19:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:19:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:19:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:19:17 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:19:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:19:19 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:19:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc88915541d6f4421b66a886f25f68b9655dc1dee732760c3086d5e8b3304a4a`  
		Last Modified: Tue, 09 Aug 2022 18:20:24 GMT  
		Size: 60.1 MB (60129514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bc8304739386ec9aab2a1dcd52eb85ca85059ce787cc536f24934bb6907c1`  
		Last Modified: Tue, 09 Aug 2022 18:20:16 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f5f51932f11b34b80147eec1268be25c87b241a595d18adb836b09480ebee6`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec51c34c596f0fcdf1cc75e2c3154642dc1e041ed2d502ad3468cbf5ee7633a`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccaa414eaa82b83c723b3217df9302e719890e1ceacda1452c141980ae6f5d`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 3.0 KB (3002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334448ededff63c05c8efe4578487e4b1ad071d95373c4c39515f1c33472d788`  
		Last Modified: Tue, 09 Aug 2022 18:20:17 GMT  
		Size: 116.7 MB (116688789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61a4040e3817598cff22a8fae45d9f16a5d5f8703e2acef71454e5df2d9889`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:905376aad5c6b1828a693ea6913e13ee18e890176d32e306d9f9d015ddd0b228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7c95b1e8662e1c67b791b144f27360f33bf8c5a12aa9beb134ef618268006`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:57:05 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 10 Aug 2022 02:57:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 10 Aug 2022 02:57:16 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 10 Aug 2022 02:57:18 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BRANDING_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_SHA256
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BASE_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ARG BONITA_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 10 Aug 2022 02:57:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:23 GMT
RUN mkdir /opt/files
# Wed, 10 Aug 2022 02:57:23 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 10 Aug 2022 02:57:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API=false
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 10 Aug 2022 02:57:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 10 Aug 2022 02:57:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 10 Aug 2022 02:57:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 10 Aug 2022 02:57:44 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 10 Aug 2022 02:57:44 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 10 Aug 2022 02:57:44 GMT
EXPOSE 8080 9000
# Wed, 10 Aug 2022 02:57:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 10 Aug 2022 02:57:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd0e6368901462206ecfbedd1db3517fe94f68bc7b57918c328df47fbdbbf3`  
		Last Modified: Wed, 10 Aug 2022 02:58:51 GMT  
		Size: 56.6 MB (56628364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2f41beebf7247171a5b275e0598e9ed16be2ad6ffa16ad4c9c8f036f8800f1`  
		Last Modified: Wed, 10 Aug 2022 02:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d583bf09d162033ea6a52f524d3142e51ab87f5ce8e1c17c918e8c47527016c`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593fae9e149af994c09345a3dcb015f0959fed2dd20e229f5fafea90d08f429b`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96057fb9286d4d93de5c991d820e3b03be1923bec7ea58592b8417b9f69368bc`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77133cc538711ede4f9dda1c5d44ea027f26326760bb0136c00411045f62d0d`  
		Last Modified: Wed, 10 Aug 2022 02:58:47 GMT  
		Size: 116.7 MB (116690853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933c622a69b13e9df15b3809c6323b98b3a6e697a0ce37025afde53920527a41`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:a7c7c53dd10f183da1116ec41b94116f9a88b7a514bdb1f317e339d3af164be9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:41b25a701abc7efb83cf4c71facb6455c39b2eb555a83ddb1944f54dd11a69b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232092703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:accdf2c15718501e9b34aaafd201d28724d8346ffc9717d36d4f7991a5a21d54`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:40:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:40:35 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:40:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:40:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:40:38 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 05 Oct 2022 16:40:39 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 05 Oct 2022 16:40:39 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 16:40:39 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:40:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 16:40:39 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 16:40:40 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:40:40 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 05 Oct 2022 16:40:46 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 05 Oct 2022 16:40:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 16:40:49 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 16:40:49 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:40:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:40:49 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:40:49 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846dabaff722db569392a1efe89906e8e1ca4bc84eb96c932aa0fbf02b7dd941`  
		Last Modified: Wed, 05 Oct 2022 16:42:51 GMT  
		Size: 91.5 MB (91515892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5863d1846e2eb78cb6e80fb44f74e1c0179933bb0f7b40c7b7b10af5911024`  
		Last Modified: Wed, 05 Oct 2022 16:42:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1edab7ef68eced67b60c7ff55958e4e40c5b8ec62c3add85114e35deeadb39`  
		Last Modified: Wed, 05 Oct 2022 16:42:38 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882f5e7941b5ac80878951fcb09869c96a0f721b0a20cdf2e6b9103a74718e`  
		Last Modified: Wed, 05 Oct 2022 16:42:37 GMT  
		Size: 506.3 KB (506348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01dc521296adcf1b2641c28131d275616de738ae0512594095e9f0f556cdc86`  
		Last Modified: Wed, 05 Oct 2022 16:42:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239c4603b63c95231e1a8f29bdf3e6bb9010f898390b011bf2980d112930be36`  
		Last Modified: Wed, 05 Oct 2022 16:42:36 GMT  
		Size: 6.9 KB (6888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a62068148635498ac11047dbbbed01f7a39e21f9b5c898acd73f69012b9c27`  
		Last Modified: Wed, 05 Oct 2022 16:42:42 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585ebc0a052582fe16181cde1cb0116ae57c459bd6879345bb7e66c49aa90ee2`  
		Last Modified: Wed, 05 Oct 2022 16:42:36 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b5b7ec88edee948ee6bfd8a659f75cae1826c5648b1c0e18e0e0b6df28e6a98f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223568945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29feeed167b49f6c932feb11f211da96afb66ab5d7609672775ad73011a1e256`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:33:49 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:33:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:33:52 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:33:53 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:33:54 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:33:55 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:33:56 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:33:57 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 05 Oct 2022 15:33:58 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 05 Oct 2022 15:33:59 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 15:34:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:34:01 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 15:34:02 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 15:34:03 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:34:05 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 05 Oct 2022 15:34:12 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 05 Oct 2022 15:34:14 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 15:34:15 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 15:34:16 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:34:18 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:34:18 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:34:19 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789bea80b428314a47eb7f4e17067a7bd9db24885b5c5678854054cc711cba8`  
		Last Modified: Wed, 05 Oct 2022 15:36:51 GMT  
		Size: 86.0 MB (86000108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690f8bafffc486d75674722c1d017aee4bddee69ec50d79d8f87077977446129`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c367ff864f5661029592d7a3bed330a2f79c16ce8102c035f28569aca191f05`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b45882e84f63cfd2040fa0e6139d9f4d0c49a5d431bec207a03048db5ce60`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 475.8 KB (475769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb763394014ec9fda7ba78421256ef5c896ee3246ae42b71779e8afedb5a511`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618b822a060022e297130c37f53754f7ee5570cffc6634dc88688343d777d5b`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 6.9 KB (6867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e129e5adefc89f85b77cd56a31118dea290fb2ea574ee259a8999a131777f8`  
		Last Modified: Wed, 05 Oct 2022 15:36:44 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d21cf708f5b91c86cde1c630ee7489c16f56fb09cf98eb139038e2cb5e43be9`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:702b31adf3f1cbacf5fb476c64eea7f9e6e38b04af9cdc8313c606579809d564
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.1 MB (231054624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefd368fe030b6d954197cd422b1159468e717856b6afce0cedb33732aa92a58`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:57:53 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:57:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:57:58 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:57:59 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:57:59 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:57:59 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 06 Sep 2022 19:57:59 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 06 Sep 2022 19:58:00 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 06 Sep 2022 19:58:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:58:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 06 Sep 2022 19:58:01 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 06 Sep 2022 19:58:02 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:58:03 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 06 Sep 2022 19:58:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 06 Sep 2022 19:58:16 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 06 Sep 2022 19:58:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 06 Sep 2022 19:58:18 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 19:58:18 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 19:58:18 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 19:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a45342cde40ee9bcc2b9d6f7f6b62c7d1a4ba167ba88e21cf76cdfcb1930`  
		Last Modified: Tue, 06 Sep 2022 20:01:20 GMT  
		Size: 86.8 MB (86779043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1c6721b8a1b2545f7ef0e233b0e15ca14a93e43ab409a5f353b3248f6cc74`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8a0e71f3ffc18a3a03cdd9a0c9f5e29daf5f7967d9660272c3150b2406fd7d`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f3529e9719325e350a51fd6326415f40a1a4816d1d8592045cb6fc2a754b4a`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 475.3 KB (475346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce41c60d6e7973360b6b0883539acff2170af8add2627160e1c5122dd9174b`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c86e9a486d34173e16099f4ad2e559896bc38ced63b112a6aa6c7004b2f5403`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 6.9 KB (6889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eecbee25c12b1416317215273436fed6a219dc49b9ab010ed18e90b7bc035c`  
		Last Modified: Tue, 06 Sep 2022 20:01:06 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7606ce6ef992c26eecd730cfea42a6cb753863a63c66b957179be10eaf26a7c9`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:a7c7c53dd10f183da1116ec41b94116f9a88b7a514bdb1f317e339d3af164be9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:41b25a701abc7efb83cf4c71facb6455c39b2eb555a83ddb1944f54dd11a69b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.1 MB (232092703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:accdf2c15718501e9b34aaafd201d28724d8346ffc9717d36d4f7991a5a21d54`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:40:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:40:35 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:40:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:40:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:40:38 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 05 Oct 2022 16:40:39 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 05 Oct 2022 16:40:39 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 16:40:39 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:40:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 16:40:39 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 16:40:40 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:40:40 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 05 Oct 2022 16:40:46 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 05 Oct 2022 16:40:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 16:40:49 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 16:40:49 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:40:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:40:49 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:40:49 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846dabaff722db569392a1efe89906e8e1ca4bc84eb96c932aa0fbf02b7dd941`  
		Last Modified: Wed, 05 Oct 2022 16:42:51 GMT  
		Size: 91.5 MB (91515892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5863d1846e2eb78cb6e80fb44f74e1c0179933bb0f7b40c7b7b10af5911024`  
		Last Modified: Wed, 05 Oct 2022 16:42:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1edab7ef68eced67b60c7ff55958e4e40c5b8ec62c3add85114e35deeadb39`  
		Last Modified: Wed, 05 Oct 2022 16:42:38 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882f5e7941b5ac80878951fcb09869c96a0f721b0a20cdf2e6b9103a74718e`  
		Last Modified: Wed, 05 Oct 2022 16:42:37 GMT  
		Size: 506.3 KB (506348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01dc521296adcf1b2641c28131d275616de738ae0512594095e9f0f556cdc86`  
		Last Modified: Wed, 05 Oct 2022 16:42:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239c4603b63c95231e1a8f29bdf3e6bb9010f898390b011bf2980d112930be36`  
		Last Modified: Wed, 05 Oct 2022 16:42:36 GMT  
		Size: 6.9 KB (6888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a62068148635498ac11047dbbbed01f7a39e21f9b5c898acd73f69012b9c27`  
		Last Modified: Wed, 05 Oct 2022 16:42:42 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585ebc0a052582fe16181cde1cb0116ae57c459bd6879345bb7e66c49aa90ee2`  
		Last Modified: Wed, 05 Oct 2022 16:42:36 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b5b7ec88edee948ee6bfd8a659f75cae1826c5648b1c0e18e0e0b6df28e6a98f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223568945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29feeed167b49f6c932feb11f211da96afb66ab5d7609672775ad73011a1e256`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:33:49 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:33:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:33:52 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:33:53 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:33:54 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:33:55 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:33:56 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:33:57 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 05 Oct 2022 15:33:58 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 05 Oct 2022 15:33:59 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 15:34:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:34:01 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 15:34:02 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 15:34:03 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:34:05 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 05 Oct 2022 15:34:12 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 05 Oct 2022 15:34:14 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 15:34:15 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 15:34:16 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:34:18 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:34:18 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:34:19 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789bea80b428314a47eb7f4e17067a7bd9db24885b5c5678854054cc711cba8`  
		Last Modified: Wed, 05 Oct 2022 15:36:51 GMT  
		Size: 86.0 MB (86000108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690f8bafffc486d75674722c1d017aee4bddee69ec50d79d8f87077977446129`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c367ff864f5661029592d7a3bed330a2f79c16ce8102c035f28569aca191f05`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b45882e84f63cfd2040fa0e6139d9f4d0c49a5d431bec207a03048db5ce60`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 475.8 KB (475769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb763394014ec9fda7ba78421256ef5c896ee3246ae42b71779e8afedb5a511`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618b822a060022e297130c37f53754f7ee5570cffc6634dc88688343d777d5b`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 6.9 KB (6867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e129e5adefc89f85b77cd56a31118dea290fb2ea574ee259a8999a131777f8`  
		Last Modified: Wed, 05 Oct 2022 15:36:44 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d21cf708f5b91c86cde1c630ee7489c16f56fb09cf98eb139038e2cb5e43be9`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:702b31adf3f1cbacf5fb476c64eea7f9e6e38b04af9cdc8313c606579809d564
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.1 MB (231054624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefd368fe030b6d954197cd422b1159468e717856b6afce0cedb33732aa92a58`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:57:53 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:57:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:57:58 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:57:59 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:57:59 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:57:59 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 06 Sep 2022 19:57:59 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 06 Sep 2022 19:58:00 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 06 Sep 2022 19:58:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:58:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 06 Sep 2022 19:58:01 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 06 Sep 2022 19:58:02 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:58:03 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 06 Sep 2022 19:58:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 06 Sep 2022 19:58:16 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 06 Sep 2022 19:58:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 06 Sep 2022 19:58:18 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 19:58:18 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 19:58:18 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 19:58:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a45342cde40ee9bcc2b9d6f7f6b62c7d1a4ba167ba88e21cf76cdfcb1930`  
		Last Modified: Tue, 06 Sep 2022 20:01:20 GMT  
		Size: 86.8 MB (86779043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1c6721b8a1b2545f7ef0e233b0e15ca14a93e43ab409a5f353b3248f6cc74`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8a0e71f3ffc18a3a03cdd9a0c9f5e29daf5f7967d9660272c3150b2406fd7d`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f3529e9719325e350a51fd6326415f40a1a4816d1d8592045cb6fc2a754b4a`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 475.3 KB (475346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebce41c60d6e7973360b6b0883539acff2170af8add2627160e1c5122dd9174b`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c86e9a486d34173e16099f4ad2e559896bc38ced63b112a6aa6c7004b2f5403`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 6.9 KB (6889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eecbee25c12b1416317215273436fed6a219dc49b9ab010ed18e90b7bc035c`  
		Last Modified: Tue, 06 Sep 2022 20:01:06 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7606ce6ef992c26eecd730cfea42a6cb753863a63c66b957179be10eaf26a7c9`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:691ff7623776b9fa26d5182b64aca8817acecc61aed4463c34e83ba50d0d4bd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:83a7eb49f01c7970d90962f5a6fef3d93192289f698dbba8f90b6b1de1cfc080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235160337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c503f25199a574cfa675b33155eceb41434132490972e0a5a0765c06cc13217`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:40:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:40:35 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:40:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:40:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:40:58 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 16:40:59 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 16:41:00 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 16:41:00 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 16:41:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 16:41:25 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 16:41:26 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 16:41:26 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:41:27 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:41:27 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:41:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846dabaff722db569392a1efe89906e8e1ca4bc84eb96c932aa0fbf02b7dd941`  
		Last Modified: Wed, 05 Oct 2022 16:42:51 GMT  
		Size: 91.5 MB (91515892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5863d1846e2eb78cb6e80fb44f74e1c0179933bb0f7b40c7b7b10af5911024`  
		Last Modified: Wed, 05 Oct 2022 16:42:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1edab7ef68eced67b60c7ff55958e4e40c5b8ec62c3add85114e35deeadb39`  
		Last Modified: Wed, 05 Oct 2022 16:42:38 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882f5e7941b5ac80878951fcb09869c96a0f721b0a20cdf2e6b9103a74718e`  
		Last Modified: Wed, 05 Oct 2022 16:42:37 GMT  
		Size: 506.3 KB (506348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8505d8ac5aa6e6e302b2a3fa2676da59ff3de8a66015d0ed0279df31c345e9`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ed97260ab1975c0d533bdc3cfd748704f12eb45d90117b40a04835f1d16ab`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccead183ac9f9e670441caefd2ea2c88a3fb5b60e46535c9f2627f530ffd17e`  
		Last Modified: Wed, 05 Oct 2022 16:43:07 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6206e1d2404f61d4c1d2849f3021d68da1f31329b64844aab294f40db564c2b`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d9a2e56af738175919ed40f2189881893afde3ad11606ab6a3db5ffe68be7e67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226636573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b9444896f965ea2b7b77331ed3333e56feed9c273f7b3c2684090933148470`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:33:49 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:33:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:33:52 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:33:53 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:34:24 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:34:25 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:34:26 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:34:27 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:34:28 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 15:34:29 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 15:34:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 15:34:31 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 15:34:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:34:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 15:34:34 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 15:34:35 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:34:37 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 15:34:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 15:34:46 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 15:34:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 15:34:48 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:34:50 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:34:50 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:34:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789bea80b428314a47eb7f4e17067a7bd9db24885b5c5678854054cc711cba8`  
		Last Modified: Wed, 05 Oct 2022 15:36:51 GMT  
		Size: 86.0 MB (86000108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690f8bafffc486d75674722c1d017aee4bddee69ec50d79d8f87077977446129`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c367ff864f5661029592d7a3bed330a2f79c16ce8102c035f28569aca191f05`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b45882e84f63cfd2040fa0e6139d9f4d0c49a5d431bec207a03048db5ce60`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 475.8 KB (475769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c3debee7cd70b67cc8265ac994d5b42e08ab5cb229174795f690ab8ed183d2`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1a0ec9d5c14889c075f0f20576c64e38a4a97b5bfc382f96da787249ef61d`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 6.9 KB (6916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf45c7651b4f1955972e94fce182ce9ab439a2eb7b97055d8a4d6fdddd0209e`  
		Last Modified: Wed, 05 Oct 2022 15:37:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd240e24317f66ce11b07ed042033468c24e3fd2e212493379b85691a89bd73`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:c5b4bae0ef2b1ec8f103c848976e76fe80a5a2c3eb57f1c9daf4faf5ecbf12a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234122262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a6153bc410cd56aae703ccffe920fc09827e5dc7d834af4491fafcaa23f90c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:57:53 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:57:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:57:58 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:58:30 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:58:31 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 06 Sep 2022 19:58:32 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 06 Sep 2022 19:58:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 06 Sep 2022 19:58:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 06 Sep 2022 19:58:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:58:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 06 Sep 2022 19:58:34 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 06 Sep 2022 19:58:35 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:58:35 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 06 Sep 2022 19:58:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 06 Sep 2022 19:58:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 06 Sep 2022 19:58:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 06 Sep 2022 19:58:47 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 19:58:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 19:58:48 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 19:58:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a45342cde40ee9bcc2b9d6f7f6b62c7d1a4ba167ba88e21cf76cdfcb1930`  
		Last Modified: Tue, 06 Sep 2022 20:01:20 GMT  
		Size: 86.8 MB (86779043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1c6721b8a1b2545f7ef0e233b0e15ca14a93e43ab409a5f353b3248f6cc74`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8a0e71f3ffc18a3a03cdd9a0c9f5e29daf5f7967d9660272c3150b2406fd7d`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f3529e9719325e350a51fd6326415f40a1a4816d1d8592045cb6fc2a754b4a`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 475.3 KB (475346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a177c133e7fc6e6a67c4b0c85ce03b15ba3f9066762af8f52b7901bd5f87b5c`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf9790806ab46f768dc484f57e39f9722a3c8189267402a1cf44427978213d9`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3591cdb3085035cae7990a6e9575e7600a3d7d0b76ee4754c4cfd67f9756222f`  
		Last Modified: Tue, 06 Sep 2022 20:01:40 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027c634b9ed975106083869c1a6bc728a99d18c5bb108b1f24e03d821ee62e5`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:691ff7623776b9fa26d5182b64aca8817acecc61aed4463c34e83ba50d0d4bd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:83a7eb49f01c7970d90962f5a6fef3d93192289f698dbba8f90b6b1de1cfc080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235160337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c503f25199a574cfa675b33155eceb41434132490972e0a5a0765c06cc13217`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:40:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:40:35 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:40:35 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:40:38 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:40:38 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:40:58 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:40:58 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 16:40:59 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:40:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 16:41:00 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 16:41:00 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 16:41:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 16:41:25 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 16:41:26 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 16:41:26 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:41:27 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:41:27 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:41:27 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846dabaff722db569392a1efe89906e8e1ca4bc84eb96c932aa0fbf02b7dd941`  
		Last Modified: Wed, 05 Oct 2022 16:42:51 GMT  
		Size: 91.5 MB (91515892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5863d1846e2eb78cb6e80fb44f74e1c0179933bb0f7b40c7b7b10af5911024`  
		Last Modified: Wed, 05 Oct 2022 16:42:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1edab7ef68eced67b60c7ff55958e4e40c5b8ec62c3add85114e35deeadb39`  
		Last Modified: Wed, 05 Oct 2022 16:42:38 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882f5e7941b5ac80878951fcb09869c96a0f721b0a20cdf2e6b9103a74718e`  
		Last Modified: Wed, 05 Oct 2022 16:42:37 GMT  
		Size: 506.3 KB (506348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8505d8ac5aa6e6e302b2a3fa2676da59ff3de8a66015d0ed0279df31c345e9`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ed97260ab1975c0d533bdc3cfd748704f12eb45d90117b40a04835f1d16ab`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccead183ac9f9e670441caefd2ea2c88a3fb5b60e46535c9f2627f530ffd17e`  
		Last Modified: Wed, 05 Oct 2022 16:43:07 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6206e1d2404f61d4c1d2849f3021d68da1f31329b64844aab294f40db564c2b`  
		Last Modified: Wed, 05 Oct 2022 16:43:01 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d9a2e56af738175919ed40f2189881893afde3ad11606ab6a3db5ffe68be7e67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226636573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b9444896f965ea2b7b77331ed3333e56feed9c273f7b3c2684090933148470`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:33:49 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:33:49 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:33:52 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:33:53 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:34:24 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:34:25 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:34:26 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:34:27 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:34:28 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 15:34:29 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 15:34:30 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 15:34:31 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 15:34:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:34:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 15:34:34 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 15:34:35 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:34:37 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 15:34:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 15:34:46 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 15:34:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 15:34:48 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:34:50 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:34:50 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:34:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789bea80b428314a47eb7f4e17067a7bd9db24885b5c5678854054cc711cba8`  
		Last Modified: Wed, 05 Oct 2022 15:36:51 GMT  
		Size: 86.0 MB (86000108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690f8bafffc486d75674722c1d017aee4bddee69ec50d79d8f87077977446129`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c367ff864f5661029592d7a3bed330a2f79c16ce8102c035f28569aca191f05`  
		Last Modified: Wed, 05 Oct 2022 15:36:39 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b45882e84f63cfd2040fa0e6139d9f4d0c49a5d431bec207a03048db5ce60`  
		Last Modified: Wed, 05 Oct 2022 15:36:37 GMT  
		Size: 475.8 KB (475769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c3debee7cd70b67cc8265ac994d5b42e08ab5cb229174795f690ab8ed183d2`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1a0ec9d5c14889c075f0f20576c64e38a4a97b5bfc382f96da787249ef61d`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 6.9 KB (6916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf45c7651b4f1955972e94fce182ce9ab439a2eb7b97055d8a4d6fdddd0209e`  
		Last Modified: Wed, 05 Oct 2022 15:37:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd240e24317f66ce11b07ed042033468c24e3fd2e212493379b85691a89bd73`  
		Last Modified: Wed, 05 Oct 2022 15:37:02 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:c5b4bae0ef2b1ec8f103c848976e76fe80a5a2c3eb57f1c9daf4faf5ecbf12a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234122262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a6153bc410cd56aae703ccffe920fc09827e5dc7d834af4491fafcaa23f90c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:57:53 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:57:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:57:58 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:57:58 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:58:30 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:58:31 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:58:31 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 06 Sep 2022 19:58:32 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 06 Sep 2022 19:58:32 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 06 Sep 2022 19:58:32 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 06 Sep 2022 19:58:33 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:58:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 06 Sep 2022 19:58:34 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 06 Sep 2022 19:58:35 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:58:35 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 06 Sep 2022 19:58:42 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 06 Sep 2022 19:58:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 06 Sep 2022 19:58:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 06 Sep 2022 19:58:47 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 19:58:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 19:58:48 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 19:58:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a45342cde40ee9bcc2b9d6f7f6b62c7d1a4ba167ba88e21cf76cdfcb1930`  
		Last Modified: Tue, 06 Sep 2022 20:01:20 GMT  
		Size: 86.8 MB (86779043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca1c6721b8a1b2545f7ef0e233b0e15ca14a93e43ab409a5f353b3248f6cc74`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8a0e71f3ffc18a3a03cdd9a0c9f5e29daf5f7967d9660272c3150b2406fd7d`  
		Last Modified: Tue, 06 Sep 2022 20:01:00 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f3529e9719325e350a51fd6326415f40a1a4816d1d8592045cb6fc2a754b4a`  
		Last Modified: Tue, 06 Sep 2022 20:00:58 GMT  
		Size: 475.3 KB (475346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a177c133e7fc6e6a67c4b0c85ce03b15ba3f9066762af8f52b7901bd5f87b5c`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf9790806ab46f768dc484f57e39f9722a3c8189267402a1cf44427978213d9`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3591cdb3085035cae7990a6e9575e7600a3d7d0b76ee4754c4cfd67f9756222f`  
		Last Modified: Tue, 06 Sep 2022 20:01:40 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027c634b9ed975106083869c1a6bc728a99d18c5bb108b1f24e03d821ee62e5`  
		Last Modified: Tue, 06 Sep 2022 20:01:32 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:ed6c5727dd691c93038d1c8eaf07c90ad8f94c80ae5029ba79f15fc77d11ae74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:5ec6cc285fdd2c5013a4369f539b46329b5abeb2f1ea8ee591a54dbee3f0c8ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232893306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935adb03164d1e08e5ac2411f80f0931671303b2eff0ce6e156f31921f87222e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:41:50 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:41:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:41:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 16:41:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:56 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:56 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 16:42:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 16:42:12 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 16:42:12 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:42:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:42:13 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:42:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55d7e27952550c878e39574ef5f7a687a84ee82af84b960475204994cc7b85`  
		Last Modified: Wed, 05 Oct 2022 16:43:33 GMT  
		Size: 91.5 MB (91515847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1417570fe4b9dc321fc36aa7ea824a4e3498fefc251bd8e58b5afd6d745f54`  
		Last Modified: Wed, 05 Oct 2022 16:43:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b68d2a3976336fad6abc36156e12c32e2a401e6e607dc91a5479259a3198a`  
		Last Modified: Wed, 05 Oct 2022 16:43:21 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266dc110117494e92f7b58387ff4d29670c803c37b0c99b0944dda29baea03`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 930.5 KB (930478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d2dff73b8f9b94aa905063c5704022fa9bb64a01a42d36975c235cf64ac8e`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7172813e2adc9a591a81a69db70059e410c9f36cc368481f252416963677601`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641657ee8ee5d0c68da40cbc72a00b625aa122301bc1caa0723344aee03bba03`  
		Last Modified: Wed, 05 Oct 2022 16:43:25 GMT  
		Size: 113.7 MB (113727928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c8a65aef90753ab97f3e21b73e29f9107a47f4c5bc6e88ecb5f03cc75d8b17`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4773b624c4630105a570178dd8e67ca28227921b769935c3fa7f569489e4bd5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224329170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f7f3ff412e8b3c99cdebdf6a3ef77bc68166ac6d9e1406bf6573111ec1a874`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:35:26 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:35:27 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:35:30 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:35:31 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:35:32 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:35:33 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:35:34 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:35:35 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:35:36 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 15:35:37 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 15:35:38 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 15:35:39 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:35:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:42 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:35:44 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 15:35:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 15:35:53 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 15:35:54 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:35:56 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:35:56 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:35:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2502bdaa7fb7beb25b710ccd1790cd1b2809e27c3dd5c46d4c4dba83d203db`  
		Last Modified: Wed, 05 Oct 2022 15:37:37 GMT  
		Size: 86.0 MB (86000050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec5e7938cf270930204c8ffd250f418f2e236a2e68f5ea5d82ab69df3001bd`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f631755389173aaf52aa72ba42646f457f3b67dcf29eac1c306f69945513485`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab611dddc527ad69c9cfa9e09313fb3c2a1ca7e1ce8252fade1d2f75b25815f1`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 859.5 KB (859530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615141c9b889b095f1947bb0315866344021a09635b522538754fc1c35412f98`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7ac7a764faba6ce254b68df36034e0ecf93b7018d31a0ba939a2bf368d86e9`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a799ecc2f3331250c473855a103f9cec1e4f28c436f4080f65df40888fb9cd1a`  
		Last Modified: Wed, 05 Oct 2022 15:37:35 GMT  
		Size: 113.7 MB (113727905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1a80e7cbbb2d6e6dcb35691ffaaae1cd720257b868f8ef1cf257f630346a7b`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:1e6578d8b4c3d62db481d25359b9f79d05166773f772ab86ea525bdac7bb3b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231787296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61bd4165a10292b247997ab6b1c2cf889953636d85084e7a366afcff2bc9a398`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:35 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:59:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:59:40 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 06 Sep 2022 19:59:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:44 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:59:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 06 Sep 2022 19:59:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 06 Sep 2022 19:59:59 GMT
ENV HTTP_API=false
# Tue, 06 Sep 2022 20:00:00 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 20:00:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 20:00:03 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 20:00:04 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8548f8c22e40d7e54097152f5b0da59a6ab2706ce9c294478a909de6a50782b7`  
		Last Modified: Tue, 06 Sep 2022 20:02:17 GMT  
		Size: 86.8 MB (86778981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa2696d5bc76b7b6f73c8606192002ed308d337fa1b2df7c169dca132344e6`  
		Last Modified: Tue, 06 Sep 2022 20:01:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a945ad1159d41018f6988b4621b18077f63b648fa86e2b3555e41848ad9490`  
		Last Modified: Tue, 06 Sep 2022 20:01:59 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca18b4ec34bc35ab22334b49712435c6120b552f4872d350742a7b60adb6cb2`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 831.6 KB (831571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8624f8cc60c44790f133f9525a2c3463c48a0f35b3434aa646c4faf8e0c1c4c5`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f26edf16545b401a0ccc43e3e284c45cbe8fe6ad064b919b43af69b4ccd563`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9095349011839ef32cdac2a80bb5534c76ab9ff79f419bae57abf6f2dcdff0cd`  
		Last Modified: Tue, 06 Sep 2022 20:02:07 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe1b0502c594aa53c8e26b703ce82124e11cf7a76f11d29000d385bb4eace9d`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:ed6c5727dd691c93038d1c8eaf07c90ad8f94c80ae5029ba79f15fc77d11ae74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:5ec6cc285fdd2c5013a4369f539b46329b5abeb2f1ea8ee591a54dbee3f0c8ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232893306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935adb03164d1e08e5ac2411f80f0931671303b2eff0ce6e156f31921f87222e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:39:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 16:41:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:41:50 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 16:41:51 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 16:41:54 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 16:41:54 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 16:41:55 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 16:41:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 16:41:56 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 16:41:56 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 16:42:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 16:42:12 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 16:42:12 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 16:42:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 16:42:13 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 16:42:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55d7e27952550c878e39574ef5f7a687a84ee82af84b960475204994cc7b85`  
		Last Modified: Wed, 05 Oct 2022 16:43:33 GMT  
		Size: 91.5 MB (91515847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1417570fe4b9dc321fc36aa7ea824a4e3498fefc251bd8e58b5afd6d745f54`  
		Last Modified: Wed, 05 Oct 2022 16:43:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b68d2a3976336fad6abc36156e12c32e2a401e6e607dc91a5479259a3198a`  
		Last Modified: Wed, 05 Oct 2022 16:43:21 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1266dc110117494e92f7b58387ff4d29670c803c37b0c99b0944dda29baea03`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 930.5 KB (930478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d2dff73b8f9b94aa905063c5704022fa9bb64a01a42d36975c235cf64ac8e`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7172813e2adc9a591a81a69db70059e410c9f36cc368481f252416963677601`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641657ee8ee5d0c68da40cbc72a00b625aa122301bc1caa0723344aee03bba03`  
		Last Modified: Wed, 05 Oct 2022 16:43:25 GMT  
		Size: 113.7 MB (113727928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c8a65aef90753ab97f3e21b73e29f9107a47f4c5bc6e88ecb5f03cc75d8b17`  
		Last Modified: Wed, 05 Oct 2022 16:43:19 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:4773b624c4630105a570178dd8e67ca28227921b769935c3fa7f569489e4bd5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224329170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f7f3ff412e8b3c99cdebdf6a3ef77bc68166ac6d9e1406bf6573111ec1a874`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:02 GMT
ADD file:4beae13e1fd7bb92776c08a5cd95feb81b8b3c80522ed8513f2441adfb1661ac in / 
# Wed, 05 Oct 2022 00:02:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:33:23 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 15:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:35:26 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 15:35:27 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 15:35:30 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 15:35:31 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 15:35:32 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 15:35:33 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 15:35:34 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 15:35:35 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 15:35:36 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 15:35:37 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 15:35:38 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 15:35:39 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:40 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 15:35:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 15:35:42 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 15:35:44 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 15:35:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 15:35:53 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 15:35:54 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 15:35:56 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 15:35:56 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 15:35:57 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:0e9b69cf8198dafe5b7db1eee7b96b96238f8346ec641dd44f961f7996c2c152`  
		Last Modified: Wed, 05 Oct 2022 00:03:33 GMT  
		Size: 23.7 MB (23734594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2502bdaa7fb7beb25b710ccd1790cd1b2809e27c3dd5c46d4c4dba83d203db`  
		Last Modified: Wed, 05 Oct 2022 15:37:37 GMT  
		Size: 86.0 MB (86000050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aec5e7938cf270930204c8ffd250f418f2e236a2e68f5ea5d82ab69df3001bd`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f631755389173aaf52aa72ba42646f457f3b67dcf29eac1c306f69945513485`  
		Last Modified: Wed, 05 Oct 2022 15:37:25 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab611dddc527ad69c9cfa9e09313fb3c2a1ca7e1ce8252fade1d2f75b25815f1`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 859.5 KB (859530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615141c9b889b095f1947bb0315866344021a09635b522538754fc1c35412f98`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7ac7a764faba6ce254b68df36034e0ecf93b7018d31a0ba939a2bf368d86e9`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 3.3 KB (3309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a799ecc2f3331250c473855a103f9cec1e4f28c436f4080f65df40888fb9cd1a`  
		Last Modified: Wed, 05 Oct 2022 15:37:35 GMT  
		Size: 113.7 MB (113727905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1a80e7cbbb2d6e6dcb35691ffaaae1cd720257b868f8ef1cf257f630346a7b`  
		Last Modified: Wed, 05 Oct 2022 15:37:23 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:1e6578d8b4c3d62db481d25359b9f79d05166773f772ab86ea525bdac7bb3b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231787296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61bd4165a10292b247997ab6b1c2cf889953636d85084e7a366afcff2bc9a398`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 06 Sep 2022 19:59:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:35 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 06 Sep 2022 19:59:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 06 Sep 2022 19:59:40 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BONITA_VERSION
# Tue, 06 Sep 2022 19:59:40 GMT
ARG BRANDING_VERSION
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_SHA256
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BASE_URL
# Tue, 06 Sep 2022 19:59:41 GMT
ARG BONITA_URL
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_VERSION=7.13.0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BRANDING_VERSION=2021.2-u0
# Tue, 06 Sep 2022 19:59:42 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Tue, 06 Sep 2022 19:59:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 06 Sep 2022 19:59:43 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Tue, 06 Sep 2022 19:59:44 GMT
RUN mkdir /opt/files
# Tue, 06 Sep 2022 19:59:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Tue, 06 Sep 2022 19:59:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Tue, 06 Sep 2022 19:59:59 GMT
ENV HTTP_API=false
# Tue, 06 Sep 2022 20:00:00 GMT
VOLUME [/opt/bonita]
# Tue, 06 Sep 2022 20:00:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 06 Sep 2022 20:00:03 GMT
EXPOSE 8080
# Tue, 06 Sep 2022 20:00:04 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8548f8c22e40d7e54097152f5b0da59a6ab2706ce9c294478a909de6a50782b7`  
		Last Modified: Tue, 06 Sep 2022 20:02:17 GMT  
		Size: 86.8 MB (86778981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa2696d5bc76b7b6f73c8606192002ed308d337fa1b2df7c169dca132344e6`  
		Last Modified: Tue, 06 Sep 2022 20:01:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a945ad1159d41018f6988b4621b18077f63b648fa86e2b3555e41848ad9490`  
		Last Modified: Tue, 06 Sep 2022 20:01:59 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca18b4ec34bc35ab22334b49712435c6120b552f4872d350742a7b60adb6cb2`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 831.6 KB (831571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8624f8cc60c44790f133f9525a2c3463c48a0f35b3434aa646c4faf8e0c1c4c5`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f26edf16545b401a0ccc43e3e284c45cbe8fe6ad064b919b43af69b4ccd563`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 3.3 KB (3305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9095349011839ef32cdac2a80bb5534c76ab9ff79f419bae57abf6f2dcdff0cd`  
		Last Modified: Tue, 06 Sep 2022 20:02:07 GMT  
		Size: 113.7 MB (113727916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe1b0502c594aa53c8e26b703ce82124e11cf7a76f11d29000d385bb4eace9d`  
		Last Modified: Tue, 06 Sep 2022 20:01:56 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:977f4e8862be31d76a5a463b0238a58fcd4af483ea1c6d6cb1ed75a1447c0d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:08cde8fece645d8b60bc13cf85691f0a092238a270c1a95554fc71714cd25237
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b7a73741c772da78e05b71140aeaa6e2838bcfef7277b7af94e3813db00ebb`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:15:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:15:47 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:15:48 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:15:49 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:50 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:15:50 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:16:01 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:16:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:16:03 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:16:03 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:16:03 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:16:03 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:16:03 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e40e66c88000cdcf6a5f303ff471b71908973b42e6d2c853ebafc528c1f58d`  
		Last Modified: Tue, 09 Aug 2022 18:16:38 GMT  
		Size: 60.8 MB (60808791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8517b429307545f8abc13fc0b37faa4607093e758af1d721cd166a9c9d59ec60`  
		Last Modified: Tue, 09 Aug 2022 18:16:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a90d8fa310d2a6ea37f38a5d6783134999b8e41a9a6cea96f56c35fef2514e`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7082e206c7455f0f4b81da210af350e50379ccb7f4d413868083cb6bd93fb7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afa20c272a36d9fffe827f8ce399a488ef133030401d5e3892cb8f30b9ab2c7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9086b05d70c72cfe77142c9829855c34c099504b88df663d5d954537502aef`  
		Last Modified: Tue, 09 Aug 2022 18:16:34 GMT  
		Size: 116.7 MB (116690829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153200db9a09f679584a791a878014d3dcdf52d99869e37107b43db18c4d9cc3`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9659f7730d354083e732097fd3656a47ab26b8c4f2010683fc2fbe6358cd9dad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30779f62863399675fedee53f8a02f2a0fea94360bde10754580989873e9ef13`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:18:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:18:36 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:18:36 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:18:37 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:18:38 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:18:39 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:18:40 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:18:41 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:18:42 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:18:43 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:18:44 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:18:45 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:18:46 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:18:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:49 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:18:51 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:19:04 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:19:05 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:19:06 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:19:07 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:19:08 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:19:09 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:19:10 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:19:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:19:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:19:13 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:19:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:19:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:19:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:19:17 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:19:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:19:19 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:19:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc88915541d6f4421b66a886f25f68b9655dc1dee732760c3086d5e8b3304a4a`  
		Last Modified: Tue, 09 Aug 2022 18:20:24 GMT  
		Size: 60.1 MB (60129514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bc8304739386ec9aab2a1dcd52eb85ca85059ce787cc536f24934bb6907c1`  
		Last Modified: Tue, 09 Aug 2022 18:20:16 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f5f51932f11b34b80147eec1268be25c87b241a595d18adb836b09480ebee6`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec51c34c596f0fcdf1cc75e2c3154642dc1e041ed2d502ad3468cbf5ee7633a`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccaa414eaa82b83c723b3217df9302e719890e1ceacda1452c141980ae6f5d`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 3.0 KB (3002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334448ededff63c05c8efe4578487e4b1ad071d95373c4c39515f1c33472d788`  
		Last Modified: Tue, 09 Aug 2022 18:20:17 GMT  
		Size: 116.7 MB (116688789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61a4040e3817598cff22a8fae45d9f16a5d5f8703e2acef71454e5df2d9889`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:905376aad5c6b1828a693ea6913e13ee18e890176d32e306d9f9d015ddd0b228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7c95b1e8662e1c67b791b144f27360f33bf8c5a12aa9beb134ef618268006`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:57:05 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 10 Aug 2022 02:57:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 10 Aug 2022 02:57:16 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 10 Aug 2022 02:57:18 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BRANDING_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_SHA256
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BASE_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ARG BONITA_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 10 Aug 2022 02:57:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:23 GMT
RUN mkdir /opt/files
# Wed, 10 Aug 2022 02:57:23 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 10 Aug 2022 02:57:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API=false
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 10 Aug 2022 02:57:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 10 Aug 2022 02:57:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 10 Aug 2022 02:57:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 10 Aug 2022 02:57:44 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 10 Aug 2022 02:57:44 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 10 Aug 2022 02:57:44 GMT
EXPOSE 8080 9000
# Wed, 10 Aug 2022 02:57:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 10 Aug 2022 02:57:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd0e6368901462206ecfbedd1db3517fe94f68bc7b57918c328df47fbdbbf3`  
		Last Modified: Wed, 10 Aug 2022 02:58:51 GMT  
		Size: 56.6 MB (56628364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2f41beebf7247171a5b275e0598e9ed16be2ad6ffa16ad4c9c8f036f8800f1`  
		Last Modified: Wed, 10 Aug 2022 02:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d583bf09d162033ea6a52f524d3142e51ab87f5ce8e1c17c918e8c47527016c`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593fae9e149af994c09345a3dcb015f0959fed2dd20e229f5fafea90d08f429b`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96057fb9286d4d93de5c991d820e3b03be1923bec7ea58592b8417b9f69368bc`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77133cc538711ede4f9dda1c5d44ea027f26326760bb0136c00411045f62d0d`  
		Last Modified: Wed, 10 Aug 2022 02:58:47 GMT  
		Size: 116.7 MB (116690853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933c622a69b13e9df15b3809c6323b98b3a6e697a0ce37025afde53920527a41`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:977f4e8862be31d76a5a463b0238a58fcd4af483ea1c6d6cb1ed75a1447c0d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:08cde8fece645d8b60bc13cf85691f0a092238a270c1a95554fc71714cd25237
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b7a73741c772da78e05b71140aeaa6e2838bcfef7277b7af94e3813db00ebb`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:15:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:15:47 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:15:48 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:15:49 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:50 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:15:50 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:16:01 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:16:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:16:03 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:16:03 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:16:03 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:16:03 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:16:03 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e40e66c88000cdcf6a5f303ff471b71908973b42e6d2c853ebafc528c1f58d`  
		Last Modified: Tue, 09 Aug 2022 18:16:38 GMT  
		Size: 60.8 MB (60808791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8517b429307545f8abc13fc0b37faa4607093e758af1d721cd166a9c9d59ec60`  
		Last Modified: Tue, 09 Aug 2022 18:16:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a90d8fa310d2a6ea37f38a5d6783134999b8e41a9a6cea96f56c35fef2514e`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7082e206c7455f0f4b81da210af350e50379ccb7f4d413868083cb6bd93fb7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afa20c272a36d9fffe827f8ce399a488ef133030401d5e3892cb8f30b9ab2c7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9086b05d70c72cfe77142c9829855c34c099504b88df663d5d954537502aef`  
		Last Modified: Tue, 09 Aug 2022 18:16:34 GMT  
		Size: 116.7 MB (116690829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153200db9a09f679584a791a878014d3dcdf52d99869e37107b43db18c4d9cc3`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9659f7730d354083e732097fd3656a47ab26b8c4f2010683fc2fbe6358cd9dad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30779f62863399675fedee53f8a02f2a0fea94360bde10754580989873e9ef13`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:18:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:18:36 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:18:36 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:18:37 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:18:38 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:18:39 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:18:40 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:18:41 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:18:42 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:18:43 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:18:44 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:18:45 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:18:46 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:18:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:49 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:18:51 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:19:04 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:19:05 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:19:06 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:19:07 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:19:08 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:19:09 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:19:10 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:19:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:19:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:19:13 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:19:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:19:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:19:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:19:17 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:19:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:19:19 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:19:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc88915541d6f4421b66a886f25f68b9655dc1dee732760c3086d5e8b3304a4a`  
		Last Modified: Tue, 09 Aug 2022 18:20:24 GMT  
		Size: 60.1 MB (60129514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bc8304739386ec9aab2a1dcd52eb85ca85059ce787cc536f24934bb6907c1`  
		Last Modified: Tue, 09 Aug 2022 18:20:16 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f5f51932f11b34b80147eec1268be25c87b241a595d18adb836b09480ebee6`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec51c34c596f0fcdf1cc75e2c3154642dc1e041ed2d502ad3468cbf5ee7633a`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccaa414eaa82b83c723b3217df9302e719890e1ceacda1452c141980ae6f5d`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 3.0 KB (3002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334448ededff63c05c8efe4578487e4b1ad071d95373c4c39515f1c33472d788`  
		Last Modified: Tue, 09 Aug 2022 18:20:17 GMT  
		Size: 116.7 MB (116688789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61a4040e3817598cff22a8fae45d9f16a5d5f8703e2acef71454e5df2d9889`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:905376aad5c6b1828a693ea6913e13ee18e890176d32e306d9f9d015ddd0b228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7c95b1e8662e1c67b791b144f27360f33bf8c5a12aa9beb134ef618268006`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:57:05 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 10 Aug 2022 02:57:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 10 Aug 2022 02:57:16 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 10 Aug 2022 02:57:18 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BRANDING_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_SHA256
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BASE_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ARG BONITA_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 10 Aug 2022 02:57:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:23 GMT
RUN mkdir /opt/files
# Wed, 10 Aug 2022 02:57:23 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 10 Aug 2022 02:57:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API=false
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 10 Aug 2022 02:57:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 10 Aug 2022 02:57:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 10 Aug 2022 02:57:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 10 Aug 2022 02:57:44 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 10 Aug 2022 02:57:44 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 10 Aug 2022 02:57:44 GMT
EXPOSE 8080 9000
# Wed, 10 Aug 2022 02:57:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 10 Aug 2022 02:57:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd0e6368901462206ecfbedd1db3517fe94f68bc7b57918c328df47fbdbbf3`  
		Last Modified: Wed, 10 Aug 2022 02:58:51 GMT  
		Size: 56.6 MB (56628364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2f41beebf7247171a5b275e0598e9ed16be2ad6ffa16ad4c9c8f036f8800f1`  
		Last Modified: Wed, 10 Aug 2022 02:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d583bf09d162033ea6a52f524d3142e51ab87f5ce8e1c17c918e8c47527016c`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593fae9e149af994c09345a3dcb015f0959fed2dd20e229f5fafea90d08f429b`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96057fb9286d4d93de5c991d820e3b03be1923bec7ea58592b8417b9f69368bc`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77133cc538711ede4f9dda1c5d44ea027f26326760bb0136c00411045f62d0d`  
		Last Modified: Wed, 10 Aug 2022 02:58:47 GMT  
		Size: 116.7 MB (116690853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933c622a69b13e9df15b3809c6323b98b3a6e697a0ce37025afde53920527a41`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:977f4e8862be31d76a5a463b0238a58fcd4af483ea1c6d6cb1ed75a1447c0d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:08cde8fece645d8b60bc13cf85691f0a092238a270c1a95554fc71714cd25237
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b7a73741c772da78e05b71140aeaa6e2838bcfef7277b7af94e3813db00ebb`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:15:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:15:47 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:15:48 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:15:48 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:15:49 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:15:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:15:50 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:15:50 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:16:01 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:16:02 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:16:02 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:16:02 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:16:02 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:16:03 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:16:03 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:16:03 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:16:03 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:16:03 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:16:03 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e40e66c88000cdcf6a5f303ff471b71908973b42e6d2c853ebafc528c1f58d`  
		Last Modified: Tue, 09 Aug 2022 18:16:38 GMT  
		Size: 60.8 MB (60808791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8517b429307545f8abc13fc0b37faa4607093e758af1d721cd166a9c9d59ec60`  
		Last Modified: Tue, 09 Aug 2022 18:16:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a90d8fa310d2a6ea37f38a5d6783134999b8e41a9a6cea96f56c35fef2514e`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7082e206c7455f0f4b81da210af350e50379ccb7f4d413868083cb6bd93fb7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afa20c272a36d9fffe827f8ce399a488ef133030401d5e3892cb8f30b9ab2c7`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 3.0 KB (3034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9086b05d70c72cfe77142c9829855c34c099504b88df663d5d954537502aef`  
		Last Modified: Tue, 09 Aug 2022 18:16:34 GMT  
		Size: 116.7 MB (116690829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153200db9a09f679584a791a878014d3dcdf52d99869e37107b43db18c4d9cc3`  
		Last Modified: Tue, 09 Aug 2022 18:16:27 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9659f7730d354083e732097fd3656a47ab26b8c4f2010683fc2fbe6358cd9dad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30779f62863399675fedee53f8a02f2a0fea94360bde10754580989873e9ef13`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:18:32 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 09 Aug 2022 18:18:36 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Tue, 09 Aug 2022 18:18:36 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 09 Aug 2022 18:18:37 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Tue, 09 Aug 2022 18:18:38 GMT
ARG BONITA_VERSION
# Tue, 09 Aug 2022 18:18:39 GMT
ARG BRANDING_VERSION
# Tue, 09 Aug 2022 18:18:40 GMT
ARG BONITA_SHA256
# Tue, 09 Aug 2022 18:18:41 GMT
ARG BASE_URL
# Tue, 09 Aug 2022 18:18:42 GMT
ARG BONITA_URL
# Tue, 09 Aug 2022 18:18:43 GMT
ENV BONITA_VERSION=7.14.0
# Tue, 09 Aug 2022 18:18:44 GMT
ENV BRANDING_VERSION=2022.1-u0
# Tue, 09 Aug 2022 18:18:45 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Tue, 09 Aug 2022 18:18:46 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 09 Aug 2022 18:18:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Tue, 09 Aug 2022 18:18:49 GMT
RUN mkdir /opt/files
# Tue, 09 Aug 2022 18:18:51 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Tue, 09 Aug 2022 18:19:04 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Tue, 09 Aug 2022 18:19:05 GMT
ENV HTTP_API=false
# Tue, 09 Aug 2022 18:19:06 GMT
ENV HTTP_API_USERNAME=http-api
# Tue, 09 Aug 2022 18:19:07 GMT
ENV HTTP_API_PASSWORD=
# Tue, 09 Aug 2022 18:19:08 GMT
ENV MONITORING_USERNAME=monitoring
# Tue, 09 Aug 2022 18:19:09 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Tue, 09 Aug 2022 18:19:10 GMT
ENV JMX_REMOTE_ACCESS=false
# Tue, 09 Aug 2022 18:19:11 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Tue, 09 Aug 2022 18:19:12 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Tue, 09 Aug 2022 18:19:13 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Tue, 09 Aug 2022 18:19:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Tue, 09 Aug 2022 18:19:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Tue, 09 Aug 2022 18:19:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Tue, 09 Aug 2022 18:19:17 GMT
ENV HTTP_MAX_THREADS=20
# Tue, 09 Aug 2022 18:19:19 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Tue, 09 Aug 2022 18:19:19 GMT
EXPOSE 8080 9000
# Tue, 09 Aug 2022 18:19:20 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Tue, 09 Aug 2022 18:19:21 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc88915541d6f4421b66a886f25f68b9655dc1dee732760c3086d5e8b3304a4a`  
		Last Modified: Tue, 09 Aug 2022 18:20:24 GMT  
		Size: 60.1 MB (60129514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bc8304739386ec9aab2a1dcd52eb85ca85059ce787cc536f24934bb6907c1`  
		Last Modified: Tue, 09 Aug 2022 18:20:16 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f5f51932f11b34b80147eec1268be25c87b241a595d18adb836b09480ebee6`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec51c34c596f0fcdf1cc75e2c3154642dc1e041ed2d502ad3468cbf5ee7633a`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccaa414eaa82b83c723b3217df9302e719890e1ceacda1452c141980ae6f5d`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 3.0 KB (3002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334448ededff63c05c8efe4578487e4b1ad071d95373c4c39515f1c33472d788`  
		Last Modified: Tue, 09 Aug 2022 18:20:17 GMT  
		Size: 116.7 MB (116688789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61a4040e3817598cff22a8fae45d9f16a5d5f8703e2acef71454e5df2d9889`  
		Last Modified: Tue, 09 Aug 2022 18:20:13 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:905376aad5c6b1828a693ea6913e13ee18e890176d32e306d9f9d015ddd0b228
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7c95b1e8662e1c67b791b144f27360f33bf8c5a12aa9beb134ef618268006`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:57:05 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 10 Aug 2022 02:57:14 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Wed, 10 Aug 2022 02:57:16 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 10 Aug 2022 02:57:18 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BRANDING_VERSION
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BONITA_SHA256
# Wed, 10 Aug 2022 02:57:19 GMT
ARG BASE_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ARG BONITA_URL
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BONITA_VERSION=7.14.0
# Wed, 10 Aug 2022 02:57:20 GMT
ENV BRANDING_VERSION=2022.1-u0
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Wed, 10 Aug 2022 02:57:21 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 10 Aug 2022 02:57:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Wed, 10 Aug 2022 02:57:23 GMT
RUN mkdir /opt/files
# Wed, 10 Aug 2022 02:57:23 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Wed, 10 Aug 2022 02:57:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API=false
# Wed, 10 Aug 2022 02:57:39 GMT
ENV HTTP_API_USERNAME=http-api
# Wed, 10 Aug 2022 02:57:40 GMT
ENV HTTP_API_PASSWORD=
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_USERNAME=monitoring
# Wed, 10 Aug 2022 02:57:40 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Wed, 10 Aug 2022 02:57:41 GMT
ENV JMX_REMOTE_ACCESS=false
# Wed, 10 Aug 2022 02:57:41 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Wed, 10 Aug 2022 02:57:42 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Wed, 10 Aug 2022 02:57:43 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Wed, 10 Aug 2022 02:57:44 GMT
ENV HTTP_MAX_THREADS=20
# Wed, 10 Aug 2022 02:57:44 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Wed, 10 Aug 2022 02:57:44 GMT
EXPOSE 8080 9000
# Wed, 10 Aug 2022 02:57:45 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Wed, 10 Aug 2022 02:57:45 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd0e6368901462206ecfbedd1db3517fe94f68bc7b57918c328df47fbdbbf3`  
		Last Modified: Wed, 10 Aug 2022 02:58:51 GMT  
		Size: 56.6 MB (56628364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2f41beebf7247171a5b275e0598e9ed16be2ad6ffa16ad4c9c8f036f8800f1`  
		Last Modified: Wed, 10 Aug 2022 02:58:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d583bf09d162033ea6a52f524d3142e51ab87f5ce8e1c17c918e8c47527016c`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593fae9e149af994c09345a3dcb015f0959fed2dd20e229f5fafea90d08f429b`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96057fb9286d4d93de5c991d820e3b03be1923bec7ea58592b8417b9f69368bc`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77133cc538711ede4f9dda1c5d44ea027f26326760bb0136c00411045f62d0d`  
		Last Modified: Wed, 10 Aug 2022 02:58:47 GMT  
		Size: 116.7 MB (116690853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933c622a69b13e9df15b3809c6323b98b3a6e697a0ce37025afde53920527a41`  
		Last Modified: Wed, 10 Aug 2022 02:58:36 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
