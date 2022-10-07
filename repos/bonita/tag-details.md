<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:2021.2`](#bonita20212)
-	[`bonita:2021.2-u0`](#bonita20212-u0)
-	[`bonita:2022.1`](#bonita20221)
-	[`bonita:2022.1-u0`](#bonita20221-u0)
-	[`bonita:2022.2`](#bonita20222)
-	[`bonita:2022.2-u0`](#bonita20222-u0)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:7.13`](#bonita713)
-	[`bonita:7.13.0`](#bonita7130)
-	[`bonita:7.14`](#bonita714)
-	[`bonita:7.14.0`](#bonita7140)
-	[`bonita:7.15`](#bonita715)
-	[`bonita:7.15.0`](#bonita7150)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:c4dfd932a248cc4c5043cbc8e948ecd99dc3f0ee0a6d2586eccb15996adcb9ba
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
$ docker pull bonita@sha256:f70def9d67125c205708688b13d1c9de4e42528839dca3297ea30e719ddb3151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234123216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fe908e53db5f3ba2be7eef1c7066ce35e743f7736f647aa54499ea3ec4a89d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:42:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:42:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:42:15 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:42:19 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:42:19 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:42:47 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 18:42:48 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 18:42:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:42:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 18:42:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 18:42:51 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:42:51 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 18:43:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 18:43:09 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 18:43:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 18:43:11 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:43:12 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65434190d8d0b310da61bd4a0c9803eafe3aaef0288085588b6f45b6d54e031`  
		Last Modified: Wed, 05 Oct 2022 18:45:45 GMT  
		Size: 86.8 MB (86779064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2732e23275ee1da8786e079deae810600f99c6fa09fc13b5ca4dd42ac67ff42`  
		Last Modified: Wed, 05 Oct 2022 18:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2790f9dce24ed4c863e7cfc3059c4fd0a843ddb8281651c79088ee5a20f27e19`  
		Last Modified: Wed, 05 Oct 2022 18:45:25 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86240b0ade55ae53beb11330c6ca00b10fa1f26ecf9811f54503459eb97bf4a2`  
		Last Modified: Wed, 05 Oct 2022 18:45:24 GMT  
		Size: 475.3 KB (475348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cacef0dbceb7ef9527fa2a04838a23406b28fe204ba0b42f26f570c0d85a34a`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed253dc6a17b72e0b0a41d81c9f15e347107836549c9e33bcba90553b1629985`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99adf8cb9165fe94b1d5448901445e2c49b0980d1fb83c061f6d4ca8c3cf45e`  
		Last Modified: Wed, 05 Oct 2022 18:46:07 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bd4fe35530481c24f429204008ff1582957f98ce98344a2b67b15b28c1ab9c`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:0d49a65293fcd6ff14ddffb804c637be836cb3cba66a6fa09766773106b0d127
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
$ docker pull bonita@sha256:9cb8e349b2bf6d4d8a1d67a572691c9f0a4ec97b85d2a9692ab2e6405c6044f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231788382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36eeb3c8ad8d36ed7a9a74232c77a82c0c1538b08a812aefbdc03de075a3c784`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:44:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:44:04 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:44:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:44:09 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:44:09 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 18:44:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:44:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:14 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:44:14 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 18:44:26 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 18:44:28 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 18:44:30 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:44:30 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:44:32 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:44:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f9e39a6a7f63873a2dc20d23d5c8d1fc5fa58eae6190c7105001b2c8d9894c`  
		Last Modified: Wed, 05 Oct 2022 18:46:45 GMT  
		Size: 86.8 MB (86779112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ea1151120c9f1f0f613e0ed92eeed3084bf66c8c45ac449f780d480247a08b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db734224771944745348b76c383673051a02f2d64bb9c5b69f3c4e8520d7765b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea716d20ae0b2b5be4d4fe4548c9e198ee759216b8e1047d64e406db51473`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 831.6 KB (831575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d394e8f62f1973732d5656c2400bb2b98241d96edf0b1cd1c24be144ca21a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcb40ceb70f178b47382a06a174c6308324d85011f65472380a43e4693db4f`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ea30fddaf1a1df0a83bc3e29628cc996b0a811b7b7689ab9122c188ef8defb`  
		Last Modified: Wed, 05 Oct 2022 18:46:33 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ecf65c2498bc270470ae0c9abfdb8dea80371ecf7b301490f6ee08aa79060a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:0d49a65293fcd6ff14ddffb804c637be836cb3cba66a6fa09766773106b0d127
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
$ docker pull bonita@sha256:9cb8e349b2bf6d4d8a1d67a572691c9f0a4ec97b85d2a9692ab2e6405c6044f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231788382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36eeb3c8ad8d36ed7a9a74232c77a82c0c1538b08a812aefbdc03de075a3c784`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:44:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:44:04 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:44:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:44:09 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:44:09 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 18:44:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:44:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:14 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:44:14 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 18:44:26 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 18:44:28 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 18:44:30 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:44:30 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:44:32 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:44:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f9e39a6a7f63873a2dc20d23d5c8d1fc5fa58eae6190c7105001b2c8d9894c`  
		Last Modified: Wed, 05 Oct 2022 18:46:45 GMT  
		Size: 86.8 MB (86779112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ea1151120c9f1f0f613e0ed92eeed3084bf66c8c45ac449f780d480247a08b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db734224771944745348b76c383673051a02f2d64bb9c5b69f3c4e8520d7765b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea716d20ae0b2b5be4d4fe4548c9e198ee759216b8e1047d64e406db51473`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 831.6 KB (831575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d394e8f62f1973732d5656c2400bb2b98241d96edf0b1cd1c24be144ca21a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcb40ceb70f178b47382a06a174c6308324d85011f65472380a43e4693db4f`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ea30fddaf1a1df0a83bc3e29628cc996b0a811b7b7689ab9122c188ef8defb`  
		Last Modified: Wed, 05 Oct 2022 18:46:33 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ecf65c2498bc270470ae0c9abfdb8dea80371ecf7b301490f6ee08aa79060a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1`

```console
$ docker pull bonita@sha256:f9e3cf341d6c539317a09231e40cb9ea7aa57b422d4d7a03ce4bb455226d240c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:67e41d4134c19e4a1966b0c0193542c4afc452996461d1c55d4c41e3617dc4b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fe400a159423f451be8962b98c0ad9a8b2864f91e161025fa32a0cfe37e25d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:52:48 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:52:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:52:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:52:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:52:55 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:52:56 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:52:57 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:52:58 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:52:59 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:53:00 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:53:01 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:53:02 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:53:03 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:53:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:06 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:53:08 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:53:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:53:16 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:53:17 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:53:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:53:19 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:53:20 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:53:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:53:22 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:53:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:53:24 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:53:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:53:26 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:53:27 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:53:28 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:53:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:53:30 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:53:31 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:53:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a72dcffd05869e5d752c06042ca884a4a8b1cc5e45920f2091bf0074f91a1`  
		Last Modified: Thu, 06 Oct 2022 19:54:26 GMT  
		Size: 60.1 MB (60129767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c53dea9976f27698da497a98de6604659903be074da8046acc0efd2336bcdc`  
		Last Modified: Thu, 06 Oct 2022 19:54:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd9113513200994b4f8363b9a3ff7d6d618fb2f1690272f476e6e42b8ba0dc2`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2dc70af30020f1fd49a24cec2bcce85130941d5c41c6dbcb5e33760e80b1e`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e37ee56ee4a54b64dc500b91def3e43575c3b4468aa1200e8ff420d00eaad`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 3.0 KB (3000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6172ff1fd0d733339e8a27557a5d788212a4f42b7491bdd830543603ab2bedf`  
		Last Modified: Thu, 06 Oct 2022 19:54:25 GMT  
		Size: 116.7 MB (116688760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2348246f4562d42618128248d56903c98195e7fb74f255d4296cc55b03a92c`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.1-u0`

```console
$ docker pull bonita@sha256:f9e3cf341d6c539317a09231e40cb9ea7aa57b422d4d7a03ce4bb455226d240c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.1-u0` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:67e41d4134c19e4a1966b0c0193542c4afc452996461d1c55d4c41e3617dc4b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fe400a159423f451be8962b98c0ad9a8b2864f91e161025fa32a0cfe37e25d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:52:48 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:52:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:52:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:52:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:52:55 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:52:56 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:52:57 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:52:58 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:52:59 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:53:00 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:53:01 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:53:02 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:53:03 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:53:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:06 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:53:08 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:53:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:53:16 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:53:17 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:53:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:53:19 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:53:20 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:53:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:53:22 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:53:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:53:24 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:53:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:53:26 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:53:27 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:53:28 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:53:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:53:30 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:53:31 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:53:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a72dcffd05869e5d752c06042ca884a4a8b1cc5e45920f2091bf0074f91a1`  
		Last Modified: Thu, 06 Oct 2022 19:54:26 GMT  
		Size: 60.1 MB (60129767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c53dea9976f27698da497a98de6604659903be074da8046acc0efd2336bcdc`  
		Last Modified: Thu, 06 Oct 2022 19:54:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd9113513200994b4f8363b9a3ff7d6d618fb2f1690272f476e6e42b8ba0dc2`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2dc70af30020f1fd49a24cec2bcce85130941d5c41c6dbcb5e33760e80b1e`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e37ee56ee4a54b64dc500b91def3e43575c3b4468aa1200e8ff420d00eaad`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 3.0 KB (3000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6172ff1fd0d733339e8a27557a5d788212a4f42b7491bdd830543603ab2bedf`  
		Last Modified: Thu, 06 Oct 2022 19:54:25 GMT  
		Size: 116.7 MB (116688760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2348246f4562d42618128248d56903c98195e7fb74f255d4296cc55b03a92c`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.1-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2`

```console
$ docker pull bonita@sha256:9326157dd76ba4fafc97e8380d64228cd53dfe369465e872e6d616c7a257b927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2` - linux; amd64

```console
$ docker pull bonita@sha256:96beb319839334dd24cf8b6cc849e68533fad89cf5aca869e1cc4ebc039d0f65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183206256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09da6c720099e834ec57a16315d0defea6cc1a1518380a596ffd3a868a9fdb59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:19:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:19:39 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:19:39 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:19:40 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:42 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:19:50 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:19:50 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:19:51 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:19:52 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:19:52 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:19:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:19:52 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:19:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:19:52 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5705f95d901e9d31f362e998a2c059acf47627969b042b4e7aaa72b533530e0`  
		Last Modified: Fri, 07 Oct 2022 19:20:29 GMT  
		Size: 61.2 MB (61197146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76059907474246c43b72aae8948b443645cfd4ab27e255f2555ba7a1f133806f`  
		Last Modified: Fri, 07 Oct 2022 19:20:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022b3528f0c93c13aeb319e8037b590351d556f7513d476a1da5d77734de820a`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c21d4b689cde4c6b32704ec260ace9395c580c5fd4403ec9691e367c6f91c`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af35cb2d6152fd421952af9e5bce9d544b5dd30338842f1d40c610fa142e2592`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202ed4e518b9784b3e9b2db17c26afe1be89539f86cea9362694f65fc089d70`  
		Last Modified: Fri, 07 Oct 2022 19:20:26 GMT  
		Size: 119.2 MB (119193019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bf2b5af323e9cc69f227a7c46ffdb4dd88609ecedc45a1a807120aa39fe89`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:678134bdb94e4f63cf83093514b25b71dfe9b347c97625e9a786aadd96ef6138
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182348091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce03089f322a258cae18ca28497bd1fa0fb756aae2b79915561d63c521a728`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:39:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:39:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:39:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:39:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:39:50 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:39:51 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:39:52 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:39:53 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:39:54 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:39:55 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:39:56 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:39:57 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:39:58 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:39:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:40:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:40:01 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:40:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:40:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:40:11 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:40:12 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:40:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:40:14 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:40:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:40:16 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:40:17 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:40:18 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:40:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:40:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:40:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:40:22 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:40:23 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:40:25 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:40:25 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:40:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:40:27 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497bd0e996de2d902f26a3023b901109ea46ec8d01ca2f527040175722bd069`  
		Last Modified: Fri, 07 Oct 2022 19:41:24 GMT  
		Size: 60.4 MB (60439220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe10e617bb9fab6e845f6c0feb39e110610ab11115ba462991c612f7a410fb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7bd7e5925381829a64c85fde46c63063cde25fe1a409cede494629ebbddb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8354d92c69b70dd6748ac85796528746adb07c9665e0686c52eeca5926e56a71`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 111.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17a0dcd655da714128f4233e36d2c2686818f3b524642fc1a4bd4ac143f735e`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d141b4d5dcee5ce2546270c1002d4a83d7458f062a52b9b7b41a3f75fb6276f`  
		Last Modified: Fri, 07 Oct 2022 19:41:27 GMT  
		Size: 119.2 MB (119191347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce674d50db2ba300dc2c6d26d93908e4c56432fa7f6d8047cd64999bf1dfe939`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:2c3128dbea0d3d5d8a63712d1db500fdecbc8b9d2995a695c37b4ebb80b5ef48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179326996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3838b00163be847a672d409b30519320813b30bf0947292136a897403f4be7`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:16:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:16:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:16:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:16:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:16:49 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:16:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:53 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:16:54 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:17:12 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:17:13 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:17:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:17:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:17:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:17:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:17:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:17:17 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:17:17 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:17:17 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c61989a45cdf74208e16d4c9fef94cee3d8eb10602f7ac45e023fb053dbf4e7`  
		Last Modified: Fri, 07 Oct 2022 19:18:27 GMT  
		Size: 57.3 MB (57320650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3fc5ec26c7a10b790182e0bc521d1c16847666abf323733fe17fb228c1839`  
		Last Modified: Fri, 07 Oct 2022 19:18:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2817209af0ad99735a5596f59d738933e465b7ef11feeaa492e45b842fb1a4cc`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d550240e348d5a213ea1a0d93c6108eb6c1d9a1936d7579c893c4cf91024ba1`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7105d16280bde13de94b8d7829efa1a960a706fae2772e49d24c0b8c0bad2`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5f0b41531d404e2a3e56f2983347537cec2d7cc8d0266e17897e3ef247be3`  
		Last Modified: Fri, 07 Oct 2022 19:18:22 GMT  
		Size: 119.2 MB (119192998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7377eb804f8177040817c5380de0d04576a7b288322ff9c5a3ee7305720e5313`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2022.2-u0`

```console
$ docker pull bonita@sha256:9326157dd76ba4fafc97e8380d64228cd53dfe369465e872e6d616c7a257b927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2022.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:96beb319839334dd24cf8b6cc849e68533fad89cf5aca869e1cc4ebc039d0f65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183206256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09da6c720099e834ec57a16315d0defea6cc1a1518380a596ffd3a868a9fdb59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:19:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:19:39 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:19:39 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:19:40 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:42 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:19:50 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:19:50 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:19:51 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:19:52 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:19:52 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:19:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:19:52 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:19:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:19:52 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5705f95d901e9d31f362e998a2c059acf47627969b042b4e7aaa72b533530e0`  
		Last Modified: Fri, 07 Oct 2022 19:20:29 GMT  
		Size: 61.2 MB (61197146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76059907474246c43b72aae8948b443645cfd4ab27e255f2555ba7a1f133806f`  
		Last Modified: Fri, 07 Oct 2022 19:20:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022b3528f0c93c13aeb319e8037b590351d556f7513d476a1da5d77734de820a`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c21d4b689cde4c6b32704ec260ace9395c580c5fd4403ec9691e367c6f91c`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af35cb2d6152fd421952af9e5bce9d544b5dd30338842f1d40c610fa142e2592`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202ed4e518b9784b3e9b2db17c26afe1be89539f86cea9362694f65fc089d70`  
		Last Modified: Fri, 07 Oct 2022 19:20:26 GMT  
		Size: 119.2 MB (119193019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bf2b5af323e9cc69f227a7c46ffdb4dd88609ecedc45a1a807120aa39fe89`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:678134bdb94e4f63cf83093514b25b71dfe9b347c97625e9a786aadd96ef6138
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182348091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce03089f322a258cae18ca28497bd1fa0fb756aae2b79915561d63c521a728`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:39:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:39:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:39:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:39:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:39:50 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:39:51 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:39:52 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:39:53 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:39:54 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:39:55 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:39:56 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:39:57 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:39:58 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:39:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:40:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:40:01 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:40:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:40:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:40:11 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:40:12 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:40:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:40:14 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:40:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:40:16 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:40:17 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:40:18 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:40:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:40:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:40:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:40:22 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:40:23 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:40:25 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:40:25 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:40:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:40:27 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497bd0e996de2d902f26a3023b901109ea46ec8d01ca2f527040175722bd069`  
		Last Modified: Fri, 07 Oct 2022 19:41:24 GMT  
		Size: 60.4 MB (60439220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe10e617bb9fab6e845f6c0feb39e110610ab11115ba462991c612f7a410fb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7bd7e5925381829a64c85fde46c63063cde25fe1a409cede494629ebbddb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8354d92c69b70dd6748ac85796528746adb07c9665e0686c52eeca5926e56a71`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 111.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17a0dcd655da714128f4233e36d2c2686818f3b524642fc1a4bd4ac143f735e`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d141b4d5dcee5ce2546270c1002d4a83d7458f062a52b9b7b41a3f75fb6276f`  
		Last Modified: Fri, 07 Oct 2022 19:41:27 GMT  
		Size: 119.2 MB (119191347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce674d50db2ba300dc2c6d26d93908e4c56432fa7f6d8047cd64999bf1dfe939`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2022.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:2c3128dbea0d3d5d8a63712d1db500fdecbc8b9d2995a695c37b4ebb80b5ef48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179326996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3838b00163be847a672d409b30519320813b30bf0947292136a897403f4be7`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:16:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:16:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:16:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:16:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:16:49 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:16:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:53 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:16:54 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:17:12 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:17:13 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:17:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:17:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:17:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:17:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:17:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:17:17 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:17:17 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:17:17 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c61989a45cdf74208e16d4c9fef94cee3d8eb10602f7ac45e023fb053dbf4e7`  
		Last Modified: Fri, 07 Oct 2022 19:18:27 GMT  
		Size: 57.3 MB (57320650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3fc5ec26c7a10b790182e0bc521d1c16847666abf323733fe17fb228c1839`  
		Last Modified: Fri, 07 Oct 2022 19:18:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2817209af0ad99735a5596f59d738933e465b7ef11feeaa492e45b842fb1a4cc`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d550240e348d5a213ea1a0d93c6108eb6c1d9a1936d7579c893c4cf91024ba1`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7105d16280bde13de94b8d7829efa1a960a706fae2772e49d24c0b8c0bad2`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5f0b41531d404e2a3e56f2983347537cec2d7cc8d0266e17897e3ef247be3`  
		Last Modified: Fri, 07 Oct 2022 19:18:22 GMT  
		Size: 119.2 MB (119192998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7377eb804f8177040817c5380de0d04576a7b288322ff9c5a3ee7305720e5313`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:c4dfd932a248cc4c5043cbc8e948ecd99dc3f0ee0a6d2586eccb15996adcb9ba
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
$ docker pull bonita@sha256:f70def9d67125c205708688b13d1c9de4e42528839dca3297ea30e719ddb3151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234123216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fe908e53db5f3ba2be7eef1c7066ce35e743f7736f647aa54499ea3ec4a89d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:42:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:42:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:42:15 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:42:19 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:42:19 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:42:47 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 18:42:48 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 18:42:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:42:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 18:42:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 18:42:51 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:42:51 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 18:43:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 18:43:09 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 18:43:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 18:43:11 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:43:12 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65434190d8d0b310da61bd4a0c9803eafe3aaef0288085588b6f45b6d54e031`  
		Last Modified: Wed, 05 Oct 2022 18:45:45 GMT  
		Size: 86.8 MB (86779064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2732e23275ee1da8786e079deae810600f99c6fa09fc13b5ca4dd42ac67ff42`  
		Last Modified: Wed, 05 Oct 2022 18:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2790f9dce24ed4c863e7cfc3059c4fd0a843ddb8281651c79088ee5a20f27e19`  
		Last Modified: Wed, 05 Oct 2022 18:45:25 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86240b0ade55ae53beb11330c6ca00b10fa1f26ecf9811f54503459eb97bf4a2`  
		Last Modified: Wed, 05 Oct 2022 18:45:24 GMT  
		Size: 475.3 KB (475348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cacef0dbceb7ef9527fa2a04838a23406b28fe204ba0b42f26f570c0d85a34a`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed253dc6a17b72e0b0a41d81c9f15e347107836549c9e33bcba90553b1629985`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99adf8cb9165fe94b1d5448901445e2c49b0980d1fb83c061f6d4ca8c3cf45e`  
		Last Modified: Wed, 05 Oct 2022 18:46:07 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bd4fe35530481c24f429204008ff1582957f98ce98344a2b67b15b28c1ab9c`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:c4dfd932a248cc4c5043cbc8e948ecd99dc3f0ee0a6d2586eccb15996adcb9ba
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
$ docker pull bonita@sha256:f70def9d67125c205708688b13d1c9de4e42528839dca3297ea30e719ddb3151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234123216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fe908e53db5f3ba2be7eef1c7066ce35e743f7736f647aa54499ea3ec4a89d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:42:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:42:14 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:42:15 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:42:19 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:42:19 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:42:46 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:42:47 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 05 Oct 2022 18:42:47 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 05 Oct 2022 18:42:48 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 18:42:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:42:48 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 05 Oct 2022 18:42:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 18:42:51 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:42:51 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 05 Oct 2022 18:43:07 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 05 Oct 2022 18:43:09 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 18:43:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 18:43:11 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:43:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:43:12 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:43:13 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65434190d8d0b310da61bd4a0c9803eafe3aaef0288085588b6f45b6d54e031`  
		Last Modified: Wed, 05 Oct 2022 18:45:45 GMT  
		Size: 86.8 MB (86779064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2732e23275ee1da8786e079deae810600f99c6fa09fc13b5ca4dd42ac67ff42`  
		Last Modified: Wed, 05 Oct 2022 18:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2790f9dce24ed4c863e7cfc3059c4fd0a843ddb8281651c79088ee5a20f27e19`  
		Last Modified: Wed, 05 Oct 2022 18:45:25 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86240b0ade55ae53beb11330c6ca00b10fa1f26ecf9811f54503459eb97bf4a2`  
		Last Modified: Wed, 05 Oct 2022 18:45:24 GMT  
		Size: 475.3 KB (475348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cacef0dbceb7ef9527fa2a04838a23406b28fe204ba0b42f26f570c0d85a34a`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed253dc6a17b72e0b0a41d81c9f15e347107836549c9e33bcba90553b1629985`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99adf8cb9165fe94b1d5448901445e2c49b0980d1fb83c061f6d4ca8c3cf45e`  
		Last Modified: Wed, 05 Oct 2022 18:46:07 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bd4fe35530481c24f429204008ff1582957f98ce98344a2b67b15b28c1ab9c`  
		Last Modified: Wed, 05 Oct 2022 18:45:58 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:0d49a65293fcd6ff14ddffb804c637be836cb3cba66a6fa09766773106b0d127
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
$ docker pull bonita@sha256:9cb8e349b2bf6d4d8a1d67a572691c9f0a4ec97b85d2a9692ab2e6405c6044f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231788382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36eeb3c8ad8d36ed7a9a74232c77a82c0c1538b08a812aefbdc03de075a3c784`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:44:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:44:04 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:44:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:44:09 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:44:09 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 18:44:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:44:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:14 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:44:14 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 18:44:26 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 18:44:28 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 18:44:30 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:44:30 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:44:32 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:44:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f9e39a6a7f63873a2dc20d23d5c8d1fc5fa58eae6190c7105001b2c8d9894c`  
		Last Modified: Wed, 05 Oct 2022 18:46:45 GMT  
		Size: 86.8 MB (86779112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ea1151120c9f1f0f613e0ed92eeed3084bf66c8c45ac449f780d480247a08b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db734224771944745348b76c383673051a02f2d64bb9c5b69f3c4e8520d7765b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea716d20ae0b2b5be4d4fe4548c9e198ee759216b8e1047d64e406db51473`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 831.6 KB (831575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d394e8f62f1973732d5656c2400bb2b98241d96edf0b1cd1c24be144ca21a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcb40ceb70f178b47382a06a174c6308324d85011f65472380a43e4693db4f`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ea30fddaf1a1df0a83bc3e29628cc996b0a811b7b7689ab9122c188ef8defb`  
		Last Modified: Wed, 05 Oct 2022 18:46:33 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ecf65c2498bc270470ae0c9abfdb8dea80371ecf7b301490f6ee08aa79060a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:0d49a65293fcd6ff14ddffb804c637be836cb3cba66a6fa09766773106b0d127
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
$ docker pull bonita@sha256:9cb8e349b2bf6d4d8a1d67a572691c9f0a4ec97b85d2a9692ab2e6405c6044f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231788382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36eeb3c8ad8d36ed7a9a74232c77a82c0c1538b08a812aefbdc03de075a3c784`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 05 Oct 2022 10:51:52 GMT
ADD file:d93b8e74342ae6048a42c90c30192dd384e92b697ad4d8d5944868e03325820c in / 
# Wed, 05 Oct 2022 10:51:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:40:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 05 Oct 2022 18:44:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:44:04 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 05 Oct 2022 18:44:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 05 Oct 2022 18:44:09 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 05 Oct 2022 18:44:09 GMT
ARG BONITA_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BRANDING_VERSION
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:44:10 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BONITA_VERSION=7.13.0
# Wed, 05 Oct 2022 18:44:11 GMT
ENV BRANDING_VERSION=2021.2-u0
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Wed, 05 Oct 2022 18:44:12 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:12 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:44:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Wed, 05 Oct 2022 18:44:14 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:44:14 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Wed, 05 Oct 2022 18:44:26 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Wed, 05 Oct 2022 18:44:28 GMT
ENV HTTP_API=false
# Wed, 05 Oct 2022 18:44:30 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:44:30 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:44:32 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:44:34 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:faece833463c99bd10748da29171f2d588a627912f7bbb982b3ca4512dd39eed`  
		Last Modified: Wed, 05 Oct 2022 10:54:03 GMT  
		Size: 30.4 MB (30442565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f9e39a6a7f63873a2dc20d23d5c8d1fc5fa58eae6190c7105001b2c8d9894c`  
		Last Modified: Wed, 05 Oct 2022 18:46:45 GMT  
		Size: 86.8 MB (86779112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ea1151120c9f1f0f613e0ed92eeed3084bf66c8c45ac449f780d480247a08b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db734224771944745348b76c383673051a02f2d64bb9c5b69f3c4e8520d7765b`  
		Last Modified: Wed, 05 Oct 2022 18:46:25 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aea716d20ae0b2b5be4d4fe4548c9e198ee759216b8e1047d64e406db51473`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 831.6 KB (831575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d394e8f62f1973732d5656c2400bb2b98241d96edf0b1cd1c24be144ca21a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcb40ceb70f178b47382a06a174c6308324d85011f65472380a43e4693db4f`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 3.3 KB (3306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ea30fddaf1a1df0a83bc3e29628cc996b0a811b7b7689ab9122c188ef8defb`  
		Last Modified: Wed, 05 Oct 2022 18:46:33 GMT  
		Size: 113.7 MB (113727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ecf65c2498bc270470ae0c9abfdb8dea80371ecf7b301490f6ee08aa79060a`  
		Last Modified: Wed, 05 Oct 2022 18:46:23 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14`

```console
$ docker pull bonita@sha256:f9e3cf341d6c539317a09231e40cb9ea7aa57b422d4d7a03ce4bb455226d240c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:67e41d4134c19e4a1966b0c0193542c4afc452996461d1c55d4c41e3617dc4b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fe400a159423f451be8962b98c0ad9a8b2864f91e161025fa32a0cfe37e25d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:52:48 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:52:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:52:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:52:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:52:55 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:52:56 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:52:57 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:52:58 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:52:59 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:53:00 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:53:01 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:53:02 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:53:03 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:53:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:06 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:53:08 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:53:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:53:16 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:53:17 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:53:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:53:19 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:53:20 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:53:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:53:22 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:53:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:53:24 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:53:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:53:26 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:53:27 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:53:28 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:53:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:53:30 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:53:31 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:53:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a72dcffd05869e5d752c06042ca884a4a8b1cc5e45920f2091bf0074f91a1`  
		Last Modified: Thu, 06 Oct 2022 19:54:26 GMT  
		Size: 60.1 MB (60129767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c53dea9976f27698da497a98de6604659903be074da8046acc0efd2336bcdc`  
		Last Modified: Thu, 06 Oct 2022 19:54:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd9113513200994b4f8363b9a3ff7d6d618fb2f1690272f476e6e42b8ba0dc2`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2dc70af30020f1fd49a24cec2bcce85130941d5c41c6dbcb5e33760e80b1e`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e37ee56ee4a54b64dc500b91def3e43575c3b4468aa1200e8ff420d00eaad`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 3.0 KB (3000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6172ff1fd0d733339e8a27557a5d788212a4f42b7491bdd830543603ab2bedf`  
		Last Modified: Thu, 06 Oct 2022 19:54:25 GMT  
		Size: 116.7 MB (116688760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2348246f4562d42618128248d56903c98195e7fb74f255d4296cc55b03a92c`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.14.0`

```console
$ docker pull bonita@sha256:f9e3cf341d6c539317a09231e40cb9ea7aa57b422d4d7a03ce4bb455226d240c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.14.0` - linux; amd64

```console
$ docker pull bonita@sha256:862fefb5c63bd62f0d955db355c2f3f4f22e193522753d8eedc527cd683c6d9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180333199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bff25d56fe4420a99127f674a2df8588fc8fdf9319915429e3416e6f76dc008`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:14:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 20:14:13 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 20:14:14 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 20:14:14 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 20:14:14 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 20:14:15 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 20:14:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 20:14:16 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 20:14:16 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 20:14:30 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 20:14:31 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 20:14:31 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 20:14:31 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 20:14:31 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 20:14:32 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 20:14:32 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 20:14:32 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 20:14:32 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 20:14:32 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 20:14:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ede2860654ad6d68046410f9ebec3dd9b9dca61c6fd599f0045a6f5741bf9d6`  
		Last Modified: Thu, 06 Oct 2022 20:15:08 GMT  
		Size: 60.8 MB (60808866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce69fcdc27b67a89739ff4629aa93b1c46f792c65d81f096c0f8a7d81a47728`  
		Last Modified: Thu, 06 Oct 2022 20:15:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af59dcbbf223b0ac4dc3fd0d01996906c078459ddaae9684440c4cea484b89c`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2805f0e33650a409f35745444bc7f23d5e82f697438025abb67df81ec03caf4`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173969905ee8acb031228953620f4d6f959d48886d22214974e9764c2d27e28a`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afce6ae14f1b5883093c182f12ce1d593988cae499bb4372256b0301c1b00e9e`  
		Last Modified: Thu, 06 Oct 2022 20:15:05 GMT  
		Size: 116.7 MB (116690804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98acc053b219affe2080f6ddfad206474004eda9666c5b092bf9fc90aa31659`  
		Last Modified: Thu, 06 Oct 2022 20:14:58 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:67e41d4134c19e4a1966b0c0193542c4afc452996461d1c55d4c41e3617dc4b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fe400a159423f451be8962b98c0ad9a8b2864f91e161025fa32a0cfe37e25d`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:52:48 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:52:52 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:52:53 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:52:54 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:52:55 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:52:56 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:52:57 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:52:58 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:52:59 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:53:00 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:53:01 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:53:02 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:53:03 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:04 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:53:05 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:53:06 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:53:08 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:53:16 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:53:16 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:53:17 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:53:18 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:53:19 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:53:20 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:53:21 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:53:22 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:53:23 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:53:24 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:53:25 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:53:26 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:53:27 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:53:28 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:53:30 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:53:30 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:53:31 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:53:32 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616a72dcffd05869e5d752c06042ca884a4a8b1cc5e45920f2091bf0074f91a1`  
		Last Modified: Thu, 06 Oct 2022 19:54:26 GMT  
		Size: 60.1 MB (60129767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c53dea9976f27698da497a98de6604659903be074da8046acc0efd2336bcdc`  
		Last Modified: Thu, 06 Oct 2022 19:54:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd9113513200994b4f8363b9a3ff7d6d618fb2f1690272f476e6e42b8ba0dc2`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a2dc70af30020f1fd49a24cec2bcce85130941d5c41c6dbcb5e33760e80b1e`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e37ee56ee4a54b64dc500b91def3e43575c3b4468aa1200e8ff420d00eaad`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 3.0 KB (3000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6172ff1fd0d733339e8a27557a5d788212a4f42b7491bdd830543603ab2bedf`  
		Last Modified: Thu, 06 Oct 2022 19:54:25 GMT  
		Size: 116.7 MB (116688760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2348246f4562d42618128248d56903c98195e7fb74f255d4296cc55b03a92c`  
		Last Modified: Thu, 06 Oct 2022 19:54:16 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.14.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:ed30ab3ec5061aff1dc71c87ce3b52a60cc3aacc160f8dcfd7692cf5f1c91383
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176142311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9e92713926d622cf557e08cf608df8445515cc2805d567604854576eabb7a1`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:56:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 06 Oct 2022 19:56:48 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre-headless
# Thu, 06 Oct 2022 19:56:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 06 Oct 2022 19:56:52 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BRANDING_VERSION
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BONITA_SHA256
# Thu, 06 Oct 2022 19:56:53 GMT
ARG BASE_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ARG BONITA_URL
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_VERSION=7.14.0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BRANDING_VERSION=2022.1-u0
# Thu, 06 Oct 2022 19:56:54 GMT
ENV BONITA_SHA256=a88b3f4368bd68dda4eccf4680a71b7e523678811b6b3bcd61cd85e67e9b9aeb
# Thu, 06 Oct 2022 19:56:55 GMT
ENV ZIP_FILE=BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 06 Oct 2022 19:56:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.1-u0/BonitaCommunity-2022.1-u0.zip
# Thu, 06 Oct 2022 19:56:56 GMT
RUN mkdir /opt/files
# Thu, 06 Oct 2022 19:56:57 GMT
COPY dir:55abb36f42ed7e3d3197415cf20ab2abe54eeefc3accbc7bc3be8dbd2d0f8d41 in /opt/files 
# Thu, 06 Oct 2022 19:57:09 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API=false
# Thu, 06 Oct 2022 19:57:11 GMT
ENV HTTP_API_USERNAME=http-api
# Thu, 06 Oct 2022 19:57:12 GMT
ENV HTTP_API_PASSWORD=
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_USERNAME=monitoring
# Thu, 06 Oct 2022 19:57:12 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Thu, 06 Oct 2022 19:57:13 GMT
ENV JMX_REMOTE_ACCESS=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Thu, 06 Oct 2022 19:57:13 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Thu, 06 Oct 2022 19:57:14 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Thu, 06 Oct 2022 19:57:15 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Thu, 06 Oct 2022 19:57:15 GMT
ENV HTTP_MAX_THREADS=20
# Thu, 06 Oct 2022 19:57:15 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Thu, 06 Oct 2022 19:57:15 GMT
EXPOSE 8080 9000
# Thu, 06 Oct 2022 19:57:16 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Thu, 06 Oct 2022 19:57:16 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef077ba375222dadf88017804c6db49ec3e6c7c7dda2b13cfe326acb96e5573`  
		Last Modified: Thu, 06 Oct 2022 19:58:18 GMT  
		Size: 56.6 MB (56628443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9b2a0c46e4583581aea4b26d7e4888620778734b640fde9a243c60896a85c`  
		Last Modified: Thu, 06 Oct 2022 19:58:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d02cbac52ba92d847db176427502c97ac8cfce0205b8df2e17984291749fb48`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5d063ca3ad4a351f1d87243e8704f415833c9636631b3c787fdabc5893e198`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ea1f55b182c3f8c835160384e887986ba36466e0bc71aa145f0065f4198f0`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dc7c2196ec38ed7be31a96dd4f6c81db83b6e9a8bc4efd5f2edd63c8b4fbc`  
		Last Modified: Thu, 06 Oct 2022 19:58:14 GMT  
		Size: 116.7 MB (116690860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00f2bd54e8ef56344883e905c4ee8e2f08246937858fd47004be957103b17bb`  
		Last Modified: Thu, 06 Oct 2022 19:58:03 GMT  
		Size: 5.4 KB (5423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15`

```console
$ docker pull bonita@sha256:9326157dd76ba4fafc97e8380d64228cd53dfe369465e872e6d616c7a257b927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15` - linux; amd64

```console
$ docker pull bonita@sha256:96beb319839334dd24cf8b6cc849e68533fad89cf5aca869e1cc4ebc039d0f65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183206256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09da6c720099e834ec57a16315d0defea6cc1a1518380a596ffd3a868a9fdb59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:19:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:19:39 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:19:39 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:19:40 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:42 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:19:50 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:19:50 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:19:51 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:19:52 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:19:52 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:19:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:19:52 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:19:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:19:52 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5705f95d901e9d31f362e998a2c059acf47627969b042b4e7aaa72b533530e0`  
		Last Modified: Fri, 07 Oct 2022 19:20:29 GMT  
		Size: 61.2 MB (61197146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76059907474246c43b72aae8948b443645cfd4ab27e255f2555ba7a1f133806f`  
		Last Modified: Fri, 07 Oct 2022 19:20:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022b3528f0c93c13aeb319e8037b590351d556f7513d476a1da5d77734de820a`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c21d4b689cde4c6b32704ec260ace9395c580c5fd4403ec9691e367c6f91c`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af35cb2d6152fd421952af9e5bce9d544b5dd30338842f1d40c610fa142e2592`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202ed4e518b9784b3e9b2db17c26afe1be89539f86cea9362694f65fc089d70`  
		Last Modified: Fri, 07 Oct 2022 19:20:26 GMT  
		Size: 119.2 MB (119193019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bf2b5af323e9cc69f227a7c46ffdb4dd88609ecedc45a1a807120aa39fe89`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:678134bdb94e4f63cf83093514b25b71dfe9b347c97625e9a786aadd96ef6138
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182348091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce03089f322a258cae18ca28497bd1fa0fb756aae2b79915561d63c521a728`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:39:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:39:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:39:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:39:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:39:50 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:39:51 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:39:52 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:39:53 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:39:54 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:39:55 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:39:56 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:39:57 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:39:58 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:39:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:40:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:40:01 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:40:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:40:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:40:11 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:40:12 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:40:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:40:14 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:40:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:40:16 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:40:17 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:40:18 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:40:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:40:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:40:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:40:22 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:40:23 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:40:25 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:40:25 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:40:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:40:27 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497bd0e996de2d902f26a3023b901109ea46ec8d01ca2f527040175722bd069`  
		Last Modified: Fri, 07 Oct 2022 19:41:24 GMT  
		Size: 60.4 MB (60439220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe10e617bb9fab6e845f6c0feb39e110610ab11115ba462991c612f7a410fb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7bd7e5925381829a64c85fde46c63063cde25fe1a409cede494629ebbddb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8354d92c69b70dd6748ac85796528746adb07c9665e0686c52eeca5926e56a71`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 111.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17a0dcd655da714128f4233e36d2c2686818f3b524642fc1a4bd4ac143f735e`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d141b4d5dcee5ce2546270c1002d4a83d7458f062a52b9b7b41a3f75fb6276f`  
		Last Modified: Fri, 07 Oct 2022 19:41:27 GMT  
		Size: 119.2 MB (119191347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce674d50db2ba300dc2c6d26d93908e4c56432fa7f6d8047cd64999bf1dfe939`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15` - linux; ppc64le

```console
$ docker pull bonita@sha256:2c3128dbea0d3d5d8a63712d1db500fdecbc8b9d2995a695c37b4ebb80b5ef48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179326996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3838b00163be847a672d409b30519320813b30bf0947292136a897403f4be7`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:16:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:16:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:16:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:16:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:16:49 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:16:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:53 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:16:54 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:17:12 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:17:13 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:17:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:17:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:17:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:17:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:17:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:17:17 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:17:17 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:17:17 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c61989a45cdf74208e16d4c9fef94cee3d8eb10602f7ac45e023fb053dbf4e7`  
		Last Modified: Fri, 07 Oct 2022 19:18:27 GMT  
		Size: 57.3 MB (57320650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3fc5ec26c7a10b790182e0bc521d1c16847666abf323733fe17fb228c1839`  
		Last Modified: Fri, 07 Oct 2022 19:18:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2817209af0ad99735a5596f59d738933e465b7ef11feeaa492e45b842fb1a4cc`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d550240e348d5a213ea1a0d93c6108eb6c1d9a1936d7579c893c4cf91024ba1`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7105d16280bde13de94b8d7829efa1a960a706fae2772e49d24c0b8c0bad2`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5f0b41531d404e2a3e56f2983347537cec2d7cc8d0266e17897e3ef247be3`  
		Last Modified: Fri, 07 Oct 2022 19:18:22 GMT  
		Size: 119.2 MB (119192998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7377eb804f8177040817c5380de0d04576a7b288322ff9c5a3ee7305720e5313`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.15.0`

```console
$ docker pull bonita@sha256:9326157dd76ba4fafc97e8380d64228cd53dfe369465e872e6d616c7a257b927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.15.0` - linux; amd64

```console
$ docker pull bonita@sha256:96beb319839334dd24cf8b6cc849e68533fad89cf5aca869e1cc4ebc039d0f65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183206256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09da6c720099e834ec57a16315d0defea6cc1a1518380a596ffd3a868a9fdb59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:19:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:19:39 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:19:39 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:19:40 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:42 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:19:50 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:19:50 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:19:51 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:19:52 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:19:52 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:19:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:19:52 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:19:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:19:52 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5705f95d901e9d31f362e998a2c059acf47627969b042b4e7aaa72b533530e0`  
		Last Modified: Fri, 07 Oct 2022 19:20:29 GMT  
		Size: 61.2 MB (61197146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76059907474246c43b72aae8948b443645cfd4ab27e255f2555ba7a1f133806f`  
		Last Modified: Fri, 07 Oct 2022 19:20:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022b3528f0c93c13aeb319e8037b590351d556f7513d476a1da5d77734de820a`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c21d4b689cde4c6b32704ec260ace9395c580c5fd4403ec9691e367c6f91c`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af35cb2d6152fd421952af9e5bce9d544b5dd30338842f1d40c610fa142e2592`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202ed4e518b9784b3e9b2db17c26afe1be89539f86cea9362694f65fc089d70`  
		Last Modified: Fri, 07 Oct 2022 19:20:26 GMT  
		Size: 119.2 MB (119193019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bf2b5af323e9cc69f227a7c46ffdb4dd88609ecedc45a1a807120aa39fe89`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:678134bdb94e4f63cf83093514b25b71dfe9b347c97625e9a786aadd96ef6138
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182348091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce03089f322a258cae18ca28497bd1fa0fb756aae2b79915561d63c521a728`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:39:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:39:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:39:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:39:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:39:50 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:39:51 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:39:52 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:39:53 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:39:54 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:39:55 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:39:56 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:39:57 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:39:58 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:39:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:40:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:40:01 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:40:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:40:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:40:11 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:40:12 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:40:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:40:14 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:40:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:40:16 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:40:17 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:40:18 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:40:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:40:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:40:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:40:22 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:40:23 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:40:25 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:40:25 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:40:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:40:27 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497bd0e996de2d902f26a3023b901109ea46ec8d01ca2f527040175722bd069`  
		Last Modified: Fri, 07 Oct 2022 19:41:24 GMT  
		Size: 60.4 MB (60439220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe10e617bb9fab6e845f6c0feb39e110610ab11115ba462991c612f7a410fb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7bd7e5925381829a64c85fde46c63063cde25fe1a409cede494629ebbddb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8354d92c69b70dd6748ac85796528746adb07c9665e0686c52eeca5926e56a71`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 111.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17a0dcd655da714128f4233e36d2c2686818f3b524642fc1a4bd4ac143f735e`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d141b4d5dcee5ce2546270c1002d4a83d7458f062a52b9b7b41a3f75fb6276f`  
		Last Modified: Fri, 07 Oct 2022 19:41:27 GMT  
		Size: 119.2 MB (119191347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce674d50db2ba300dc2c6d26d93908e4c56432fa7f6d8047cd64999bf1dfe939`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.15.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:2c3128dbea0d3d5d8a63712d1db500fdecbc8b9d2995a695c37b4ebb80b5ef48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179326996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3838b00163be847a672d409b30519320813b30bf0947292136a897403f4be7`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:16:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:16:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:16:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:16:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:16:49 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:16:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:53 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:16:54 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:17:12 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:17:13 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:17:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:17:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:17:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:17:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:17:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:17:17 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:17:17 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:17:17 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c61989a45cdf74208e16d4c9fef94cee3d8eb10602f7ac45e023fb053dbf4e7`  
		Last Modified: Fri, 07 Oct 2022 19:18:27 GMT  
		Size: 57.3 MB (57320650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3fc5ec26c7a10b790182e0bc521d1c16847666abf323733fe17fb228c1839`  
		Last Modified: Fri, 07 Oct 2022 19:18:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2817209af0ad99735a5596f59d738933e465b7ef11feeaa492e45b842fb1a4cc`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d550240e348d5a213ea1a0d93c6108eb6c1d9a1936d7579c893c4cf91024ba1`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7105d16280bde13de94b8d7829efa1a960a706fae2772e49d24c0b8c0bad2`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5f0b41531d404e2a3e56f2983347537cec2d7cc8d0266e17897e3ef247be3`  
		Last Modified: Fri, 07 Oct 2022 19:18:22 GMT  
		Size: 119.2 MB (119192998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7377eb804f8177040817c5380de0d04576a7b288322ff9c5a3ee7305720e5313`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:9326157dd76ba4fafc97e8380d64228cd53dfe369465e872e6d616c7a257b927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:96beb319839334dd24cf8b6cc849e68533fad89cf5aca869e1cc4ebc039d0f65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183206256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09da6c720099e834ec57a16315d0defea6cc1a1518380a596ffd3a868a9fdb59`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:19:35 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:19:39 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:19:39 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:19:40 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:19:40 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:19:41 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:19:41 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:19:42 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:19:42 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:19:50 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:19:50 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:19:51 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:19:51 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:19:51 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:19:51 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:19:52 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:19:52 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:19:52 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:19:52 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:19:52 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:19:52 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5705f95d901e9d31f362e998a2c059acf47627969b042b4e7aaa72b533530e0`  
		Last Modified: Fri, 07 Oct 2022 19:20:29 GMT  
		Size: 61.2 MB (61197146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76059907474246c43b72aae8948b443645cfd4ab27e255f2555ba7a1f133806f`  
		Last Modified: Fri, 07 Oct 2022 19:20:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022b3528f0c93c13aeb319e8037b590351d556f7513d476a1da5d77734de820a`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c21d4b689cde4c6b32704ec260ace9395c580c5fd4403ec9691e367c6f91c`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af35cb2d6152fd421952af9e5bce9d544b5dd30338842f1d40c610fa142e2592`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202ed4e518b9784b3e9b2db17c26afe1be89539f86cea9362694f65fc089d70`  
		Last Modified: Fri, 07 Oct 2022 19:20:26 GMT  
		Size: 119.2 MB (119193019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bf2b5af323e9cc69f227a7c46ffdb4dd88609ecedc45a1a807120aa39fe89`  
		Last Modified: Fri, 07 Oct 2022 19:20:18 GMT  
		Size: 5.4 KB (5422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:678134bdb94e4f63cf83093514b25b71dfe9b347c97625e9a786aadd96ef6138
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182348091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce03089f322a258cae18ca28497bd1fa0fb756aae2b79915561d63c521a728`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:39:43 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:39:47 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:39:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:39:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:39:50 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:39:51 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:39:52 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:39:53 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:39:54 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:39:55 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:39:56 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:39:57 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:39:58 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:39:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:40:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:40:01 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:40:03 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:40:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:40:11 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:40:12 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:40:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:40:14 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:40:15 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:40:16 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:40:17 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:40:18 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:40:19 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:40:20 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:40:21 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:40:22 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:40:23 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:40:25 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:40:25 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:40:26 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:40:27 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497bd0e996de2d902f26a3023b901109ea46ec8d01ca2f527040175722bd069`  
		Last Modified: Fri, 07 Oct 2022 19:41:24 GMT  
		Size: 60.4 MB (60439220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe10e617bb9fab6e845f6c0feb39e110610ab11115ba462991c612f7a410fb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7bd7e5925381829a64c85fde46c63063cde25fe1a409cede494629ebbddb4`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8354d92c69b70dd6748ac85796528746adb07c9665e0686c52eeca5926e56a71`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 111.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17a0dcd655da714128f4233e36d2c2686818f3b524642fc1a4bd4ac143f735e`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 3.0 KB (3011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d141b4d5dcee5ce2546270c1002d4a83d7458f062a52b9b7b41a3f75fb6276f`  
		Last Modified: Fri, 07 Oct 2022 19:41:27 GMT  
		Size: 119.2 MB (119191347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce674d50db2ba300dc2c6d26d93908e4c56432fa7f6d8047cd64999bf1dfe939`  
		Last Modified: Fri, 07 Oct 2022 19:41:13 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:2c3128dbea0d3d5d8a63712d1db500fdecbc8b9d2995a695c37b4ebb80b5ef48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179326996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3838b00163be847a672d409b30519320813b30bf0947292136a897403f4be7`
-	Entrypoint: `["\/opt\/files\/startup.sh"]`
-	Default Command: `["\/opt\/bonita\/server\/bin\/catalina.sh","run"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 19:16:36 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Oct 2022 19:16:45 GMT
RUN apk add --no-cache curl unzip bash su-exec jattach openjdk11-jre
# Fri, 07 Oct 2022 19:16:48 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Oct 2022 19:16:49 GMT
RUN addgroup -S -g 1000 bonita  && adduser -u 1000 -S  -G bonita -h /opt/bonita/ -s /sbin/nologin  bonita
# Fri, 07 Oct 2022 19:16:49 GMT
ARG BONITA_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BRANDING_VERSION
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_SHA256
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BASE_URL
# Fri, 07 Oct 2022 19:16:50 GMT
ARG BONITA_URL
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_VERSION=7.15.0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BRANDING_VERSION=2022.2-u0
# Fri, 07 Oct 2022 19:16:51 GMT
ENV BONITA_SHA256=9e6d35b3763ccc091b4b4dec1697c96231552847d4329420e796727c946e37a6
# Fri, 07 Oct 2022 19:16:52 GMT
ENV ZIP_FILE=BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Oct 2022 19:16:52 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2022.2-u0/BonitaCommunity-2022.2-u0.zip
# Fri, 07 Oct 2022 19:16:53 GMT
RUN mkdir /opt/files
# Fri, 07 Oct 2022 19:16:54 GMT
COPY dir:2f998cb77cda0ed47e4d103dacbc15e680f0e173a75b624320e21173de664a22 in /opt/files 
# Fri, 07 Oct 2022 19:17:11 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && echo "$BONITA_SHA256 */opt/files/$ZIP_FILE" | sha256sum -c - ; fi   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && mv /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/* /opt/bonita   && rmdir /opt/bonita/BonitaCommunity-${BRANDING_VERSION}   && unzip /opt/bonita/server/webapps/bonita.war -d /opt/bonita/server/webapps/bonita/   && rm /opt/bonita/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip   && mkdir -p /opt/bonita/conf/logs/   && mkdir -p /opt/bonita/logs/   && mv /opt/files/log4j2/log4j2-appenders.xml /opt/bonita/conf/logs/   && mv /opt/bonita/server/conf/log4j2-loggers.xml /opt/bonita/conf/logs/   && chown -R bonita:bonita /opt/bonita   && chmod go+w /opt/   && chmod -R +rX /opt   && chmod go+w /opt/bonita   && chmod 777 /opt/bonita/server/logs   && chmod 777 /opt/bonita/logs/   && chmod 777 /opt/bonita/server/temp   && chmod 777 /opt/bonita/server/work   && chmod -R go+w /opt/bonita/server/conf   && chmod -R go+w /opt/bonita/server/bin   && chmod -R go+w /opt/bonita/server/lib/bonita   && chmod -R go+w /opt/bonita/setup
# Fri, 07 Oct 2022 19:17:12 GMT
ENV HTTP_API=false
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_USERNAME=http-api
# Fri, 07 Oct 2022 19:17:13 GMT
ENV HTTP_API_PASSWORD=
# Fri, 07 Oct 2022 19:17:13 GMT
ENV MONITORING_USERNAME=monitoring
# Fri, 07 Oct 2022 19:17:14 GMT
ENV MONITORING_PASSWORD=mon1tor1ng_adm1n
# Fri, 07 Oct 2022 19:17:14 GMT
ENV JMX_REMOTE_ACCESS=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV REMOTE_IP_VALVE_ENABLED=false
# Fri, 07 Oct 2022 19:17:14 GMT
ENV ACCESSLOGS_STDOUT_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_FILES_ENABLED=false
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH=/opt/bonita/logs
# Fri, 07 Oct 2022 19:17:15 GMT
ENV ACCESSLOGS_PATH_APPEND_HOSTNAME=false
# Fri, 07 Oct 2022 19:17:16 GMT
ENV ACCESSLOGS_MAX_DAYS=30
# Fri, 07 Oct 2022 19:17:16 GMT
ENV HTTP_MAX_THREADS=20
# Fri, 07 Oct 2022 19:17:16 GMT
COPY dir:ad0fdf5900d3b914efcbba3170cc7d773b5d57072eba969a052457514aa27adc in /opt/templates 
# Fri, 07 Oct 2022 19:17:17 GMT
EXPOSE 8080 9000
# Fri, 07 Oct 2022 19:17:17 GMT
ENTRYPOINT ["/opt/files/startup.sh"]
# Fri, 07 Oct 2022 19:17:17 GMT
CMD ["/opt/bonita/server/bin/catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c61989a45cdf74208e16d4c9fef94cee3d8eb10602f7ac45e023fb053dbf4e7`  
		Last Modified: Fri, 07 Oct 2022 19:18:27 GMT  
		Size: 57.3 MB (57320650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd3fc5ec26c7a10b790182e0bc521d1c16847666abf323733fe17fb228c1839`  
		Last Modified: Fri, 07 Oct 2022 19:18:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2817209af0ad99735a5596f59d738933e465b7ef11feeaa492e45b842fb1a4cc`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d550240e348d5a213ea1a0d93c6108eb6c1d9a1936d7579c893c4cf91024ba1`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7105d16280bde13de94b8d7829efa1a960a706fae2772e49d24c0b8c0bad2`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 3.0 KB (3043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5f0b41531d404e2a3e56f2983347537cec2d7cc8d0266e17897e3ef247be3`  
		Last Modified: Fri, 07 Oct 2022 19:18:22 GMT  
		Size: 119.2 MB (119192998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7377eb804f8177040817c5380de0d04576a7b288322ff9c5a3ee7305720e5313`  
		Last Modified: Fri, 07 Oct 2022 19:18:11 GMT  
		Size: 5.4 KB (5419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
