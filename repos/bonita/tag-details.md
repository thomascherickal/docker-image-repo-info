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
$ docker pull bonita@sha256:001e7a4c4967ffb30a612c09d61c1a7decdc64c34d03ea128a05af5067126a6f
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
$ docker pull bonita@sha256:001e7a4c4967ffb30a612c09d61c1a7decdc64c34d03ea128a05af5067126a6f
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

## `bonita:7.11`

```console
$ docker pull bonita@sha256:8616e65aacbf8c30c1f3acd23303b72e5542a87f1cf4e18478f71f4ee350d64c
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
$ docker pull bonita@sha256:fc6b7271f03eab417027b4d991e796a373e7abfa77ce3b35f7154af41c5e661d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.1 MB (231055609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:272dd42b2975a102cf48edcb9cbc2af5b704bac11f2cd93fd865d8124c59b264`
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
# Wed, 05 Oct 2022 18:42:19 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:42:20 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:42:20 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:42:20 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 05 Oct 2022 18:42:21 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 05 Oct 2022 18:42:21 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 18:42:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:42:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 18:42:22 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 18:42:24 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:42:24 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 05 Oct 2022 18:42:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 05 Oct 2022 18:42:35 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 18:42:37 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 18:42:37 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:42:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:42:38 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:42:38 GMT
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
	-	`sha256:ea0b4345d6fe5ed7f203488a4f08626f27440360ce8e465c8c785583389d1ab6`  
		Last Modified: Wed, 05 Oct 2022 18:45:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c316cecc763f5c0929d75581bb2f06f6a44f89826808872481a6dff67d443f96`  
		Last Modified: Wed, 05 Oct 2022 18:45:23 GMT  
		Size: 6.9 KB (6898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3181897adb41d477fb929d6afcc3f5580752c0f13e7976a4a48a181efae3a233`  
		Last Modified: Wed, 05 Oct 2022 18:45:33 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63758a09f55176adc2f4c03c42033c3f10d334807e42de61713a5d381da0eda`  
		Last Modified: Wed, 05 Oct 2022 18:45:23 GMT  
		Size: 1.7 KB (1717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:8616e65aacbf8c30c1f3acd23303b72e5542a87f1cf4e18478f71f4ee350d64c
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
$ docker pull bonita@sha256:fc6b7271f03eab417027b4d991e796a373e7abfa77ce3b35f7154af41c5e661d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.1 MB (231055609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:272dd42b2975a102cf48edcb9cbc2af5b704bac11f2cd93fd865d8124c59b264`
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
# Wed, 05 Oct 2022 18:42:19 GMT
ARG BONITA_SHA256
# Wed, 05 Oct 2022 18:42:20 GMT
ARG BASE_URL
# Wed, 05 Oct 2022 18:42:20 GMT
ARG BONITA_URL
# Wed, 05 Oct 2022 18:42:20 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 05 Oct 2022 18:42:21 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 05 Oct 2022 18:42:21 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 18:42:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 05 Oct 2022 18:42:21 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 05 Oct 2022 18:42:22 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 05 Oct 2022 18:42:24 GMT
RUN mkdir /opt/files
# Wed, 05 Oct 2022 18:42:24 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 05 Oct 2022 18:42:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 05 Oct 2022 18:42:35 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 05 Oct 2022 18:42:37 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 05 Oct 2022 18:42:37 GMT
VOLUME [/opt/bonita]
# Wed, 05 Oct 2022 18:42:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 05 Oct 2022 18:42:38 GMT
EXPOSE 8080
# Wed, 05 Oct 2022 18:42:38 GMT
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
	-	`sha256:ea0b4345d6fe5ed7f203488a4f08626f27440360ce8e465c8c785583389d1ab6`  
		Last Modified: Wed, 05 Oct 2022 18:45:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c316cecc763f5c0929d75581bb2f06f6a44f89826808872481a6dff67d443f96`  
		Last Modified: Wed, 05 Oct 2022 18:45:23 GMT  
		Size: 6.9 KB (6898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3181897adb41d477fb929d6afcc3f5580752c0f13e7976a4a48a181efae3a233`  
		Last Modified: Wed, 05 Oct 2022 18:45:33 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63758a09f55176adc2f4c03c42033c3f10d334807e42de61713a5d381da0eda`  
		Last Modified: Wed, 05 Oct 2022 18:45:23 GMT  
		Size: 1.7 KB (1717 bytes)  
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
$ docker pull bonita@sha256:001e7a4c4967ffb30a612c09d61c1a7decdc64c34d03ea128a05af5067126a6f
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
$ docker pull bonita@sha256:001e7a4c4967ffb30a612c09d61c1a7decdc64c34d03ea128a05af5067126a6f
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

## `bonita:latest`

```console
$ docker pull bonita@sha256:001e7a4c4967ffb30a612c09d61c1a7decdc64c34d03ea128a05af5067126a6f
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

### `bonita:latest` - linux; ppc64le

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
