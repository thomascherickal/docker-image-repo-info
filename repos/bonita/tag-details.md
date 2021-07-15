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
$ docker pull bonita@sha256:e7b3f12dd62820806337d92a2abb053c8ac4893ec44a8b17c8085ecbb32736ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:ca94d2e7f5bbb0b99ea21f5d28953f5b251429780269ff6b72faba3a1166deee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237176579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c082732516f02e2420afb55f7ea56a975fd95c1d054cd606948e955733b0cb1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:50:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 22:50:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:50:57 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:50:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:51:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:51:01 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 22:51:28 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:30 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 22:51:31 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 22:51:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 22:51:35 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 22:51:37 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 22:51:39 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 22:51:39 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:51:39 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 22:51:40 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:51:40 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8d7f47c4c91b8d9dbce730b796e70940a94024d9deb6fe6c3c7a3c097b837`  
		Last Modified: Tue, 13 Jul 2021 22:53:00 GMT  
		Size: 93.5 MB (93468936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d57029df8192f7fe92beee6610f11707e2b36a3d87f3a4699dbba6fe558a61`  
		Last Modified: Tue, 13 Jul 2021 22:52:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24804a7ca337850329a0363fbc58cdaef060aa67650f7f5826b22714b45eb32b`  
		Last Modified: Tue, 13 Jul 2021 22:52:40 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d52e992561df06f2a88902eb1eae5f59f672d405d214e7e2b6f0385c1638c`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 575.3 KB (575254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf61e6427078809c42793b5f22fd21f92553a46d21fc49d8c56b7943fe4fb2`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f57c93c1bafbca439485a348b5d878cd324adfc4f818da9edb6b8bc5539e32`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f2ee158830adb62106fca0a7dcbf70dabcd078fba1eb71b5b2a19e867dcb6`  
		Last Modified: Tue, 13 Jul 2021 22:53:20 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08860bc426f481ccaa9b5cf7e2b91ad5c9cb5b71f7b3cddcc8d944368922c8cd`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:32cb588b373c3845a9d74d5ddab498f9d98df525709303a177b62fb5d19a694a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226288317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7058c8e16114eba430521762990dc50b33c9f2bbc6ff3f13a23513a981a25843`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:29:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 23:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:30:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:30:08 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 23:30:27 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:28 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 23:30:29 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 23:30:29 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 23:30:33 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 23:30:34 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 23:30:36 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 23:30:36 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:30:36 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 23:30:36 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:30:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b2d40d48563623b5da173028af540053694b83df5a1fa4033dcc46d5d0108f`  
		Last Modified: Tue, 13 Jul 2021 23:31:53 GMT  
		Size: 85.6 MB (85585613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaa3e5d5e3aa193ba5788e79d26cecbb288990bf94e34a0b09f4b1ceb66583`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc45aa8282d969a51cad8f0533fef4323cfad7c72ece492176d04a6331571eb9`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05133f4e2f35fb0b63eec6c0b888d4869ba796b2d817baba42abd64d8af2b951`  
		Last Modified: Tue, 13 Jul 2021 23:31:36 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b57dc4d2d4fdbace1ca3de4ec8f30cec16747b639f63cfc977479803d1988`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982e0e6118afaa6d9a609ccbac3ad25d1357b66b944626f1a1d5807e9ca8fa2f`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e1acb7a095d261a173aa38cf2c4af10431dafa3ced90106095fe88b4d791bb`  
		Last Modified: Tue, 13 Jul 2021 23:32:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd65387ac6e82414900048ffaa5e690250c839a2605b67d830ff2057f99a407`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:6d42098255d7f0cc80c2f0ffb70c5c76e99739651e6aac3c2716d1e8c9ab3bad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233796336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efda9e0b763ba1558488a71d85829892d6d9dcf7a7549ca1cb1052667717c9dc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:23:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jul 2021 04:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:28:27 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:28:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:29:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:29:17 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:32:59 GMT
ARG BRANDING_VERSION
# Wed, 14 Jul 2021 04:33:01 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:33:08 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:33:17 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:33:21 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 14 Jul 2021 04:33:24 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 14 Jul 2021 04:33:39 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 14 Jul 2021 04:33:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:33:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:33:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:34:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 14 Jul 2021 04:34:21 GMT
RUN mkdir /opt/files
# Wed, 14 Jul 2021 04:34:26 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 14 Jul 2021 04:34:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 14 Jul 2021 04:34:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 14 Jul 2021 04:35:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 14 Jul 2021 04:35:08 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:35:11 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 14 Jul 2021 04:35:15 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:35:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6d20994673343d11028ac1ac0bcc098d0f1ac3b04655623d2d2cafa4bee8d`  
		Last Modified: Wed, 14 Jul 2021 04:37:02 GMT  
		Size: 86.4 MB (86395354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a025e3dd302981f640be07c88365b3ddfa8c7d2a818971b050001fa255123`  
		Last Modified: Wed, 14 Jul 2021 04:36:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c867ae2580be2a8356c180288cecbeca16488f530908d5ebb203c0c5bf0a99`  
		Last Modified: Wed, 14 Jul 2021 04:36:44 GMT  
		Size: 1.9 KB (1900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732888c6ddf76b2f60aa2ce9638a1b17b4a33dc96c7a969b6b0a3401b8c8568`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 546.7 KB (546731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01503d0bfb3e8749a1da3e2fe6cbf5e5208d577a78b429c339ba548a3e20f3aa`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91434b0d6bc799538f5ccea05a983777aa3db998cee240f7e841f059c8982d1`  
		Last Modified: Wed, 14 Jul 2021 04:37:16 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ceb99ecfc3b3526d131f1a01116aaaf5821a5a16c59e76ea0e83d14b7c0b5f`  
		Last Modified: Wed, 14 Jul 2021 04:37:26 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b028984ead8def425d58ddd729fc1448e107673994a53e44d976baf1ae7ad0`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10`

```console
$ docker pull bonita@sha256:5f7a4730c8e4edec47fe8fd68b6d6efe52a7625ed9125aa993b348098bf88ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:bf3c98910077fd61eb70352b4b1aec263b071d47af70a341c146cbfa636088f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242296295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c735c55d4b705d7571e70a096c47a4d0f866430299c0996e1e5511f6ced6aa87`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:47:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Tue, 13 Jul 2021 22:49:39 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:49:41 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:49:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:49:47 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:49:48 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:49:48 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:49:48 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:49:49 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:49:49 GMT
ENV BONITA_VERSION=7.10.6
# Tue, 13 Jul 2021 22:49:49 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Tue, 13 Jul 2021 22:49:50 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:49:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Tue, 13 Jul 2021 22:49:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 13 Jul 2021 22:49:57 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 22:50:00 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 22:50:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 13 Jul 2021 22:50:03 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:50:04 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Tue, 13 Jul 2021 22:50:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 13 Jul 2021 22:50:05 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:50:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab28a633dfc06139dc97d8d5d7c76d27af168535c1b9accb391a16613aefd8d`  
		Last Modified: Tue, 13 Jul 2021 22:52:26 GMT  
		Size: 117.0 MB (117027883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e70999f655d0891e916ba694de58878791cca6c2b064302f774401da11b34b`  
		Last Modified: Tue, 13 Jul 2021 22:52:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a89d207289c3e10d273667409a14fa849c1781c54b4a507473942e8eca67d7`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 1.9 KB (1911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a889f742a84ea3b440fb7b086815903c65b6fffe49db7777d103ce729bff9`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a727924898c9beaf564d038fa6d0396a3b1f065eddf5944d60dff4ed2ba948d`  
		Last Modified: Tue, 13 Jul 2021 22:52:09 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc23bede567c4a4905082333f77e2adc3c057d733a29b669d6ef3144a723b08`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acb58634e5459fa65bc25f76807991c11eb120c4902fb3c024fe0638413af7a`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dd9586dc2c4bb37eda52b61d69d05eebd5d78d765af1773ba2d5c593d3267212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230995494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8fcbf17e17c0d45771b38ade9c283da4f5940a6e9ea71562333d95c0ca3b5e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:28:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Tue, 13 Jul 2021 23:29:19 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:29:21 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:29:21 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:29:25 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:29:25 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:29:26 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:29:26 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:29:26 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:29:26 GMT
ENV BONITA_VERSION=7.10.6
# Tue, 13 Jul 2021 23:29:27 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Tue, 13 Jul 2021 23:29:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:29:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Tue, 13 Jul 2021 23:29:28 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 13 Jul 2021 23:29:31 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 23:29:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 23:29:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 13 Jul 2021 23:29:34 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:29:34 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Tue, 13 Jul 2021 23:29:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 13 Jul 2021 23:29:35 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:29:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa5798c422ccff43652d8f8e47b801e87fb7e48e1c02a22801252bce5d8f40`  
		Last Modified: Tue, 13 Jul 2021 23:31:23 GMT  
		Size: 108.7 MB (108733705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1c124349ba3d39cea452b525015e9bfb6ab84c363ee6104c17eed87e75914`  
		Last Modified: Tue, 13 Jul 2021 23:31:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed33706eebfb9c64446b0c81fec102b4a50c54056c501689a6a5242f14114cf2`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 1.9 KB (1915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7478f54d2915b55db991b7ed108a91a8739d82d2d11207d90cac1204860108f8`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 547.0 KB (546954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b7722bbb94f07206f77d4c2b49041adf8aeca79e82ca1c085032758cd87fac`  
		Last Modified: Tue, 13 Jul 2021 23:31:10 GMT  
		Size: 98.0 MB (97973963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02fbaab1afb7e6246d991a6a73d11feba8553e3c85663152eaf14389ebba75a`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 7.7 KB (7652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7ea066646762f10c025c1d435a48606d4242a64f90e77131c20f174384fb4d`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:20332bc4ee4a8a974c2b32ad4745dfdc968508cea96a30d3db2aa20e3baea6de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240271367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77234d27352ad11f8224312ff3ad45419019199c47f3f7ba19de7eb6f4f96f2b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:08:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 14 Jul 2021 04:19:12 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:19:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:19:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:20:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:20:22 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:20:40 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:20:49 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:20:55 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:21:00 GMT
ENV BONITA_VERSION=7.10.6
# Wed, 14 Jul 2021 04:21:03 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Wed, 14 Jul 2021 04:21:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:21:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Wed, 14 Jul 2021 04:21:31 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 14 Jul 2021 04:21:52 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 14 Jul 2021 04:22:06 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 14 Jul 2021 04:22:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 14 Jul 2021 04:22:29 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:22:32 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Wed, 14 Jul 2021 04:22:37 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 14 Jul 2021 04:22:43 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:22:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2553da853866173ce9729df14e099165262b630df5f2072bbdb6947ac4f95b80`  
		Last Modified: Wed, 14 Jul 2021 04:36:23 GMT  
		Size: 111.3 MB (111311300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788967d9c19b9b7dd0c8ee83597d3b05172d86a419ca589a8e8368b2ac77cb7b`  
		Last Modified: Wed, 14 Jul 2021 04:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437884138b6c53d6a43c99e8dd16a8d76b4eb153676b68d3f2d69ba95439a902`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5463917c53c3914b5f613e2a27ff62925e7995c8812a6c0a064547b9e691a49`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbdeaae0326f56e4805363bcdfa6732a6c89fa953e841597e0da8c2f6d7b979`  
		Last Modified: Wed, 14 Jul 2021 04:36:06 GMT  
		Size: 98.0 MB (97973963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1217386105f4000a8a625d18b342c35a333d072132b16f6cdb7699bc43ffa4a2`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21eb31509ac553404bedddbf106a2136791cbea246c5c78309c40033273795c8`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:5f7a4730c8e4edec47fe8fd68b6d6efe52a7625ed9125aa993b348098bf88ed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.6` - linux; amd64

```console
$ docker pull bonita@sha256:bf3c98910077fd61eb70352b4b1aec263b071d47af70a341c146cbfa636088f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242296295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c735c55d4b705d7571e70a096c47a4d0f866430299c0996e1e5511f6ced6aa87`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:47:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Tue, 13 Jul 2021 22:49:39 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:49:41 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:49:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:49:47 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:49:48 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:49:48 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:49:48 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:49:49 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:49:49 GMT
ENV BONITA_VERSION=7.10.6
# Tue, 13 Jul 2021 22:49:49 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Tue, 13 Jul 2021 22:49:50 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:49:50 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Tue, 13 Jul 2021 22:49:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 13 Jul 2021 22:49:57 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 22:50:00 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 22:50:03 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 13 Jul 2021 22:50:03 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:50:04 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Tue, 13 Jul 2021 22:50:04 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 13 Jul 2021 22:50:05 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:50:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab28a633dfc06139dc97d8d5d7c76d27af168535c1b9accb391a16613aefd8d`  
		Last Modified: Tue, 13 Jul 2021 22:52:26 GMT  
		Size: 117.0 MB (117027883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e70999f655d0891e916ba694de58878791cca6c2b064302f774401da11b34b`  
		Last Modified: Tue, 13 Jul 2021 22:52:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a89d207289c3e10d273667409a14fa849c1781c54b4a507473942e8eca67d7`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 1.9 KB (1911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a889f742a84ea3b440fb7b086815903c65b6fffe49db7777d103ce729bff9`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 576.9 KB (576940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a727924898c9beaf564d038fa6d0396a3b1f065eddf5944d60dff4ed2ba948d`  
		Last Modified: Tue, 13 Jul 2021 22:52:09 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc23bede567c4a4905082333f77e2adc3c057d733a29b669d6ef3144a723b08`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acb58634e5459fa65bc25f76807991c11eb120c4902fb3c024fe0638413af7a`  
		Last Modified: Tue, 13 Jul 2021 22:52:01 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:dd9586dc2c4bb37eda52b61d69d05eebd5d78d765af1773ba2d5c593d3267212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230995494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8fcbf17e17c0d45771b38ade9c283da4f5940a6e9ea71562333d95c0ca3b5e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:28:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Tue, 13 Jul 2021 23:29:19 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:29:21 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:29:21 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:29:25 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:29:25 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:29:26 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:29:26 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:29:26 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:29:26 GMT
ENV BONITA_VERSION=7.10.6
# Tue, 13 Jul 2021 23:29:27 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Tue, 13 Jul 2021 23:29:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:29:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Tue, 13 Jul 2021 23:29:28 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 13 Jul 2021 23:29:31 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 23:29:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 13 Jul 2021 23:29:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 13 Jul 2021 23:29:34 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:29:34 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Tue, 13 Jul 2021 23:29:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Tue, 13 Jul 2021 23:29:35 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:29:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa5798c422ccff43652d8f8e47b801e87fb7e48e1c02a22801252bce5d8f40`  
		Last Modified: Tue, 13 Jul 2021 23:31:23 GMT  
		Size: 108.7 MB (108733705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1c124349ba3d39cea452b525015e9bfb6ab84c363ee6104c17eed87e75914`  
		Last Modified: Tue, 13 Jul 2021 23:31:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed33706eebfb9c64446b0c81fec102b4a50c54056c501689a6a5242f14114cf2`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 1.9 KB (1915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7478f54d2915b55db991b7ed108a91a8739d82d2d11207d90cac1204860108f8`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 547.0 KB (546954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b7722bbb94f07206f77d4c2b49041adf8aeca79e82ca1c085032758cd87fac`  
		Last Modified: Tue, 13 Jul 2021 23:31:10 GMT  
		Size: 98.0 MB (97973963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02fbaab1afb7e6246d991a6a73d11feba8553e3c85663152eaf14389ebba75a`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 7.7 KB (7652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7ea066646762f10c025c1d435a48606d4242a64f90e77131c20f174384fb4d`  
		Last Modified: Tue, 13 Jul 2021 23:31:04 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; ppc64le

```console
$ docker pull bonita@sha256:20332bc4ee4a8a974c2b32ad4745dfdc968508cea96a30d3db2aa20e3baea6de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240271367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77234d27352ad11f8224312ff3ad45419019199c47f3f7ba19de7eb6f4f96f2b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:08:13 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 14 Jul 2021 04:19:12 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:19:28 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:19:54 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:20:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:20:22 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:20:40 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:20:49 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:20:55 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:21:00 GMT
ENV BONITA_VERSION=7.10.6
# Wed, 14 Jul 2021 04:21:03 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Wed, 14 Jul 2021 04:21:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:21:15 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Wed, 14 Jul 2021 04:21:31 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 14 Jul 2021 04:21:52 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 14 Jul 2021 04:22:06 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 14 Jul 2021 04:22:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 14 Jul 2021 04:22:29 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:22:32 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Wed, 14 Jul 2021 04:22:37 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 14 Jul 2021 04:22:43 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:22:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2553da853866173ce9729df14e099165262b630df5f2072bbdb6947ac4f95b80`  
		Last Modified: Wed, 14 Jul 2021 04:36:23 GMT  
		Size: 111.3 MB (111311300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788967d9c19b9b7dd0c8ee83597d3b05172d86a419ca589a8e8368b2ac77cb7b`  
		Last Modified: Wed, 14 Jul 2021 04:36:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437884138b6c53d6a43c99e8dd16a8d76b4eb153676b68d3f2d69ba95439a902`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5463917c53c3914b5f613e2a27ff62925e7995c8812a6c0a064547b9e691a49`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 546.7 KB (546735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbdeaae0326f56e4805363bcdfa6732a6c89fa953e841597e0da8c2f6d7b979`  
		Last Modified: Wed, 14 Jul 2021 04:36:06 GMT  
		Size: 98.0 MB (97973963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1217386105f4000a8a625d18b342c35a333d072132b16f6cdb7699bc43ffa4a2`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21eb31509ac553404bedddbf106a2136791cbea246c5c78309c40033273795c8`  
		Last Modified: Wed, 14 Jul 2021 04:35:58 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:cd9d1ada1bbcabb9319935febd09dafc5a4579c51d4cebcbae3944c84db4381c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:7bd46ba1a5ddfb7e096f8f82628970669a02ad9165c7511cad084215fe172301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234108953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0a04e6b52b92080fef1776d88c48e66730772c40db71b9872a31a57bcf0f07`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:50:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 22:50:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:50:57 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:50:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:51:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:51:01 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:51:02 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:51:02 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:51:02 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:51:02 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 13 Jul 2021 22:51:03 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 13 Jul 2021 22:51:03 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 22:51:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:51:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 22:51:05 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 22:51:06 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 22:51:06 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 13 Jul 2021 22:51:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 13 Jul 2021 22:51:12 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 22:51:14 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 22:51:14 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:51:14 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 22:51:15 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:51:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8d7f47c4c91b8d9dbce730b796e70940a94024d9deb6fe6c3c7a3c097b837`  
		Last Modified: Tue, 13 Jul 2021 22:53:00 GMT  
		Size: 93.5 MB (93468936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d57029df8192f7fe92beee6610f11707e2b36a3d87f3a4699dbba6fe558a61`  
		Last Modified: Tue, 13 Jul 2021 22:52:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24804a7ca337850329a0363fbc58cdaef060aa67650f7f5826b22714b45eb32b`  
		Last Modified: Tue, 13 Jul 2021 22:52:40 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d52e992561df06f2a88902eb1eae5f59f672d405d214e7e2b6f0385c1638c`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 575.3 KB (575254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebfeb4aa41a275efd7e283291cb618b55dcb72cf7f75578bef5e344f1e2845f`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725fed16517858a4ed3ba10a6184ef9c40865ea372d03895f402588ac35e9c90`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf612f6ced5e7e0f47be183280edcc3deb08679074270ffce3068d3ff3ea9ef`  
		Last Modified: Tue, 13 Jul 2021 22:52:48 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e40833e2092d0e9cc51f8969e7630ce3faf028ee3e2388b6ccc7f65ee54667`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:cb9db9a1186fee76087e3f6d3b333d55d891a144af82f9da0155f150b22ea32c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223220685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7f5f390b0144ab6f793b4c68686088a65bb69cbf9d84a756628c364d92361d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:29:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 23:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:30:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:30:08 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:30:09 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 13 Jul 2021 23:30:09 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 13 Jul 2021 23:30:09 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 23:30:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:30:10 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 23:30:10 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 23:30:11 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 23:30:12 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 13 Jul 2021 23:30:15 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 13 Jul 2021 23:30:16 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 23:30:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 23:30:18 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:30:18 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 23:30:18 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:30:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b2d40d48563623b5da173028af540053694b83df5a1fa4033dcc46d5d0108f`  
		Last Modified: Tue, 13 Jul 2021 23:31:53 GMT  
		Size: 85.6 MB (85585613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaa3e5d5e3aa193ba5788e79d26cecbb288990bf94e34a0b09f4b1ceb66583`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc45aa8282d969a51cad8f0533fef4323cfad7c72ece492176d04a6331571eb9`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05133f4e2f35fb0b63eec6c0b888d4869ba796b2d817baba42abd64d8af2b951`  
		Last Modified: Tue, 13 Jul 2021 23:31:36 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8239c9c70fdc10b4661ddc5fb30f328f933a5372baee2b89576c013b723fd2e4`  
		Last Modified: Tue, 13 Jul 2021 23:31:35 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18d31676d83552679d2baba7208545548be4dbd3ce89bca69a5fd79a3f25199`  
		Last Modified: Tue, 13 Jul 2021 23:31:35 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e8d48b96d2cab7b9fbb8f55b45986d8d32f43e27bc3bcd39818aa5bf45f8b`  
		Last Modified: Tue, 13 Jul 2021 23:31:42 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2cdc3ed876a18a7416058e38260e9d07ec2226f1d2260eac79363692b6ec3`  
		Last Modified: Tue, 13 Jul 2021 23:31:35 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:2958d6a5bde9958b077c93f38afb6c34dc2004592c5d4a8f185a82fc3ca7ab20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230728713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6462a293d0d2870577a6ef14785e95017141fd3cd1414c8cd1ece04817071118`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:23:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jul 2021 04:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:28:27 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:28:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:29:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:29:17 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:29:25 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:29:32 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:29:36 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:29:40 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 14 Jul 2021 04:29:50 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 14 Jul 2021 04:29:58 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 14 Jul 2021 04:30:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:30:17 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 14 Jul 2021 04:30:32 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 14 Jul 2021 04:30:51 GMT
RUN mkdir /opt/files
# Wed, 14 Jul 2021 04:30:54 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 14 Jul 2021 04:31:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 14 Jul 2021 04:31:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 14 Jul 2021 04:32:13 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 14 Jul 2021 04:32:21 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:32:24 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 14 Jul 2021 04:32:38 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:32:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6d20994673343d11028ac1ac0bcc098d0f1ac3b04655623d2d2cafa4bee8d`  
		Last Modified: Wed, 14 Jul 2021 04:37:02 GMT  
		Size: 86.4 MB (86395354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a025e3dd302981f640be07c88365b3ddfa8c7d2a818971b050001fa255123`  
		Last Modified: Wed, 14 Jul 2021 04:36:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c867ae2580be2a8356c180288cecbeca16488f530908d5ebb203c0c5bf0a99`  
		Last Modified: Wed, 14 Jul 2021 04:36:44 GMT  
		Size: 1.9 KB (1900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732888c6ddf76b2f60aa2ce9638a1b17b4a33dc96c7a969b6b0a3401b8c8568`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 546.7 KB (546731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fe2e4073223b4d7fbdedc2545b34d8174239157725e6c0a24fbd28d9a8d19`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3547178d7d78c1496b84942e11d81ef65cfa3b32a5f6c7839a06493e4eecf0d`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 6.9 KB (6895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6540b82f34eeb6be88b346855d91ef64c48e76e0c63aa603f951375d98c145a`  
		Last Modified: Wed, 14 Jul 2021 04:36:50 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159e285cbe267e213a16b7de6a44e260147a70600c5e397e47802a7301768d81`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:cd9d1ada1bbcabb9319935febd09dafc5a4579c51d4cebcbae3944c84db4381c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:7bd46ba1a5ddfb7e096f8f82628970669a02ad9165c7511cad084215fe172301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234108953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0a04e6b52b92080fef1776d88c48e66730772c40db71b9872a31a57bcf0f07`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:50:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 22:50:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:50:57 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:50:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:51:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:51:01 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:51:02 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:51:02 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:51:02 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:51:02 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 13 Jul 2021 22:51:03 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 13 Jul 2021 22:51:03 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 22:51:03 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:51:03 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 22:51:05 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 22:51:06 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 22:51:06 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 13 Jul 2021 22:51:10 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 13 Jul 2021 22:51:12 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 22:51:14 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 22:51:14 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:51:14 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 22:51:15 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:51:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8d7f47c4c91b8d9dbce730b796e70940a94024d9deb6fe6c3c7a3c097b837`  
		Last Modified: Tue, 13 Jul 2021 22:53:00 GMT  
		Size: 93.5 MB (93468936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d57029df8192f7fe92beee6610f11707e2b36a3d87f3a4699dbba6fe558a61`  
		Last Modified: Tue, 13 Jul 2021 22:52:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24804a7ca337850329a0363fbc58cdaef060aa67650f7f5826b22714b45eb32b`  
		Last Modified: Tue, 13 Jul 2021 22:52:40 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d52e992561df06f2a88902eb1eae5f59f672d405d214e7e2b6f0385c1638c`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 575.3 KB (575254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebfeb4aa41a275efd7e283291cb618b55dcb72cf7f75578bef5e344f1e2845f`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725fed16517858a4ed3ba10a6184ef9c40865ea372d03895f402588ac35e9c90`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf612f6ced5e7e0f47be183280edcc3deb08679074270ffce3068d3ff3ea9ef`  
		Last Modified: Tue, 13 Jul 2021 22:52:48 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e40833e2092d0e9cc51f8969e7630ce3faf028ee3e2388b6ccc7f65ee54667`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:cb9db9a1186fee76087e3f6d3b333d55d891a144af82f9da0155f150b22ea32c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223220685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7f5f390b0144ab6f793b4c68686088a65bb69cbf9d84a756628c364d92361d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:29:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 23:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:30:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:30:08 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:30:09 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 13 Jul 2021 23:30:09 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 13 Jul 2021 23:30:09 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 23:30:09 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:30:10 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 13 Jul 2021 23:30:10 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 23:30:11 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 23:30:12 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 13 Jul 2021 23:30:15 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 13 Jul 2021 23:30:16 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 23:30:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 23:30:18 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:30:18 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 23:30:18 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:30:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b2d40d48563623b5da173028af540053694b83df5a1fa4033dcc46d5d0108f`  
		Last Modified: Tue, 13 Jul 2021 23:31:53 GMT  
		Size: 85.6 MB (85585613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaa3e5d5e3aa193ba5788e79d26cecbb288990bf94e34a0b09f4b1ceb66583`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc45aa8282d969a51cad8f0533fef4323cfad7c72ece492176d04a6331571eb9`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05133f4e2f35fb0b63eec6c0b888d4869ba796b2d817baba42abd64d8af2b951`  
		Last Modified: Tue, 13 Jul 2021 23:31:36 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8239c9c70fdc10b4661ddc5fb30f328f933a5372baee2b89576c013b723fd2e4`  
		Last Modified: Tue, 13 Jul 2021 23:31:35 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18d31676d83552679d2baba7208545548be4dbd3ce89bca69a5fd79a3f25199`  
		Last Modified: Tue, 13 Jul 2021 23:31:35 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e8d48b96d2cab7b9fbb8f55b45986d8d32f43e27bc3bcd39818aa5bf45f8b`  
		Last Modified: Tue, 13 Jul 2021 23:31:42 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2cdc3ed876a18a7416058e38260e9d07ec2226f1d2260eac79363692b6ec3`  
		Last Modified: Tue, 13 Jul 2021 23:31:35 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:2958d6a5bde9958b077c93f38afb6c34dc2004592c5d4a8f185a82fc3ca7ab20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230728713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6462a293d0d2870577a6ef14785e95017141fd3cd1414c8cd1ece04817071118`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:23:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jul 2021 04:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:28:27 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:28:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:29:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:29:17 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:29:25 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:29:32 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:29:36 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:29:40 GMT
ENV BONITA_VERSION=7.11.4
# Wed, 14 Jul 2021 04:29:50 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Wed, 14 Jul 2021 04:29:58 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Wed, 14 Jul 2021 04:30:05 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:30:17 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Wed, 14 Jul 2021 04:30:32 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 14 Jul 2021 04:30:51 GMT
RUN mkdir /opt/files
# Wed, 14 Jul 2021 04:30:54 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 14 Jul 2021 04:31:19 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 14 Jul 2021 04:31:55 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 14 Jul 2021 04:32:13 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 14 Jul 2021 04:32:21 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:32:24 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 14 Jul 2021 04:32:38 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:32:45 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6d20994673343d11028ac1ac0bcc098d0f1ac3b04655623d2d2cafa4bee8d`  
		Last Modified: Wed, 14 Jul 2021 04:37:02 GMT  
		Size: 86.4 MB (86395354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a025e3dd302981f640be07c88365b3ddfa8c7d2a818971b050001fa255123`  
		Last Modified: Wed, 14 Jul 2021 04:36:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c867ae2580be2a8356c180288cecbeca16488f530908d5ebb203c0c5bf0a99`  
		Last Modified: Wed, 14 Jul 2021 04:36:44 GMT  
		Size: 1.9 KB (1900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732888c6ddf76b2f60aa2ce9638a1b17b4a33dc96c7a969b6b0a3401b8c8568`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 546.7 KB (546731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fe2e4073223b4d7fbdedc2545b34d8174239157725e6c0a24fbd28d9a8d19`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3547178d7d78c1496b84942e11d81ef65cfa3b32a5f6c7839a06493e4eecf0d`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 6.9 KB (6895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6540b82f34eeb6be88b346855d91ef64c48e76e0c63aa603f951375d98c145a`  
		Last Modified: Wed, 14 Jul 2021 04:36:50 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159e285cbe267e213a16b7de6a44e260147a70600c5e397e47802a7301768d81`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:e7b3f12dd62820806337d92a2abb053c8ac4893ec44a8b17c8085ecbb32736ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:ca94d2e7f5bbb0b99ea21f5d28953f5b251429780269ff6b72faba3a1166deee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237176579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c082732516f02e2420afb55f7ea56a975fd95c1d054cd606948e955733b0cb1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:50:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 22:50:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:50:57 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:50:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:51:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:51:01 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 22:51:28 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:30 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 22:51:31 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 22:51:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 22:51:35 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 22:51:37 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 22:51:39 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 22:51:39 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:51:39 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 22:51:40 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:51:40 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8d7f47c4c91b8d9dbce730b796e70940a94024d9deb6fe6c3c7a3c097b837`  
		Last Modified: Tue, 13 Jul 2021 22:53:00 GMT  
		Size: 93.5 MB (93468936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d57029df8192f7fe92beee6610f11707e2b36a3d87f3a4699dbba6fe558a61`  
		Last Modified: Tue, 13 Jul 2021 22:52:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24804a7ca337850329a0363fbc58cdaef060aa67650f7f5826b22714b45eb32b`  
		Last Modified: Tue, 13 Jul 2021 22:52:40 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d52e992561df06f2a88902eb1eae5f59f672d405d214e7e2b6f0385c1638c`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 575.3 KB (575254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf61e6427078809c42793b5f22fd21f92553a46d21fc49d8c56b7943fe4fb2`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f57c93c1bafbca439485a348b5d878cd324adfc4f818da9edb6b8bc5539e32`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f2ee158830adb62106fca0a7dcbf70dabcd078fba1eb71b5b2a19e867dcb6`  
		Last Modified: Tue, 13 Jul 2021 22:53:20 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08860bc426f481ccaa9b5cf7e2b91ad5c9cb5b71f7b3cddcc8d944368922c8cd`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:32cb588b373c3845a9d74d5ddab498f9d98df525709303a177b62fb5d19a694a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226288317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7058c8e16114eba430521762990dc50b33c9f2bbc6ff3f13a23513a981a25843`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:29:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 23:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:30:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:30:08 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 23:30:27 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:28 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 23:30:29 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 23:30:29 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 23:30:33 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 23:30:34 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 23:30:36 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 23:30:36 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:30:36 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 23:30:36 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:30:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b2d40d48563623b5da173028af540053694b83df5a1fa4033dcc46d5d0108f`  
		Last Modified: Tue, 13 Jul 2021 23:31:53 GMT  
		Size: 85.6 MB (85585613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaa3e5d5e3aa193ba5788e79d26cecbb288990bf94e34a0b09f4b1ceb66583`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc45aa8282d969a51cad8f0533fef4323cfad7c72ece492176d04a6331571eb9`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05133f4e2f35fb0b63eec6c0b888d4869ba796b2d817baba42abd64d8af2b951`  
		Last Modified: Tue, 13 Jul 2021 23:31:36 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b57dc4d2d4fdbace1ca3de4ec8f30cec16747b639f63cfc977479803d1988`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982e0e6118afaa6d9a609ccbac3ad25d1357b66b944626f1a1d5807e9ca8fa2f`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e1acb7a095d261a173aa38cf2c4af10431dafa3ced90106095fe88b4d791bb`  
		Last Modified: Tue, 13 Jul 2021 23:32:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd65387ac6e82414900048ffaa5e690250c839a2605b67d830ff2057f99a407`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:6d42098255d7f0cc80c2f0ffb70c5c76e99739651e6aac3c2716d1e8c9ab3bad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233796336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efda9e0b763ba1558488a71d85829892d6d9dcf7a7549ca1cb1052667717c9dc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:23:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jul 2021 04:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:28:27 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:28:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:29:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:29:17 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:32:59 GMT
ARG BRANDING_VERSION
# Wed, 14 Jul 2021 04:33:01 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:33:08 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:33:17 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:33:21 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 14 Jul 2021 04:33:24 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 14 Jul 2021 04:33:39 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 14 Jul 2021 04:33:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:33:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:33:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:34:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 14 Jul 2021 04:34:21 GMT
RUN mkdir /opt/files
# Wed, 14 Jul 2021 04:34:26 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 14 Jul 2021 04:34:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 14 Jul 2021 04:34:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 14 Jul 2021 04:35:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 14 Jul 2021 04:35:08 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:35:11 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 14 Jul 2021 04:35:15 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:35:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6d20994673343d11028ac1ac0bcc098d0f1ac3b04655623d2d2cafa4bee8d`  
		Last Modified: Wed, 14 Jul 2021 04:37:02 GMT  
		Size: 86.4 MB (86395354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a025e3dd302981f640be07c88365b3ddfa8c7d2a818971b050001fa255123`  
		Last Modified: Wed, 14 Jul 2021 04:36:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c867ae2580be2a8356c180288cecbeca16488f530908d5ebb203c0c5bf0a99`  
		Last Modified: Wed, 14 Jul 2021 04:36:44 GMT  
		Size: 1.9 KB (1900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732888c6ddf76b2f60aa2ce9638a1b17b4a33dc96c7a969b6b0a3401b8c8568`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 546.7 KB (546731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01503d0bfb3e8749a1da3e2fe6cbf5e5208d577a78b429c339ba548a3e20f3aa`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91434b0d6bc799538f5ccea05a983777aa3db998cee240f7e841f059c8982d1`  
		Last Modified: Wed, 14 Jul 2021 04:37:16 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ceb99ecfc3b3526d131f1a01116aaaf5821a5a16c59e76ea0e83d14b7c0b5f`  
		Last Modified: Wed, 14 Jul 2021 04:37:26 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b028984ead8def425d58ddd729fc1448e107673994a53e44d976baf1ae7ad0`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:e7b3f12dd62820806337d92a2abb053c8ac4893ec44a8b17c8085ecbb32736ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:ca94d2e7f5bbb0b99ea21f5d28953f5b251429780269ff6b72faba3a1166deee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237176579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c082732516f02e2420afb55f7ea56a975fd95c1d054cd606948e955733b0cb1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:50:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 22:50:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:50:57 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:50:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:51:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:51:01 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 22:51:28 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:30 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 22:51:31 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 22:51:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 22:51:35 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 22:51:37 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 22:51:39 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 22:51:39 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:51:39 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 22:51:40 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:51:40 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8d7f47c4c91b8d9dbce730b796e70940a94024d9deb6fe6c3c7a3c097b837`  
		Last Modified: Tue, 13 Jul 2021 22:53:00 GMT  
		Size: 93.5 MB (93468936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d57029df8192f7fe92beee6610f11707e2b36a3d87f3a4699dbba6fe558a61`  
		Last Modified: Tue, 13 Jul 2021 22:52:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24804a7ca337850329a0363fbc58cdaef060aa67650f7f5826b22714b45eb32b`  
		Last Modified: Tue, 13 Jul 2021 22:52:40 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d52e992561df06f2a88902eb1eae5f59f672d405d214e7e2b6f0385c1638c`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 575.3 KB (575254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf61e6427078809c42793b5f22fd21f92553a46d21fc49d8c56b7943fe4fb2`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f57c93c1bafbca439485a348b5d878cd324adfc4f818da9edb6b8bc5539e32`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f2ee158830adb62106fca0a7dcbf70dabcd078fba1eb71b5b2a19e867dcb6`  
		Last Modified: Tue, 13 Jul 2021 22:53:20 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08860bc426f481ccaa9b5cf7e2b91ad5c9cb5b71f7b3cddcc8d944368922c8cd`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:32cb588b373c3845a9d74d5ddab498f9d98df525709303a177b62fb5d19a694a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226288317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7058c8e16114eba430521762990dc50b33c9f2bbc6ff3f13a23513a981a25843`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:29:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 23:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:30:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:30:08 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 23:30:27 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:28 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 23:30:29 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 23:30:29 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 23:30:33 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 23:30:34 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 23:30:36 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 23:30:36 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:30:36 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 23:30:36 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:30:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b2d40d48563623b5da173028af540053694b83df5a1fa4033dcc46d5d0108f`  
		Last Modified: Tue, 13 Jul 2021 23:31:53 GMT  
		Size: 85.6 MB (85585613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaa3e5d5e3aa193ba5788e79d26cecbb288990bf94e34a0b09f4b1ceb66583`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc45aa8282d969a51cad8f0533fef4323cfad7c72ece492176d04a6331571eb9`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05133f4e2f35fb0b63eec6c0b888d4869ba796b2d817baba42abd64d8af2b951`  
		Last Modified: Tue, 13 Jul 2021 23:31:36 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b57dc4d2d4fdbace1ca3de4ec8f30cec16747b639f63cfc977479803d1988`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982e0e6118afaa6d9a609ccbac3ad25d1357b66b944626f1a1d5807e9ca8fa2f`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e1acb7a095d261a173aa38cf2c4af10431dafa3ced90106095fe88b4d791bb`  
		Last Modified: Tue, 13 Jul 2021 23:32:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd65387ac6e82414900048ffaa5e690250c839a2605b67d830ff2057f99a407`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:6d42098255d7f0cc80c2f0ffb70c5c76e99739651e6aac3c2716d1e8c9ab3bad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233796336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efda9e0b763ba1558488a71d85829892d6d9dcf7a7549ca1cb1052667717c9dc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:23:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jul 2021 04:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:28:27 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:28:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:29:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:29:17 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:32:59 GMT
ARG BRANDING_VERSION
# Wed, 14 Jul 2021 04:33:01 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:33:08 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:33:17 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:33:21 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 14 Jul 2021 04:33:24 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 14 Jul 2021 04:33:39 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 14 Jul 2021 04:33:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:33:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:33:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:34:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 14 Jul 2021 04:34:21 GMT
RUN mkdir /opt/files
# Wed, 14 Jul 2021 04:34:26 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 14 Jul 2021 04:34:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 14 Jul 2021 04:34:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 14 Jul 2021 04:35:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 14 Jul 2021 04:35:08 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:35:11 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 14 Jul 2021 04:35:15 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:35:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6d20994673343d11028ac1ac0bcc098d0f1ac3b04655623d2d2cafa4bee8d`  
		Last Modified: Wed, 14 Jul 2021 04:37:02 GMT  
		Size: 86.4 MB (86395354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a025e3dd302981f640be07c88365b3ddfa8c7d2a818971b050001fa255123`  
		Last Modified: Wed, 14 Jul 2021 04:36:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c867ae2580be2a8356c180288cecbeca16488f530908d5ebb203c0c5bf0a99`  
		Last Modified: Wed, 14 Jul 2021 04:36:44 GMT  
		Size: 1.9 KB (1900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732888c6ddf76b2f60aa2ce9638a1b17b4a33dc96c7a969b6b0a3401b8c8568`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 546.7 KB (546731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01503d0bfb3e8749a1da3e2fe6cbf5e5208d577a78b429c339ba548a3e20f3aa`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91434b0d6bc799538f5ccea05a983777aa3db998cee240f7e841f059c8982d1`  
		Last Modified: Wed, 14 Jul 2021 04:37:16 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ceb99ecfc3b3526d131f1a01116aaaf5821a5a16c59e76ea0e83d14b7c0b5f`  
		Last Modified: Wed, 14 Jul 2021 04:37:26 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b028984ead8def425d58ddd729fc1448e107673994a53e44d976baf1ae7ad0`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:e7b3f12dd62820806337d92a2abb053c8ac4893ec44a8b17c8085ecbb32736ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:ca94d2e7f5bbb0b99ea21f5d28953f5b251429780269ff6b72faba3a1166deee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237176579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c082732516f02e2420afb55f7ea56a975fd95c1d054cd606948e955733b0cb1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:50:16 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 22:50:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:50:57 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 22:50:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 22:51:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 22:51:01 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 22:51:27 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 22:51:28 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 22:51:28 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 22:51:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 22:51:30 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 22:51:31 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 22:51:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 22:51:35 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 22:51:37 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 22:51:39 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 22:51:39 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 22:51:39 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 22:51:40 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 22:51:40 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8d7f47c4c91b8d9dbce730b796e70940a94024d9deb6fe6c3c7a3c097b837`  
		Last Modified: Tue, 13 Jul 2021 22:53:00 GMT  
		Size: 93.5 MB (93468936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d57029df8192f7fe92beee6610f11707e2b36a3d87f3a4699dbba6fe558a61`  
		Last Modified: Tue, 13 Jul 2021 22:52:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24804a7ca337850329a0363fbc58cdaef060aa67650f7f5826b22714b45eb32b`  
		Last Modified: Tue, 13 Jul 2021 22:52:40 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d52e992561df06f2a88902eb1eae5f59f672d405d214e7e2b6f0385c1638c`  
		Last Modified: Tue, 13 Jul 2021 22:52:38 GMT  
		Size: 575.3 KB (575254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf61e6427078809c42793b5f22fd21f92553a46d21fc49d8c56b7943fe4fb2`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f57c93c1bafbca439485a348b5d878cd324adfc4f818da9edb6b8bc5539e32`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f2ee158830adb62106fca0a7dcbf70dabcd078fba1eb71b5b2a19e867dcb6`  
		Last Modified: Tue, 13 Jul 2021 22:53:20 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08860bc426f481ccaa9b5cf7e2b91ad5c9cb5b71f7b3cddcc8d944368922c8cd`  
		Last Modified: Tue, 13 Jul 2021 22:53:12 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:32cb588b373c3845a9d74d5ddab498f9d98df525709303a177b62fb5d19a694a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226288317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7058c8e16114eba430521762990dc50b33c9f2bbc6ff3f13a23513a981a25843`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:29:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Tue, 13 Jul 2021 23:30:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:30:04 GMT
RUN mkdir /opt/custom-init.d/
# Tue, 13 Jul 2021 23:30:05 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Tue, 13 Jul 2021 23:30:08 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Tue, 13 Jul 2021 23:30:08 GMT
ARG BONITA_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BRANDING_VERSION
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BONITA_SHA256
# Tue, 13 Jul 2021 23:30:25 GMT
ARG BASE_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ARG BONITA_URL
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_VERSION=7.12.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BRANDING_VERSION=2021.1
# Tue, 13 Jul 2021 23:30:26 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Tue, 13 Jul 2021 23:30:27 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 13 Jul 2021 23:30:27 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Tue, 13 Jul 2021 23:30:28 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 13 Jul 2021 23:30:29 GMT
RUN mkdir /opt/files
# Tue, 13 Jul 2021 23:30:29 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Tue, 13 Jul 2021 23:30:33 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Tue, 13 Jul 2021 23:30:34 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 13 Jul 2021 23:30:36 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 13 Jul 2021 23:30:36 GMT
VOLUME [/opt/bonita]
# Tue, 13 Jul 2021 23:30:36 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 13 Jul 2021 23:30:36 GMT
EXPOSE 8080
# Tue, 13 Jul 2021 23:30:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b2d40d48563623b5da173028af540053694b83df5a1fa4033dcc46d5d0108f`  
		Last Modified: Tue, 13 Jul 2021 23:31:53 GMT  
		Size: 85.6 MB (85585613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaa3e5d5e3aa193ba5788e79d26cecbb288990bf94e34a0b09f4b1ceb66583`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc45aa8282d969a51cad8f0533fef4323cfad7c72ece492176d04a6331571eb9`  
		Last Modified: Tue, 13 Jul 2021 23:31:38 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05133f4e2f35fb0b63eec6c0b888d4869ba796b2d817baba42abd64d8af2b951`  
		Last Modified: Tue, 13 Jul 2021 23:31:36 GMT  
		Size: 547.0 KB (546951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6b57dc4d2d4fdbace1ca3de4ec8f30cec16747b639f63cfc977479803d1988`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982e0e6118afaa6d9a609ccbac3ad25d1357b66b944626f1a1d5807e9ca8fa2f`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e1acb7a095d261a173aa38cf2c4af10431dafa3ced90106095fe88b4d791bb`  
		Last Modified: Tue, 13 Jul 2021 23:32:12 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd65387ac6e82414900048ffaa5e690250c839a2605b67d830ff2057f99a407`  
		Last Modified: Tue, 13 Jul 2021 23:32:05 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:6d42098255d7f0cc80c2f0ffb70c5c76e99739651e6aac3c2716d1e8c9ab3bad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233796336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efda9e0b763ba1558488a71d85829892d6d9dcf7a7549ca1cb1052667717c9dc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:23:21 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 14 Jul 2021 04:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:28:27 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 14 Jul 2021 04:28:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 14 Jul 2021 04:29:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 14 Jul 2021 04:29:17 GMT
ARG BONITA_VERSION
# Wed, 14 Jul 2021 04:32:59 GMT
ARG BRANDING_VERSION
# Wed, 14 Jul 2021 04:33:01 GMT
ARG BONITA_SHA256
# Wed, 14 Jul 2021 04:33:08 GMT
ARG BASE_URL
# Wed, 14 Jul 2021 04:33:17 GMT
ARG BONITA_URL
# Wed, 14 Jul 2021 04:33:21 GMT
ENV BONITA_VERSION=7.12.1
# Wed, 14 Jul 2021 04:33:24 GMT
ENV BRANDING_VERSION=2021.1
# Wed, 14 Jul 2021 04:33:39 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Wed, 14 Jul 2021 04:33:45 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:33:52 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 14 Jul 2021 04:33:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Wed, 14 Jul 2021 04:34:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 14 Jul 2021 04:34:21 GMT
RUN mkdir /opt/files
# Wed, 14 Jul 2021 04:34:26 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Wed, 14 Jul 2021 04:34:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Wed, 14 Jul 2021 04:34:56 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 14 Jul 2021 04:35:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 14 Jul 2021 04:35:08 GMT
VOLUME [/opt/bonita]
# Wed, 14 Jul 2021 04:35:11 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 14 Jul 2021 04:35:15 GMT
EXPOSE 8080
# Wed, 14 Jul 2021 04:35:21 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6d20994673343d11028ac1ac0bcc098d0f1ac3b04655623d2d2cafa4bee8d`  
		Last Modified: Wed, 14 Jul 2021 04:37:02 GMT  
		Size: 86.4 MB (86395354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a025e3dd302981f640be07c88365b3ddfa8c7d2a818971b050001fa255123`  
		Last Modified: Wed, 14 Jul 2021 04:36:46 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c867ae2580be2a8356c180288cecbeca16488f530908d5ebb203c0c5bf0a99`  
		Last Modified: Wed, 14 Jul 2021 04:36:44 GMT  
		Size: 1.9 KB (1900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732888c6ddf76b2f60aa2ce9638a1b17b4a33dc96c7a969b6b0a3401b8c8568`  
		Last Modified: Wed, 14 Jul 2021 04:36:41 GMT  
		Size: 546.7 KB (546731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01503d0bfb3e8749a1da3e2fe6cbf5e5208d577a78b429c339ba548a3e20f3aa`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91434b0d6bc799538f5ccea05a983777aa3db998cee240f7e841f059c8982d1`  
		Last Modified: Wed, 14 Jul 2021 04:37:16 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ceb99ecfc3b3526d131f1a01116aaaf5821a5a16c59e76ea0e83d14b7c0b5f`  
		Last Modified: Wed, 14 Jul 2021 04:37:26 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b028984ead8def425d58ddd729fc1448e107673994a53e44d976baf1ae7ad0`  
		Last Modified: Wed, 14 Jul 2021 04:37:15 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
