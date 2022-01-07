<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:2021.1`](#bonita20211)
-	[`bonita:2021.2`](#bonita20212)
-	[`bonita:2021.2-u0`](#bonita20212-u0)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.4`](#bonita7114)
-	[`bonita:7.12`](#bonita712)
-	[`bonita:7.12.1`](#bonita7121)
-	[`bonita:7.13`](#bonita713)
-	[`bonita:7.13.0`](#bonita7130)
-	[`bonita:latest`](#bonitalatest)

## `bonita:2021.1`

```console
$ docker pull bonita@sha256:7646be9fdfe8572764643e913578b77c29ef4194c8459ce76a6c3ce76180fb1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:ebc8ed86516521fb7edbd1c57902ce5a1beb1d4a285a03bd2a46553938dcfc34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237283638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e686edce26811e11a8d97473d4234ef8fb283555b0b4e202d773f0ad4bb51b0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:44:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:44:21 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:44:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:44:31 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:44:48 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 07 Jan 2022 02:44:48 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:44:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:44:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:44:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:44:51 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:44:51 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 07 Jan 2022 02:44:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:44:59 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:45:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:45:01 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:02 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7f3786c0c40f6e8deb47a2475ea53f4977287ebe714a44d44f950aaeec98ba`  
		Last Modified: Fri, 07 Jan 2022 02:46:34 GMT  
		Size: 93.6 MB (93575399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b661c522eadbab3f8f5ac630a7b61d0c75a436d97338298d029bad643809963a`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027782aea31321bb35d0f16a41c0b7207dcfbd88616de57459b062f409c5ecf3`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a02a08a1262d5108da96ace50d5ec3d318977c3a3c315a9da633d57653637d`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 577.0 KB (576963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb230869d25418bb417be80a7509bdafd7de12adab466a6c5b17dea712383139`  
		Last Modified: Fri, 07 Jan 2022 02:46:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6956864b7724141a69ce62391a3d8d74b4546843b335af20b52817e65d788d9`  
		Last Modified: Fri, 07 Jan 2022 02:46:46 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3ecf350694a1d2de08afd09a7311d0ecdefca39df5c7fc611b9e7c07f0913c`  
		Last Modified: Fri, 07 Jan 2022 02:46:55 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4e8317f722de18d2d67e8d6dad91fbe8f8e36f355d93af5c6521bfc79db8f`  
		Last Modified: Fri, 07 Jan 2022 02:46:45 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b47e16e82e4e8a2c94492e3a6d28f4e471f8ba9abc6b3380272f67ad088a0cb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226403449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8b9ffa0aa4b699cce26760edcb675c11f323cd2e592238acdb443b8614c30c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:12:24 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:12:25 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:12:36 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:12:37 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:13:10 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:13:11 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:13:12 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:13:13 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:13:14 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 07 Jan 2022 02:13:15 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 07 Jan 2022 02:13:16 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 07 Jan 2022 02:13:17 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:13:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:13:19 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:13:20 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:13:21 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:13:23 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 07 Jan 2022 02:13:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:13:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:13:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:13:32 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:13:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:13:34 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:13:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca822e6ba2fafa543991c7a6a40f34c01cc87fe3901534e562deb088176d7493`  
		Last Modified: Fri, 07 Jan 2022 02:15:44 GMT  
		Size: 85.7 MB (85703479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c51cef86fe6d8c848b23bf9356efd72d40eb9309423f30fb15cbc4c2742b45`  
		Last Modified: Fri, 07 Jan 2022 02:15:33 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d51d8356f23b73c45579abe97c2e7ae9fea11535c8a366b335e028731fdcc83`  
		Last Modified: Fri, 07 Jan 2022 02:15:32 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1503bacdf75977cb3264983f76442c8a2cce1ef3523605d38ea96570902981`  
		Last Modified: Fri, 07 Jan 2022 02:15:30 GMT  
		Size: 546.9 KB (546946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed14de4751c7e19603293038d3df64d993cb9d3d11f701dee5c99be24e969176`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2056d740f0a61d6cfbc612462f1f2bfc55803aabfa51d83a0c69e01e381430da`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 6.9 KB (6920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9ba6429c757c2825161ef4d1df346c4a723c950961988d2608a8fd4e35a7bc`  
		Last Modified: Fri, 07 Jan 2022 02:16:02 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995da71b9130454ebc7011f734b6911ae7ea272154ef258fc2d2baa7a3e0f360`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:ac1416c77bcac78a9298a94a94abbefde6a84f30d1c8c6ddb9d974813850e64d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233842751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f570d1f0ea23c7cb3e2af3d23faa36d28d1e857626b870b352bb5bed8d9921`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 06 Oct 2021 17:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:46:47 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 06 Oct 2021 17:46:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 06 Oct 2021 17:47:20 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 06 Oct 2021 17:47:24 GMT
ARG BONITA_VERSION
# Wed, 06 Oct 2021 17:49:45 GMT
ARG BRANDING_VERSION
# Wed, 06 Oct 2021 17:49:48 GMT
ARG BONITA_SHA256
# Wed, 06 Oct 2021 17:49:51 GMT
ARG BASE_URL
# Wed, 06 Oct 2021 17:49:55 GMT
ARG BONITA_URL
# Wed, 06 Oct 2021 17:50:00 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 06 Oct 2021 17:50:05 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 06 Oct 2021 17:50:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 06 Oct 2021 17:50:17 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 06 Oct 2021 17:50:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 06 Oct 2021 17:50:24 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 06 Oct 2021 17:50:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 06 Oct 2021 17:50:46 GMT
RUN mkdir /opt/files
# Wed, 06 Oct 2021 17:50:49 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 06 Oct 2021 17:51:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 06 Oct 2021 17:51:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 06 Oct 2021 17:52:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 06 Oct 2021 17:52:34 GMT
VOLUME [/opt/bonita]
# Wed, 06 Oct 2021 17:52:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 06 Oct 2021 17:52:43 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 17:52:52 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3edc21cfc352b7713634c746e33cbc4fa7e3ca0a6a30ff4b38e53392c9b32`  
		Last Modified: Wed, 06 Oct 2021 17:54:27 GMT  
		Size: 86.4 MB (86436862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018aca2fc40ed2d9ef571ad40cece30b4b96114ea033190abeebc6b26f1159a`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1a43207f8aeb2bffccebb563d56f146a642348a74c917fccedc5406ff7c048`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944db579c4969b5a1590926d71763dcdeff12d81aa7bc74411ea87c3999aa9c9`  
		Last Modified: Wed, 06 Oct 2021 17:54:11 GMT  
		Size: 546.7 KB (546726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bb1157a2d16356c3fe03471316decff49b6dc50796a886d2fb6537ec3c3b21`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3c397b4e693ea0a648aa5d5d11a1d68a1688c3894e594755a4c7b9ab141155`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd833d0ae3726dfae569704a9b090ee2eb0dc552d22117765785b6bfbc7a682f`  
		Last Modified: Wed, 06 Oct 2021 17:54:48 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c02458dc3f64372d814c185b974e07b342eec4c2dabd730f6e29a0f1e1b7d56`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2`

```console
$ docker pull bonita@sha256:9a3b4f11a5f355af70bf2f7fb4563972bce6ee11fe5152d72a11a9f5293ed3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2` - linux; amd64

```console
$ docker pull bonita@sha256:ed211d8966e81479a0de35d88067abc19128f5115f4ed0a18583d0109418c320
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235020325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f34dfd6f06c782fe12de949e94a95aec280a87fede53c2ecf93bdd31c1415`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:45:29 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:45:30 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:45:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:45:41 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:45:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:45:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:44 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:45:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:45:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:45:57 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:45:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:58 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97708e1be04f300190a6447eb5701bf6136bde08c7fc9d2f100554dee600862f`  
		Last Modified: Fri, 07 Jan 2022 02:47:23 GMT  
		Size: 93.6 MB (93576944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ccaf14419ce16922f1fadc9c0cfca941583821338487070f248663793e6a60`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee464fd0cad364188182240e3445e5ef7d60fcd8b054ea0f81f87bf26f2c1512`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30817fa401eb65a7fe63940c50cc18df1e57394daaec77595f0084faaa94d9b`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.0 MB (1003220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd02559b7c70dc211f68f796d7deef9233732d34de4041ea0e1b352b27736ef`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35076f161983cdfb4a547a85ce068f58dc441047b1ccc6cd3f1db1afbd64a40`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec320074cb8322b6f32e97f7fd43f3e74bceb2525a35c4d4003827d7891d876f`  
		Last Modified: Fri, 07 Jan 2022 02:47:15 GMT  
		Size: 113.7 MB (113727934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7f49324ac46378dd042d253b551c923c11f94b0f5328e3e242837544501e19`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e7dc23c1c127163649ca01a096ffa92d034bf77da4f1f174af5c8ddb4f83e870
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.1 MB (224094739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561be5fff3a0045b486baa9db80b475e8c51bacf50e62007dd73a619477d8922`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:14:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:14:24 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:14:25 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:14:26 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:14:27 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:14:28 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:14:29 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:14:30 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:14:31 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:14:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:14:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:14:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:36 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:14:38 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:14:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:14:46 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:14:47 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:14:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:14:50 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:14:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402cc759bf42029a19e7ddfcc42dc0db85ecb4bd43c89e8e3e1e0f7498cff516`  
		Last Modified: Fri, 07 Jan 2022 02:16:30 GMT  
		Size: 85.7 MB (85703427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da0cfcb5c10e4b2dc1bab617e8c29a34bb963f3e9ffa94e92c6c38f3bebeb04`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61837014e57970f4f06446a4c60d4f3cf530889c0fc449e3b4d758d8d4179c78`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2b8055c41250c722a929d047034ec9405cb0ee956a0be28f44d1e97a044f3a`  
		Last Modified: Fri, 07 Jan 2022 02:16:17 GMT  
		Size: 929.4 KB (929406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a9192b771b82b241d0bd13fa7ec48f7748732d4ea523071d6380c9054e1bb0`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8817c2a9b0f82e4e5e851a7431064c1dbfea617a62b83d8ff82852c72ece60`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f424b7e4fabf4819c12d14f9e2f95f08ca015a46b0be6e7cbc551ab9bd7eb5`  
		Last Modified: Fri, 07 Jan 2022 02:16:29 GMT  
		Size: 113.7 MB (113727903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a990cce3d3807e01700ddcaf1423e46f68f4b5444f90731f8c07548b71962`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2` - linux; ppc64le

```console
$ docker pull bonita@sha256:8f84286a16f847ace8b3ba19ce8ad3610d7cee0ee4fe2949cb336a18dd5a32e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e940107c65dc134dd59beb4e8fd39205865773d8dee6a0452f3d2436591ac92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 19:19:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 19:20:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 19:20:16 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 19:20:37 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 19:20:44 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 19:20:50 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 19:20:53 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 19:20:57 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 19:21:00 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 19:21:01 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 19:21:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 19:21:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 19:21:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 19:21:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:26 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 19:21:28 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 19:21:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 19:21:49 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 19:21:57 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 19:21:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 19:22:03 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 19:22:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d89d6ede66e22e682b17c5fb5b2665ee97d7f7d155861dda91815620662729`  
		Last Modified: Thu, 07 Oct 2021 19:23:14 GMT  
		Size: 86.4 MB (86437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fce009be160a4fe12d228556c91a26fda3281f23c16ec6136dea0a080ad37`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a62824290cee741a0aeb9676745be2c616eaa8dcd4ce7b949df063b35a1e16`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3250c10bd3ceef93513e091b435d9897e902f8ea3ea62f967eb4dc76a75b7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 904.2 KB (904197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e4b367f2ce3d9341f43a189bb7c26cbf78cc7c571661df9d2d1793e1ef2914`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6914c214de6daae2dd2e975b43ded87b3e54adb9560308f7769d1607bea7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e28e1cffdb6e7a72d3e63da9a49539242b8d4fa50dbecec5ff825c8942f0a6`  
		Last Modified: Thu, 07 Oct 2021 19:23:07 GMT  
		Size: 113.7 MB (113727917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc8bb2f32fefca639b2ccaffdf8d9cf883c5d510e0093ee31525ccbbf1df8d5`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:2021.2-u0`

```console
$ docker pull bonita@sha256:9a3b4f11a5f355af70bf2f7fb4563972bce6ee11fe5152d72a11a9f5293ed3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.2-u0` - linux; amd64

```console
$ docker pull bonita@sha256:ed211d8966e81479a0de35d88067abc19128f5115f4ed0a18583d0109418c320
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235020325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f34dfd6f06c782fe12de949e94a95aec280a87fede53c2ecf93bdd31c1415`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:45:29 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:45:30 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:45:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:45:41 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:45:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:45:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:44 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:45:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:45:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:45:57 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:45:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:58 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97708e1be04f300190a6447eb5701bf6136bde08c7fc9d2f100554dee600862f`  
		Last Modified: Fri, 07 Jan 2022 02:47:23 GMT  
		Size: 93.6 MB (93576944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ccaf14419ce16922f1fadc9c0cfca941583821338487070f248663793e6a60`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee464fd0cad364188182240e3445e5ef7d60fcd8b054ea0f81f87bf26f2c1512`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30817fa401eb65a7fe63940c50cc18df1e57394daaec77595f0084faaa94d9b`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.0 MB (1003220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd02559b7c70dc211f68f796d7deef9233732d34de4041ea0e1b352b27736ef`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35076f161983cdfb4a547a85ce068f58dc441047b1ccc6cd3f1db1afbd64a40`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec320074cb8322b6f32e97f7fd43f3e74bceb2525a35c4d4003827d7891d876f`  
		Last Modified: Fri, 07 Jan 2022 02:47:15 GMT  
		Size: 113.7 MB (113727934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7f49324ac46378dd042d253b551c923c11f94b0f5328e3e242837544501e19`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e7dc23c1c127163649ca01a096ffa92d034bf77da4f1f174af5c8ddb4f83e870
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.1 MB (224094739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561be5fff3a0045b486baa9db80b475e8c51bacf50e62007dd73a619477d8922`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:14:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:14:24 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:14:25 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:14:26 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:14:27 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:14:28 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:14:29 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:14:30 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:14:31 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:14:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:14:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:14:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:36 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:14:38 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:14:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:14:46 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:14:47 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:14:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:14:50 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:14:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402cc759bf42029a19e7ddfcc42dc0db85ecb4bd43c89e8e3e1e0f7498cff516`  
		Last Modified: Fri, 07 Jan 2022 02:16:30 GMT  
		Size: 85.7 MB (85703427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da0cfcb5c10e4b2dc1bab617e8c29a34bb963f3e9ffa94e92c6c38f3bebeb04`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61837014e57970f4f06446a4c60d4f3cf530889c0fc449e3b4d758d8d4179c78`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2b8055c41250c722a929d047034ec9405cb0ee956a0be28f44d1e97a044f3a`  
		Last Modified: Fri, 07 Jan 2022 02:16:17 GMT  
		Size: 929.4 KB (929406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a9192b771b82b241d0bd13fa7ec48f7748732d4ea523071d6380c9054e1bb0`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8817c2a9b0f82e4e5e851a7431064c1dbfea617a62b83d8ff82852c72ece60`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f424b7e4fabf4819c12d14f9e2f95f08ca015a46b0be6e7cbc551ab9bd7eb5`  
		Last Modified: Fri, 07 Jan 2022 02:16:29 GMT  
		Size: 113.7 MB (113727903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a990cce3d3807e01700ddcaf1423e46f68f4b5444f90731f8c07548b71962`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.2-u0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8f84286a16f847ace8b3ba19ce8ad3610d7cee0ee4fe2949cb336a18dd5a32e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e940107c65dc134dd59beb4e8fd39205865773d8dee6a0452f3d2436591ac92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 19:19:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 19:20:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 19:20:16 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 19:20:37 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 19:20:44 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 19:20:50 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 19:20:53 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 19:20:57 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 19:21:00 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 19:21:01 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 19:21:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 19:21:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 19:21:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 19:21:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:26 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 19:21:28 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 19:21:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 19:21:49 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 19:21:57 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 19:21:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 19:22:03 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 19:22:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d89d6ede66e22e682b17c5fb5b2665ee97d7f7d155861dda91815620662729`  
		Last Modified: Thu, 07 Oct 2021 19:23:14 GMT  
		Size: 86.4 MB (86437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fce009be160a4fe12d228556c91a26fda3281f23c16ec6136dea0a080ad37`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a62824290cee741a0aeb9676745be2c616eaa8dcd4ce7b949df063b35a1e16`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3250c10bd3ceef93513e091b435d9897e902f8ea3ea62f967eb4dc76a75b7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 904.2 KB (904197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e4b367f2ce3d9341f43a189bb7c26cbf78cc7c571661df9d2d1793e1ef2914`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6914c214de6daae2dd2e975b43ded87b3e54adb9560308f7769d1607bea7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e28e1cffdb6e7a72d3e63da9a49539242b8d4fa50dbecec5ff825c8942f0a6`  
		Last Modified: Thu, 07 Oct 2021 19:23:07 GMT  
		Size: 113.7 MB (113727917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc8bb2f32fefca639b2ccaffdf8d9cf883c5d510e0093ee31525ccbbf1df8d5`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:68f18ff88ab2d3a03e46628eabc415baf0a78d8a54aeb06463efed49498f3da6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:98e0e3e7aa16d4dfc285a125c8496cb46655940ee2a9328da767fdcba05a188b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234216005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84b704b9e129bdc8b4934ffdd0cee3b5a26d462fe758e6f1c6a00e8a91e7210`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:44:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:44:21 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:44:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:44:31 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:44:32 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:44:32 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 07 Jan 2022 02:44:32 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 07 Jan 2022 02:44:32 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:44:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:44:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:44:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:44:34 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:44:35 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 07 Jan 2022 02:44:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:44:41 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:44:43 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:44:43 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:44:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:44:43 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:44:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7f3786c0c40f6e8deb47a2475ea53f4977287ebe714a44d44f950aaeec98ba`  
		Last Modified: Fri, 07 Jan 2022 02:46:34 GMT  
		Size: 93.6 MB (93575399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b661c522eadbab3f8f5ac630a7b61d0c75a436d97338298d029bad643809963a`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027782aea31321bb35d0f16a41c0b7207dcfbd88616de57459b062f409c5ecf3`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a02a08a1262d5108da96ace50d5ec3d318977c3a3c315a9da633d57653637d`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 577.0 KB (576963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12007faa78bb7892635b508938bce7aeb43d7c80c07af46c8be65ad114012518`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93641292ec66a3d8043cd840dc7ada2d25a982650a41c7062bbd91a77ed94c2d`  
		Last Modified: Fri, 07 Jan 2022 02:46:18 GMT  
		Size: 6.9 KB (6889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223b515b5a52b97c3ddef3e70d87d99c98d399283b3d24fa44d93b18c94b2f81`  
		Last Modified: Fri, 07 Jan 2022 02:46:25 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb5d13f1a335b24f04ea63997e7ddc1d22f9e2e05a8a52271b5f91a32ce5370`  
		Last Modified: Fri, 07 Jan 2022 02:46:18 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d3ee3eb5641255a86ca14018afa77ff5902d1fcefd82f0f26dd74956dbd15265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223335813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dde139c075cb4260d81c7306b783777bbbef6397631e231b6efca7ab6f8bfcf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:12:24 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:12:25 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:12:36 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:12:37 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:12:38 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:12:39 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:12:40 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:12:41 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 07 Jan 2022 02:12:42 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 07 Jan 2022 02:12:43 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:12:44 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:12:45 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:12:46 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:12:47 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:12:49 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 07 Jan 2022 02:12:54 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:12:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:12:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:12:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:12:59 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:12:59 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:13:00 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca822e6ba2fafa543991c7a6a40f34c01cc87fe3901534e562deb088176d7493`  
		Last Modified: Fri, 07 Jan 2022 02:15:44 GMT  
		Size: 85.7 MB (85703479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c51cef86fe6d8c848b23bf9356efd72d40eb9309423f30fb15cbc4c2742b45`  
		Last Modified: Fri, 07 Jan 2022 02:15:33 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d51d8356f23b73c45579abe97c2e7ae9fea11535c8a366b335e028731fdcc83`  
		Last Modified: Fri, 07 Jan 2022 02:15:32 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1503bacdf75977cb3264983f76442c8a2cce1ef3523605d38ea96570902981`  
		Last Modified: Fri, 07 Jan 2022 02:15:30 GMT  
		Size: 546.9 KB (546946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4621397c0386db7be7d982a11223465cd931b9b00e319d060e58eabe52a8cc19`  
		Last Modified: Fri, 07 Jan 2022 02:15:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ca03608759134b55f8473ca1c9d04ec285ccd4b7c3ddc75b065c5320e40a62`  
		Last Modified: Fri, 07 Jan 2022 02:15:29 GMT  
		Size: 6.9 KB (6866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdd5c5c44aed2cf2ae10040ac9ed80019474236306bf8b0018724a929914454`  
		Last Modified: Fri, 07 Jan 2022 02:15:38 GMT  
		Size: 113.3 MB (113347829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afb5cab595b9cc0699ca6085f8b01a292d60fbeb28bcb1c19d8389d7814bbf1`  
		Last Modified: Fri, 07 Jan 2022 02:15:29 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:0701d5a2fdcc829fbb7bacbaa8f3de5b70a145abcac8762591fc6089858084de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230775119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:018671c72fe4f5563be295013fda4aa9aeaf106c25a0fbabff379053949e078b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 06 Oct 2021 17:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:46:47 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 06 Oct 2021 17:46:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 06 Oct 2021 17:47:20 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 06 Oct 2021 17:47:24 GMT
ARG BONITA_VERSION
# Wed, 06 Oct 2021 17:47:28 GMT
ARG BONITA_SHA256
# Wed, 06 Oct 2021 17:47:31 GMT
ARG BASE_URL
# Wed, 06 Oct 2021 17:47:34 GMT
ARG BONITA_URL
# Wed, 06 Oct 2021 17:47:39 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 06 Oct 2021 17:47:48 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 06 Oct 2021 17:47:54 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 06 Oct 2021 17:47:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 06 Oct 2021 17:48:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 06 Oct 2021 17:48:14 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 06 Oct 2021 17:48:25 GMT
RUN mkdir /opt/files
# Wed, 06 Oct 2021 17:48:26 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 06 Oct 2021 17:48:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 06 Oct 2021 17:48:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 06 Oct 2021 17:49:10 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 06 Oct 2021 17:49:12 GMT
VOLUME [/opt/bonita]
# Wed, 06 Oct 2021 17:49:14 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 06 Oct 2021 17:49:16 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 17:49:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3edc21cfc352b7713634c746e33cbc4fa7e3ca0a6a30ff4b38e53392c9b32`  
		Last Modified: Wed, 06 Oct 2021 17:54:27 GMT  
		Size: 86.4 MB (86436862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018aca2fc40ed2d9ef571ad40cece30b4b96114ea033190abeebc6b26f1159a`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1a43207f8aeb2bffccebb563d56f146a642348a74c917fccedc5406ff7c048`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944db579c4969b5a1590926d71763dcdeff12d81aa7bc74411ea87c3999aa9c9`  
		Last Modified: Wed, 06 Oct 2021 17:54:11 GMT  
		Size: 546.7 KB (546726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836bafca5e14e9559f37720debdea93a01c8863316d746f560dc6c76de13114d`  
		Last Modified: Wed, 06 Oct 2021 17:54:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233a6a775023061666f06611263f38e2cc5956ccb007cea963d74e04e2a23b03`  
		Last Modified: Wed, 06 Oct 2021 17:54:10 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5515c62070531ed4fcaa8a2d06626755081cd163ed0fec62bb15edfcb9c1f804`  
		Last Modified: Wed, 06 Oct 2021 17:54:18 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d6c54f1c4218e5b76e7882f84c3f0595947848a2b0a1b84d6ae8fb3349275d`  
		Last Modified: Wed, 06 Oct 2021 17:54:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:68f18ff88ab2d3a03e46628eabc415baf0a78d8a54aeb06463efed49498f3da6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:98e0e3e7aa16d4dfc285a125c8496cb46655940ee2a9328da767fdcba05a188b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234216005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84b704b9e129bdc8b4934ffdd0cee3b5a26d462fe758e6f1c6a00e8a91e7210`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:44:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:44:21 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:44:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:44:31 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:44:32 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:44:32 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 07 Jan 2022 02:44:32 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 07 Jan 2022 02:44:32 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:44:32 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:44:33 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:44:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:44:34 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:44:35 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 07 Jan 2022 02:44:40 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:44:41 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:44:43 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:44:43 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:44:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:44:43 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:44:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7f3786c0c40f6e8deb47a2475ea53f4977287ebe714a44d44f950aaeec98ba`  
		Last Modified: Fri, 07 Jan 2022 02:46:34 GMT  
		Size: 93.6 MB (93575399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b661c522eadbab3f8f5ac630a7b61d0c75a436d97338298d029bad643809963a`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027782aea31321bb35d0f16a41c0b7207dcfbd88616de57459b062f409c5ecf3`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a02a08a1262d5108da96ace50d5ec3d318977c3a3c315a9da633d57653637d`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 577.0 KB (576963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12007faa78bb7892635b508938bce7aeb43d7c80c07af46c8be65ad114012518`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93641292ec66a3d8043cd840dc7ada2d25a982650a41c7062bbd91a77ed94c2d`  
		Last Modified: Fri, 07 Jan 2022 02:46:18 GMT  
		Size: 6.9 KB (6889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223b515b5a52b97c3ddef3e70d87d99c98d399283b3d24fa44d93b18c94b2f81`  
		Last Modified: Fri, 07 Jan 2022 02:46:25 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb5d13f1a335b24f04ea63997e7ddc1d22f9e2e05a8a52271b5f91a32ce5370`  
		Last Modified: Fri, 07 Jan 2022 02:46:18 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d3ee3eb5641255a86ca14018afa77ff5902d1fcefd82f0f26dd74956dbd15265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.3 MB (223335813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dde139c075cb4260d81c7306b783777bbbef6397631e231b6efca7ab6f8bfcf`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:12:24 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:12:25 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:12:36 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:12:37 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:12:38 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:12:39 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:12:40 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:12:41 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 07 Jan 2022 02:12:42 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 07 Jan 2022 02:12:43 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:12:44 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:12:45 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 07 Jan 2022 02:12:46 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:12:47 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:12:49 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 07 Jan 2022 02:12:54 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:12:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:12:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:12:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:12:59 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:12:59 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:13:00 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca822e6ba2fafa543991c7a6a40f34c01cc87fe3901534e562deb088176d7493`  
		Last Modified: Fri, 07 Jan 2022 02:15:44 GMT  
		Size: 85.7 MB (85703479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c51cef86fe6d8c848b23bf9356efd72d40eb9309423f30fb15cbc4c2742b45`  
		Last Modified: Fri, 07 Jan 2022 02:15:33 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d51d8356f23b73c45579abe97c2e7ae9fea11535c8a366b335e028731fdcc83`  
		Last Modified: Fri, 07 Jan 2022 02:15:32 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1503bacdf75977cb3264983f76442c8a2cce1ef3523605d38ea96570902981`  
		Last Modified: Fri, 07 Jan 2022 02:15:30 GMT  
		Size: 546.9 KB (546946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4621397c0386db7be7d982a11223465cd931b9b00e319d060e58eabe52a8cc19`  
		Last Modified: Fri, 07 Jan 2022 02:15:29 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ca03608759134b55f8473ca1c9d04ec285ccd4b7c3ddc75b065c5320e40a62`  
		Last Modified: Fri, 07 Jan 2022 02:15:29 GMT  
		Size: 6.9 KB (6866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdd5c5c44aed2cf2ae10040ac9ed80019474236306bf8b0018724a929914454`  
		Last Modified: Fri, 07 Jan 2022 02:15:38 GMT  
		Size: 113.3 MB (113347829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afb5cab595b9cc0699ca6085f8b01a292d60fbeb28bcb1c19d8389d7814bbf1`  
		Last Modified: Fri, 07 Jan 2022 02:15:29 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:0701d5a2fdcc829fbb7bacbaa8f3de5b70a145abcac8762591fc6089858084de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230775119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:018671c72fe4f5563be295013fda4aa9aeaf106c25a0fbabff379053949e078b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 06 Oct 2021 17:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:46:47 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 06 Oct 2021 17:46:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 06 Oct 2021 17:47:20 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 06 Oct 2021 17:47:24 GMT
ARG BONITA_VERSION
# Wed, 06 Oct 2021 17:47:28 GMT
ARG BONITA_SHA256
# Wed, 06 Oct 2021 17:47:31 GMT
ARG BASE_URL
# Wed, 06 Oct 2021 17:47:34 GMT
ARG BONITA_URL
# Wed, 06 Oct 2021 17:47:39 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 06 Oct 2021 17:47:48 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 06 Oct 2021 17:47:54 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 06 Oct 2021 17:47:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 06 Oct 2021 17:48:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 06 Oct 2021 17:48:14 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 06 Oct 2021 17:48:25 GMT
RUN mkdir /opt/files
# Wed, 06 Oct 2021 17:48:26 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 06 Oct 2021 17:48:37 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 06 Oct 2021 17:48:57 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 06 Oct 2021 17:49:10 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 06 Oct 2021 17:49:12 GMT
VOLUME [/opt/bonita]
# Wed, 06 Oct 2021 17:49:14 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 06 Oct 2021 17:49:16 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 17:49:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3edc21cfc352b7713634c746e33cbc4fa7e3ca0a6a30ff4b38e53392c9b32`  
		Last Modified: Wed, 06 Oct 2021 17:54:27 GMT  
		Size: 86.4 MB (86436862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018aca2fc40ed2d9ef571ad40cece30b4b96114ea033190abeebc6b26f1159a`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1a43207f8aeb2bffccebb563d56f146a642348a74c917fccedc5406ff7c048`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944db579c4969b5a1590926d71763dcdeff12d81aa7bc74411ea87c3999aa9c9`  
		Last Modified: Wed, 06 Oct 2021 17:54:11 GMT  
		Size: 546.7 KB (546726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836bafca5e14e9559f37720debdea93a01c8863316d746f560dc6c76de13114d`  
		Last Modified: Wed, 06 Oct 2021 17:54:10 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233a6a775023061666f06611263f38e2cc5956ccb007cea963d74e04e2a23b03`  
		Last Modified: Wed, 06 Oct 2021 17:54:10 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5515c62070531ed4fcaa8a2d06626755081cd163ed0fec62bb15edfcb9c1f804`  
		Last Modified: Wed, 06 Oct 2021 17:54:18 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d6c54f1c4218e5b76e7882f84c3f0595947848a2b0a1b84d6ae8fb3349275d`  
		Last Modified: Wed, 06 Oct 2021 17:54:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:7646be9fdfe8572764643e913578b77c29ef4194c8459ce76a6c3ce76180fb1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:ebc8ed86516521fb7edbd1c57902ce5a1beb1d4a285a03bd2a46553938dcfc34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237283638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e686edce26811e11a8d97473d4234ef8fb283555b0b4e202d773f0ad4bb51b0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:44:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:44:21 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:44:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:44:31 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:44:48 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 07 Jan 2022 02:44:48 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:44:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:44:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:44:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:44:51 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:44:51 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 07 Jan 2022 02:44:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:44:59 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:45:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:45:01 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:02 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7f3786c0c40f6e8deb47a2475ea53f4977287ebe714a44d44f950aaeec98ba`  
		Last Modified: Fri, 07 Jan 2022 02:46:34 GMT  
		Size: 93.6 MB (93575399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b661c522eadbab3f8f5ac630a7b61d0c75a436d97338298d029bad643809963a`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027782aea31321bb35d0f16a41c0b7207dcfbd88616de57459b062f409c5ecf3`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a02a08a1262d5108da96ace50d5ec3d318977c3a3c315a9da633d57653637d`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 577.0 KB (576963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb230869d25418bb417be80a7509bdafd7de12adab466a6c5b17dea712383139`  
		Last Modified: Fri, 07 Jan 2022 02:46:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6956864b7724141a69ce62391a3d8d74b4546843b335af20b52817e65d788d9`  
		Last Modified: Fri, 07 Jan 2022 02:46:46 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3ecf350694a1d2de08afd09a7311d0ecdefca39df5c7fc611b9e7c07f0913c`  
		Last Modified: Fri, 07 Jan 2022 02:46:55 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4e8317f722de18d2d67e8d6dad91fbe8f8e36f355d93af5c6521bfc79db8f`  
		Last Modified: Fri, 07 Jan 2022 02:46:45 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b47e16e82e4e8a2c94492e3a6d28f4e471f8ba9abc6b3380272f67ad088a0cb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226403449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8b9ffa0aa4b699cce26760edcb675c11f323cd2e592238acdb443b8614c30c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:12:24 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:12:25 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:12:36 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:12:37 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:13:10 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:13:11 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:13:12 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:13:13 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:13:14 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 07 Jan 2022 02:13:15 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 07 Jan 2022 02:13:16 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 07 Jan 2022 02:13:17 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:13:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:13:19 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:13:20 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:13:21 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:13:23 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 07 Jan 2022 02:13:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:13:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:13:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:13:32 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:13:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:13:34 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:13:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca822e6ba2fafa543991c7a6a40f34c01cc87fe3901534e562deb088176d7493`  
		Last Modified: Fri, 07 Jan 2022 02:15:44 GMT  
		Size: 85.7 MB (85703479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c51cef86fe6d8c848b23bf9356efd72d40eb9309423f30fb15cbc4c2742b45`  
		Last Modified: Fri, 07 Jan 2022 02:15:33 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d51d8356f23b73c45579abe97c2e7ae9fea11535c8a366b335e028731fdcc83`  
		Last Modified: Fri, 07 Jan 2022 02:15:32 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1503bacdf75977cb3264983f76442c8a2cce1ef3523605d38ea96570902981`  
		Last Modified: Fri, 07 Jan 2022 02:15:30 GMT  
		Size: 546.9 KB (546946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed14de4751c7e19603293038d3df64d993cb9d3d11f701dee5c99be24e969176`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2056d740f0a61d6cfbc612462f1f2bfc55803aabfa51d83a0c69e01e381430da`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 6.9 KB (6920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9ba6429c757c2825161ef4d1df346c4a723c950961988d2608a8fd4e35a7bc`  
		Last Modified: Fri, 07 Jan 2022 02:16:02 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995da71b9130454ebc7011f734b6911ae7ea272154ef258fc2d2baa7a3e0f360`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:ac1416c77bcac78a9298a94a94abbefde6a84f30d1c8c6ddb9d974813850e64d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233842751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f570d1f0ea23c7cb3e2af3d23faa36d28d1e857626b870b352bb5bed8d9921`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 06 Oct 2021 17:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:46:47 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 06 Oct 2021 17:46:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 06 Oct 2021 17:47:20 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 06 Oct 2021 17:47:24 GMT
ARG BONITA_VERSION
# Wed, 06 Oct 2021 17:49:45 GMT
ARG BRANDING_VERSION
# Wed, 06 Oct 2021 17:49:48 GMT
ARG BONITA_SHA256
# Wed, 06 Oct 2021 17:49:51 GMT
ARG BASE_URL
# Wed, 06 Oct 2021 17:49:55 GMT
ARG BONITA_URL
# Wed, 06 Oct 2021 17:50:00 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 06 Oct 2021 17:50:05 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 06 Oct 2021 17:50:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 06 Oct 2021 17:50:17 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 06 Oct 2021 17:50:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 06 Oct 2021 17:50:24 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 06 Oct 2021 17:50:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 06 Oct 2021 17:50:46 GMT
RUN mkdir /opt/files
# Wed, 06 Oct 2021 17:50:49 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 06 Oct 2021 17:51:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 06 Oct 2021 17:51:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 06 Oct 2021 17:52:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 06 Oct 2021 17:52:34 GMT
VOLUME [/opt/bonita]
# Wed, 06 Oct 2021 17:52:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 06 Oct 2021 17:52:43 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 17:52:52 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3edc21cfc352b7713634c746e33cbc4fa7e3ca0a6a30ff4b38e53392c9b32`  
		Last Modified: Wed, 06 Oct 2021 17:54:27 GMT  
		Size: 86.4 MB (86436862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018aca2fc40ed2d9ef571ad40cece30b4b96114ea033190abeebc6b26f1159a`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1a43207f8aeb2bffccebb563d56f146a642348a74c917fccedc5406ff7c048`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944db579c4969b5a1590926d71763dcdeff12d81aa7bc74411ea87c3999aa9c9`  
		Last Modified: Wed, 06 Oct 2021 17:54:11 GMT  
		Size: 546.7 KB (546726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bb1157a2d16356c3fe03471316decff49b6dc50796a886d2fb6537ec3c3b21`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3c397b4e693ea0a648aa5d5d11a1d68a1688c3894e594755a4c7b9ab141155`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd833d0ae3726dfae569704a9b090ee2eb0dc552d22117765785b6bfbc7a682f`  
		Last Modified: Wed, 06 Oct 2021 17:54:48 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c02458dc3f64372d814c185b974e07b342eec4c2dabd730f6e29a0f1e1b7d56`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:7646be9fdfe8572764643e913578b77c29ef4194c8459ce76a6c3ce76180fb1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:ebc8ed86516521fb7edbd1c57902ce5a1beb1d4a285a03bd2a46553938dcfc34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237283638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e686edce26811e11a8d97473d4234ef8fb283555b0b4e202d773f0ad4bb51b0`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:44:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:44:21 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:44:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:44:31 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:44:31 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:44:47 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:44:48 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 07 Jan 2022 02:44:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 07 Jan 2022 02:44:48 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:44:49 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:44:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:44:50 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:44:51 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:44:51 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 07 Jan 2022 02:44:58 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:44:59 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:45:01 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:45:01 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:01 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:02 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:02 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7f3786c0c40f6e8deb47a2475ea53f4977287ebe714a44d44f950aaeec98ba`  
		Last Modified: Fri, 07 Jan 2022 02:46:34 GMT  
		Size: 93.6 MB (93575399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b661c522eadbab3f8f5ac630a7b61d0c75a436d97338298d029bad643809963a`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027782aea31321bb35d0f16a41c0b7207dcfbd88616de57459b062f409c5ecf3`  
		Last Modified: Fri, 07 Jan 2022 02:46:21 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a02a08a1262d5108da96ace50d5ec3d318977c3a3c315a9da633d57653637d`  
		Last Modified: Fri, 07 Jan 2022 02:46:19 GMT  
		Size: 577.0 KB (576963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb230869d25418bb417be80a7509bdafd7de12adab466a6c5b17dea712383139`  
		Last Modified: Fri, 07 Jan 2022 02:46:45 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6956864b7724141a69ce62391a3d8d74b4546843b335af20b52817e65d788d9`  
		Last Modified: Fri, 07 Jan 2022 02:46:46 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3ecf350694a1d2de08afd09a7311d0ecdefca39df5c7fc611b9e7c07f0913c`  
		Last Modified: Fri, 07 Jan 2022 02:46:55 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4e8317f722de18d2d67e8d6dad91fbe8f8e36f355d93af5c6521bfc79db8f`  
		Last Modified: Fri, 07 Jan 2022 02:46:45 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:b47e16e82e4e8a2c94492e3a6d28f4e471f8ba9abc6b3380272f67ad088a0cb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226403449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8b9ffa0aa4b699cce26760edcb675c11f323cd2e592238acdb443b8614c30c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:12:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:12:24 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:12:25 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:12:36 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:12:37 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:13:10 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:13:11 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:13:12 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:13:13 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:13:14 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 07 Jan 2022 02:13:15 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 07 Jan 2022 02:13:16 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 07 Jan 2022 02:13:17 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:13:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:13:19 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 07 Jan 2022 02:13:20 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 07 Jan 2022 02:13:21 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:13:23 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 07 Jan 2022 02:13:29 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 07 Jan 2022 02:13:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 07 Jan 2022 02:13:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 07 Jan 2022 02:13:32 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:13:34 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:13:34 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:13:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca822e6ba2fafa543991c7a6a40f34c01cc87fe3901534e562deb088176d7493`  
		Last Modified: Fri, 07 Jan 2022 02:15:44 GMT  
		Size: 85.7 MB (85703479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c51cef86fe6d8c848b23bf9356efd72d40eb9309423f30fb15cbc4c2742b45`  
		Last Modified: Fri, 07 Jan 2022 02:15:33 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d51d8356f23b73c45579abe97c2e7ae9fea11535c8a366b335e028731fdcc83`  
		Last Modified: Fri, 07 Jan 2022 02:15:32 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1503bacdf75977cb3264983f76442c8a2cce1ef3523605d38ea96570902981`  
		Last Modified: Fri, 07 Jan 2022 02:15:30 GMT  
		Size: 546.9 KB (546946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed14de4751c7e19603293038d3df64d993cb9d3d11f701dee5c99be24e969176`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2056d740f0a61d6cfbc612462f1f2bfc55803aabfa51d83a0c69e01e381430da`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 6.9 KB (6920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9ba6429c757c2825161ef4d1df346c4a723c950961988d2608a8fd4e35a7bc`  
		Last Modified: Fri, 07 Jan 2022 02:16:02 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995da71b9130454ebc7011f734b6911ae7ea272154ef258fc2d2baa7a3e0f360`  
		Last Modified: Fri, 07 Jan 2022 02:15:55 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:ac1416c77bcac78a9298a94a94abbefde6a84f30d1c8c6ddb9d974813850e64d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233842751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f570d1f0ea23c7cb3e2af3d23faa36d28d1e857626b870b352bb5bed8d9921`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 06 Oct 2021 17:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 17:46:47 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 06 Oct 2021 17:46:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 06 Oct 2021 17:47:20 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 06 Oct 2021 17:47:24 GMT
ARG BONITA_VERSION
# Wed, 06 Oct 2021 17:49:45 GMT
ARG BRANDING_VERSION
# Wed, 06 Oct 2021 17:49:48 GMT
ARG BONITA_SHA256
# Wed, 06 Oct 2021 17:49:51 GMT
ARG BASE_URL
# Wed, 06 Oct 2021 17:49:55 GMT
ARG BONITA_URL
# Wed, 06 Oct 2021 17:50:00 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 06 Oct 2021 17:50:05 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 06 Oct 2021 17:50:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 06 Oct 2021 17:50:17 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 06 Oct 2021 17:50:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 06 Oct 2021 17:50:24 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 06 Oct 2021 17:50:33 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 06 Oct 2021 17:50:46 GMT
RUN mkdir /opt/files
# Wed, 06 Oct 2021 17:50:49 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 06 Oct 2021 17:51:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 06 Oct 2021 17:51:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 06 Oct 2021 17:52:20 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 06 Oct 2021 17:52:34 GMT
VOLUME [/opt/bonita]
# Wed, 06 Oct 2021 17:52:38 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 06 Oct 2021 17:52:43 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 17:52:52 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3edc21cfc352b7713634c746e33cbc4fa7e3ca0a6a30ff4b38e53392c9b32`  
		Last Modified: Wed, 06 Oct 2021 17:54:27 GMT  
		Size: 86.4 MB (86436862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018aca2fc40ed2d9ef571ad40cece30b4b96114ea033190abeebc6b26f1159a`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1a43207f8aeb2bffccebb563d56f146a642348a74c917fccedc5406ff7c048`  
		Last Modified: Wed, 06 Oct 2021 17:54:13 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944db579c4969b5a1590926d71763dcdeff12d81aa7bc74411ea87c3999aa9c9`  
		Last Modified: Wed, 06 Oct 2021 17:54:11 GMT  
		Size: 546.7 KB (546726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bb1157a2d16356c3fe03471316decff49b6dc50796a886d2fb6537ec3c3b21`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3c397b4e693ea0a648aa5d5d11a1d68a1688c3894e594755a4c7b9ab141155`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd833d0ae3726dfae569704a9b090ee2eb0dc552d22117765785b6bfbc7a682f`  
		Last Modified: Wed, 06 Oct 2021 17:54:48 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c02458dc3f64372d814c185b974e07b342eec4c2dabd730f6e29a0f1e1b7d56`  
		Last Modified: Wed, 06 Oct 2021 17:54:39 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13`

```console
$ docker pull bonita@sha256:9a3b4f11a5f355af70bf2f7fb4563972bce6ee11fe5152d72a11a9f5293ed3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13` - linux; amd64

```console
$ docker pull bonita@sha256:ed211d8966e81479a0de35d88067abc19128f5115f4ed0a18583d0109418c320
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235020325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f34dfd6f06c782fe12de949e94a95aec280a87fede53c2ecf93bdd31c1415`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:45:29 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:45:30 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:45:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:45:41 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:45:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:45:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:44 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:45:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:45:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:45:57 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:45:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:58 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97708e1be04f300190a6447eb5701bf6136bde08c7fc9d2f100554dee600862f`  
		Last Modified: Fri, 07 Jan 2022 02:47:23 GMT  
		Size: 93.6 MB (93576944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ccaf14419ce16922f1fadc9c0cfca941583821338487070f248663793e6a60`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee464fd0cad364188182240e3445e5ef7d60fcd8b054ea0f81f87bf26f2c1512`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30817fa401eb65a7fe63940c50cc18df1e57394daaec77595f0084faaa94d9b`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.0 MB (1003220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd02559b7c70dc211f68f796d7deef9233732d34de4041ea0e1b352b27736ef`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35076f161983cdfb4a547a85ce068f58dc441047b1ccc6cd3f1db1afbd64a40`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec320074cb8322b6f32e97f7fd43f3e74bceb2525a35c4d4003827d7891d876f`  
		Last Modified: Fri, 07 Jan 2022 02:47:15 GMT  
		Size: 113.7 MB (113727934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7f49324ac46378dd042d253b551c923c11f94b0f5328e3e242837544501e19`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e7dc23c1c127163649ca01a096ffa92d034bf77da4f1f174af5c8ddb4f83e870
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.1 MB (224094739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561be5fff3a0045b486baa9db80b475e8c51bacf50e62007dd73a619477d8922`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:14:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:14:24 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:14:25 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:14:26 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:14:27 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:14:28 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:14:29 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:14:30 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:14:31 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:14:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:14:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:14:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:36 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:14:38 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:14:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:14:46 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:14:47 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:14:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:14:50 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:14:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402cc759bf42029a19e7ddfcc42dc0db85ecb4bd43c89e8e3e1e0f7498cff516`  
		Last Modified: Fri, 07 Jan 2022 02:16:30 GMT  
		Size: 85.7 MB (85703427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da0cfcb5c10e4b2dc1bab617e8c29a34bb963f3e9ffa94e92c6c38f3bebeb04`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61837014e57970f4f06446a4c60d4f3cf530889c0fc449e3b4d758d8d4179c78`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2b8055c41250c722a929d047034ec9405cb0ee956a0be28f44d1e97a044f3a`  
		Last Modified: Fri, 07 Jan 2022 02:16:17 GMT  
		Size: 929.4 KB (929406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a9192b771b82b241d0bd13fa7ec48f7748732d4ea523071d6380c9054e1bb0`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8817c2a9b0f82e4e5e851a7431064c1dbfea617a62b83d8ff82852c72ece60`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f424b7e4fabf4819c12d14f9e2f95f08ca015a46b0be6e7cbc551ab9bd7eb5`  
		Last Modified: Fri, 07 Jan 2022 02:16:29 GMT  
		Size: 113.7 MB (113727903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a990cce3d3807e01700ddcaf1423e46f68f4b5444f90731f8c07548b71962`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13` - linux; ppc64le

```console
$ docker pull bonita@sha256:8f84286a16f847ace8b3ba19ce8ad3610d7cee0ee4fe2949cb336a18dd5a32e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e940107c65dc134dd59beb4e8fd39205865773d8dee6a0452f3d2436591ac92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 19:19:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 19:20:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 19:20:16 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 19:20:37 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 19:20:44 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 19:20:50 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 19:20:53 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 19:20:57 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 19:21:00 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 19:21:01 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 19:21:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 19:21:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 19:21:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 19:21:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:26 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 19:21:28 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 19:21:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 19:21:49 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 19:21:57 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 19:21:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 19:22:03 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 19:22:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d89d6ede66e22e682b17c5fb5b2665ee97d7f7d155861dda91815620662729`  
		Last Modified: Thu, 07 Oct 2021 19:23:14 GMT  
		Size: 86.4 MB (86437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fce009be160a4fe12d228556c91a26fda3281f23c16ec6136dea0a080ad37`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a62824290cee741a0aeb9676745be2c616eaa8dcd4ce7b949df063b35a1e16`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3250c10bd3ceef93513e091b435d9897e902f8ea3ea62f967eb4dc76a75b7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 904.2 KB (904197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e4b367f2ce3d9341f43a189bb7c26cbf78cc7c571661df9d2d1793e1ef2914`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6914c214de6daae2dd2e975b43ded87b3e54adb9560308f7769d1607bea7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e28e1cffdb6e7a72d3e63da9a49539242b8d4fa50dbecec5ff825c8942f0a6`  
		Last Modified: Thu, 07 Oct 2021 19:23:07 GMT  
		Size: 113.7 MB (113727917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc8bb2f32fefca639b2ccaffdf8d9cf883c5d510e0093ee31525ccbbf1df8d5`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.13.0`

```console
$ docker pull bonita@sha256:9a3b4f11a5f355af70bf2f7fb4563972bce6ee11fe5152d72a11a9f5293ed3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.13.0` - linux; amd64

```console
$ docker pull bonita@sha256:ed211d8966e81479a0de35d88067abc19128f5115f4ed0a18583d0109418c320
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235020325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f34dfd6f06c782fe12de949e94a95aec280a87fede53c2ecf93bdd31c1415`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:45:29 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:45:30 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:45:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:45:41 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:45:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:45:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:44 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:45:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:45:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:45:57 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:45:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:58 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97708e1be04f300190a6447eb5701bf6136bde08c7fc9d2f100554dee600862f`  
		Last Modified: Fri, 07 Jan 2022 02:47:23 GMT  
		Size: 93.6 MB (93576944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ccaf14419ce16922f1fadc9c0cfca941583821338487070f248663793e6a60`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee464fd0cad364188182240e3445e5ef7d60fcd8b054ea0f81f87bf26f2c1512`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30817fa401eb65a7fe63940c50cc18df1e57394daaec77595f0084faaa94d9b`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.0 MB (1003220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd02559b7c70dc211f68f796d7deef9233732d34de4041ea0e1b352b27736ef`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35076f161983cdfb4a547a85ce068f58dc441047b1ccc6cd3f1db1afbd64a40`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec320074cb8322b6f32e97f7fd43f3e74bceb2525a35c4d4003827d7891d876f`  
		Last Modified: Fri, 07 Jan 2022 02:47:15 GMT  
		Size: 113.7 MB (113727934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7f49324ac46378dd042d253b551c923c11f94b0f5328e3e242837544501e19`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e7dc23c1c127163649ca01a096ffa92d034bf77da4f1f174af5c8ddb4f83e870
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.1 MB (224094739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561be5fff3a0045b486baa9db80b475e8c51bacf50e62007dd73a619477d8922`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:14:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:14:24 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:14:25 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:14:26 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:14:27 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:14:28 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:14:29 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:14:30 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:14:31 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:14:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:14:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:14:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:36 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:14:38 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:14:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:14:46 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:14:47 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:14:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:14:50 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:14:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402cc759bf42029a19e7ddfcc42dc0db85ecb4bd43c89e8e3e1e0f7498cff516`  
		Last Modified: Fri, 07 Jan 2022 02:16:30 GMT  
		Size: 85.7 MB (85703427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da0cfcb5c10e4b2dc1bab617e8c29a34bb963f3e9ffa94e92c6c38f3bebeb04`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61837014e57970f4f06446a4c60d4f3cf530889c0fc449e3b4d758d8d4179c78`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2b8055c41250c722a929d047034ec9405cb0ee956a0be28f44d1e97a044f3a`  
		Last Modified: Fri, 07 Jan 2022 02:16:17 GMT  
		Size: 929.4 KB (929406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a9192b771b82b241d0bd13fa7ec48f7748732d4ea523071d6380c9054e1bb0`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8817c2a9b0f82e4e5e851a7431064c1dbfea617a62b83d8ff82852c72ece60`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f424b7e4fabf4819c12d14f9e2f95f08ca015a46b0be6e7cbc551ab9bd7eb5`  
		Last Modified: Fri, 07 Jan 2022 02:16:29 GMT  
		Size: 113.7 MB (113727903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a990cce3d3807e01700ddcaf1423e46f68f4b5444f90731f8c07548b71962`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.13.0` - linux; ppc64le

```console
$ docker pull bonita@sha256:8f84286a16f847ace8b3ba19ce8ad3610d7cee0ee4fe2949cb336a18dd5a32e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e940107c65dc134dd59beb4e8fd39205865773d8dee6a0452f3d2436591ac92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 19:19:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 19:20:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 19:20:16 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 19:20:37 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 19:20:44 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 19:20:50 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 19:20:53 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 19:20:57 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 19:21:00 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 19:21:01 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 19:21:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 19:21:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 19:21:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 19:21:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:26 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 19:21:28 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 19:21:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 19:21:49 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 19:21:57 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 19:21:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 19:22:03 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 19:22:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d89d6ede66e22e682b17c5fb5b2665ee97d7f7d155861dda91815620662729`  
		Last Modified: Thu, 07 Oct 2021 19:23:14 GMT  
		Size: 86.4 MB (86437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fce009be160a4fe12d228556c91a26fda3281f23c16ec6136dea0a080ad37`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a62824290cee741a0aeb9676745be2c616eaa8dcd4ce7b949df063b35a1e16`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3250c10bd3ceef93513e091b435d9897e902f8ea3ea62f967eb4dc76a75b7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 904.2 KB (904197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e4b367f2ce3d9341f43a189bb7c26cbf78cc7c571661df9d2d1793e1ef2914`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6914c214de6daae2dd2e975b43ded87b3e54adb9560308f7769d1607bea7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e28e1cffdb6e7a72d3e63da9a49539242b8d4fa50dbecec5ff825c8942f0a6`  
		Last Modified: Thu, 07 Oct 2021 19:23:07 GMT  
		Size: 113.7 MB (113727917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc8bb2f32fefca639b2ccaffdf8d9cf883c5d510e0093ee31525ccbbf1df8d5`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:9a3b4f11a5f355af70bf2f7fb4563972bce6ee11fe5152d72a11a9f5293ed3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:ed211d8966e81479a0de35d88067abc19128f5115f4ed0a18583d0109418c320
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235020325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:320f34dfd6f06c782fe12de949e94a95aec280a87fede53c2ecf93bdd31c1415`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:21 GMT
ADD file:2aa3e79e3cff3c048612744ac310cf86bc27de3433d420711bafc6612445befc in / 
# Fri, 07 Jan 2022 02:25:21 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:43:09 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:45:29 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:45:30 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:45:41 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:45:41 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:45:42 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:45:43 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:43 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:45:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:45:44 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:45:45 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:45:56 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:45:57 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:45:57 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:45:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:45:58 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:45:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2f94e549220aea96f00cae7eb95f401e61b41a16cc5eb0b4ea592d0ce871930a`  
		Last Modified: Thu, 06 Jan 2022 23:50:21 GMT  
		Size: 26.7 MB (26705027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97708e1be04f300190a6447eb5701bf6136bde08c7fc9d2f100554dee600862f`  
		Last Modified: Fri, 07 Jan 2022 02:47:23 GMT  
		Size: 93.6 MB (93576944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ccaf14419ce16922f1fadc9c0cfca941583821338487070f248663793e6a60`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee464fd0cad364188182240e3445e5ef7d60fcd8b054ea0f81f87bf26f2c1512`  
		Last Modified: Fri, 07 Jan 2022 02:47:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30817fa401eb65a7fe63940c50cc18df1e57394daaec77595f0084faaa94d9b`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.0 MB (1003220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd02559b7c70dc211f68f796d7deef9233732d34de4041ea0e1b352b27736ef`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35076f161983cdfb4a547a85ce068f58dc441047b1ccc6cd3f1db1afbd64a40`  
		Last Modified: Fri, 07 Jan 2022 02:47:07 GMT  
		Size: 3.3 KB (3307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec320074cb8322b6f32e97f7fd43f3e74bceb2525a35c4d4003827d7891d876f`  
		Last Modified: Fri, 07 Jan 2022 02:47:15 GMT  
		Size: 113.7 MB (113727934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7f49324ac46378dd042d253b551c923c11f94b0f5328e3e242837544501e19`  
		Last Modified: Fri, 07 Jan 2022 02:47:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e7dc23c1c127163649ca01a096ffa92d034bf77da4f1f174af5c8ddb4f83e870
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.1 MB (224094739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561be5fff3a0045b486baa9db80b475e8c51bacf50e62007dd73a619477d8922`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:37 GMT
ADD file:def71737de83b2ed2d5ddb5520331ef14ccd496fc11b4f830b79318dd65164a3 in / 
# Fri, 07 Jan 2022 01:53:38 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:11:57 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 07 Jan 2022 02:14:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:14:12 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 07 Jan 2022 02:14:13 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 07 Jan 2022 02:14:24 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 07 Jan 2022 02:14:25 GMT
ARG BONITA_VERSION
# Fri, 07 Jan 2022 02:14:26 GMT
ARG BRANDING_VERSION
# Fri, 07 Jan 2022 02:14:27 GMT
ARG BONITA_SHA256
# Fri, 07 Jan 2022 02:14:28 GMT
ARG BASE_URL
# Fri, 07 Jan 2022 02:14:29 GMT
ARG BONITA_URL
# Fri, 07 Jan 2022 02:14:30 GMT
ENV BONITA_VERSION=7.13.0
# Fri, 07 Jan 2022 02:14:31 GMT
ENV BRANDING_VERSION=2021.2-u0
# Fri, 07 Jan 2022 02:14:32 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Fri, 07 Jan 2022 02:14:33 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:34 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 07 Jan 2022 02:14:35 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Fri, 07 Jan 2022 02:14:36 GMT
RUN mkdir /opt/files
# Fri, 07 Jan 2022 02:14:38 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Fri, 07 Jan 2022 02:14:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Fri, 07 Jan 2022 02:14:46 GMT
ENV HTTP_API=false
# Fri, 07 Jan 2022 02:14:47 GMT
VOLUME [/opt/bonita]
# Fri, 07 Jan 2022 02:14:49 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 07 Jan 2022 02:14:50 GMT
EXPOSE 8080
# Fri, 07 Jan 2022 02:14:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:976e4515cbe3bb05d3eaff6aa830f00c2593211ff7600840d5e9a030c803bbee`  
		Last Modified: Fri, 07 Jan 2022 01:55:15 GMT  
		Size: 23.7 MB (23726915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402cc759bf42029a19e7ddfcc42dc0db85ecb4bd43c89e8e3e1e0f7498cff516`  
		Last Modified: Fri, 07 Jan 2022 02:16:30 GMT  
		Size: 85.7 MB (85703427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da0cfcb5c10e4b2dc1bab617e8c29a34bb963f3e9ffa94e92c6c38f3bebeb04`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61837014e57970f4f06446a4c60d4f3cf530889c0fc449e3b4d758d8d4179c78`  
		Last Modified: Fri, 07 Jan 2022 02:16:19 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2b8055c41250c722a929d047034ec9405cb0ee956a0be28f44d1e97a044f3a`  
		Last Modified: Fri, 07 Jan 2022 02:16:17 GMT  
		Size: 929.4 KB (929406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a9192b771b82b241d0bd13fa7ec48f7748732d4ea523071d6380c9054e1bb0`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8817c2a9b0f82e4e5e851a7431064c1dbfea617a62b83d8ff82852c72ece60`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f424b7e4fabf4819c12d14f9e2f95f08ca015a46b0be6e7cbc551ab9bd7eb5`  
		Last Modified: Fri, 07 Jan 2022 02:16:29 GMT  
		Size: 113.7 MB (113727903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a990cce3d3807e01700ddcaf1423e46f68f4b5444f90731f8c07548b71962`  
		Last Modified: Fri, 07 Jan 2022 02:16:16 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:8f84286a16f847ace8b3ba19ce8ad3610d7cee0ee4fe2949cb336a18dd5a32e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e940107c65dc134dd59beb4e8fd39205865773d8dee6a0452f3d2436591ac92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:29 GMT
ADD file:fd96554dfb72307c3cf9292c343050a8b9f0848735b7555820f0068914ebd758 in / 
# Tue, 05 Oct 2021 11:07:35 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 17:43:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 07 Oct 2021 19:19:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends       curl       gnupg2       mysql-client-core-5.7       openjdk-11-jre-headless       postgresql-client       unzip       zip   && rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 19:20:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 07 Oct 2021 19:20:16 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 07 Oct 2021 19:20:37 GMT
RUN gpg --keyserver keyserver.ubuntu.com --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.13/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 07 Oct 2021 19:20:44 GMT
ARG BONITA_VERSION
# Thu, 07 Oct 2021 19:20:50 GMT
ARG BRANDING_VERSION
# Thu, 07 Oct 2021 19:20:53 GMT
ARG BONITA_SHA256
# Thu, 07 Oct 2021 19:20:57 GMT
ARG BASE_URL
# Thu, 07 Oct 2021 19:21:00 GMT
ARG BONITA_URL
# Thu, 07 Oct 2021 19:21:01 GMT
ENV BONITA_VERSION=7.13.0
# Thu, 07 Oct 2021 19:21:05 GMT
ENV BRANDING_VERSION=2021.2-u0
# Thu, 07 Oct 2021 19:21:11 GMT
ENV BONITA_SHA256=e4f279765cd729885a4e353d96d1d85c5f69fef63f79183e0ccf3ffaa0cb2417
# Thu, 07 Oct 2021 19:21:15 GMT
ENV ZIP_FILE=BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 07 Oct 2021 19:21:20 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.2-u0/BonitaCommunity-2021.2-u0.zip
# Thu, 07 Oct 2021 19:21:26 GMT
RUN mkdir /opt/files
# Thu, 07 Oct 2021 19:21:28 GMT
COPY dir:6250b774ea0abc098d97c259e44608a8bf8835310bd84b47cecb5b027fb6826b in /opt/files 
# Thu, 07 Oct 2021 19:21:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi   && sha256sum /opt/files/${ZIP_FILE}   && echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -   && unzip -q /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip -d /opt/bonita/   && unzip /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war -d /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita/   && rm /opt/bonita/BonitaCommunity-${BRANDING_VERSION}/server/webapps/bonita.war   && rm -f /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip
# Thu, 07 Oct 2021 19:21:49 GMT
ENV HTTP_API=false
# Thu, 07 Oct 2021 19:21:57 GMT
VOLUME [/opt/bonita]
# Thu, 07 Oct 2021 19:21:58 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 07 Oct 2021 19:22:03 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 19:22:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:db28fc1e594e5598e665c54ac1b7fd602d86dddaf8bb237a72303cec22a9185c`  
		Last Modified: Tue, 05 Oct 2021 11:10:31 GMT  
		Size: 30.4 MB (30432921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d89d6ede66e22e682b17c5fb5b2665ee97d7f7d155861dda91815620662729`  
		Last Modified: Thu, 07 Oct 2021 19:23:14 GMT  
		Size: 86.4 MB (86437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fce009be160a4fe12d228556c91a26fda3281f23c16ec6136dea0a080ad37`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a62824290cee741a0aeb9676745be2c616eaa8dcd4ce7b949df063b35a1e16`  
		Last Modified: Thu, 07 Oct 2021 19:22:59 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3250c10bd3ceef93513e091b435d9897e902f8ea3ea62f967eb4dc76a75b7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 904.2 KB (904197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e4b367f2ce3d9341f43a189bb7c26cbf78cc7c571661df9d2d1793e1ef2914`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045f6914c214de6daae2dd2e975b43ded87b3e54adb9560308f7769d1607bea7`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 3.3 KB (3308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e28e1cffdb6e7a72d3e63da9a49539242b8d4fa50dbecec5ff825c8942f0a6`  
		Last Modified: Thu, 07 Oct 2021 19:23:07 GMT  
		Size: 113.7 MB (113727917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc8bb2f32fefca639b2ccaffdf8d9cf883c5d510e0093ee31525ccbbf1df8d5`  
		Last Modified: Thu, 07 Oct 2021 19:22:57 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
