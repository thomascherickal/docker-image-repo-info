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
$ docker pull bonita@sha256:a0160dd5fea19184ebd54faf3eadf2cba823a05d2f928fc756b0fcfd407534d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:153bd4671f7ad09ee2716016ee8ad3d43694423122ebaa4c12a2cd6549671ae7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233788879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:804c0871b0cb80fb64ffcd30d8be5a38f225dda3cd2522cbc11fb907beb8b7bc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:21:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 02:26:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:26:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:26:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:26:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:26:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:29:20 GMT
ARG BRANDING_VERSION
# Fri, 18 Jun 2021 02:29:24 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:29:27 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:29:33 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:29:37 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 18 Jun 2021 02:29:43 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 18 Jun 2021 02:29:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 18 Jun 2021 02:29:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:29:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:30:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:30:07 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 02:30:16 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 02:30:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 18 Jun 2021 02:30:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 18 Jun 2021 02:30:44 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 02:30:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 02:30:55 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:30:57 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 02:31:00 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:31:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c113c1ae7dc0dc313c204f9ea9d49012a00e73130cca1db6d19ff3ece5ff2e1f`  
		Last Modified: Fri, 18 Jun 2021 02:32:16 GMT  
		Size: 86.4 MB (86395400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d984d51010082df8d61be12d8020b2d44f690e07fb07b9a9b9630ee86ebf4c5`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411376b8dfae1e17abca2b5147246aeedc03374283b137c7bccec6324e95ff89`  
		Last Modified: Fri, 18 Jun 2021 02:32:00 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212579edc8cb831f0bb8e60071b4de21345dc08bea4efca91980f86ee8a11dc2`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 541.9 KB (541862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa19053e375465e65088596f3b21a5bbd55d803e7aaa0561d9344a82720350e`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1516cbee7ebb6721e42ee2d2b4c65fc7dbfd24f4f5c4125f6710842e209717`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914bd3d46ee1158c57fd7f2367ed8e728a3789fab081c0346a59c1b07ce9092`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515bf202b48d0ae2be88189c04ca348be78331dc29469edecd1fa67c434da3c`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10`

```console
$ docker pull bonita@sha256:78f038eefcbef709a54be2ef1100f84a06293cd7058372a16a2d20b39d025ba9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:8a3287b2469f69ebbcdce9e5426a82be3835a9bb4d88d4e0c8c14f165d2be292
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240263855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302554f23430596b5324c17dbef33edc133a34a60f266d5e363897fe033c4b67`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:09:19 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 18 Jun 2021 02:17:42 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:04 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:18:24 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:18:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:18:45 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:18:52 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:18:59 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:19:12 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:19:18 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 18 Jun 2021 02:19:27 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 18 Jun 2021 02:19:36 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:19:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 18 Jun 2021 02:20:04 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 18 Jun 2021 02:20:22 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 02:20:37 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 02:20:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 18 Jun 2021 02:20:55 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:20:59 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 18 Jun 2021 02:21:01 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 18 Jun 2021 02:21:12 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:21:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a1bc3198fa2c8f13d7918a57de27a3e5868287d63fc6e20e38bf402882c25e`  
		Last Modified: Fri, 18 Jun 2021 02:31:45 GMT  
		Size: 111.3 MB (111311288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5911aa1c02a1c34479532f8f41b572e12bcf853e4f137a0c54c80f6ff9a5e873`  
		Last Modified: Fri, 18 Jun 2021 02:31:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0686fbc9c641341de82871906bd9aa2caae8ea9b2b0ee99bb6df16c88ba2ac55`  
		Last Modified: Fri, 18 Jun 2021 02:31:22 GMT  
		Size: 1.9 KB (1923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda45ff3056f8d24d069c4b06913fe229a180a9c2e8a1241e7517e2900df0b40`  
		Last Modified: Fri, 18 Jun 2021 02:31:23 GMT  
		Size: 541.9 KB (541865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b9a6fe8235330d6f3178558c3484d24b7f82b1ca6fbb64a24b0da038890661`  
		Last Modified: Fri, 18 Jun 2021 02:31:31 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c3fc659dfb0232cf2ba8e7de6e6bc4918b59fd091ac3a318b5217f7622a1f`  
		Last Modified: Fri, 18 Jun 2021 02:31:22 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33e53fada89b44854349e1ad0fc01fd2d4567af20a3e3d3342bd7ca6d3164d5`  
		Last Modified: Fri, 18 Jun 2021 02:31:22 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:78f038eefcbef709a54be2ef1100f84a06293cd7058372a16a2d20b39d025ba9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:8a3287b2469f69ebbcdce9e5426a82be3835a9bb4d88d4e0c8c14f165d2be292
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240263855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302554f23430596b5324c17dbef33edc133a34a60f266d5e363897fe033c4b67`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:09:19 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 18 Jun 2021 02:17:42 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:18:04 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:18:24 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:18:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:18:45 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:18:52 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:18:59 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:19:12 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:19:18 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 18 Jun 2021 02:19:27 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 18 Jun 2021 02:19:36 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:19:47 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 18 Jun 2021 02:20:04 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 18 Jun 2021 02:20:22 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 02:20:37 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 02:20:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 18 Jun 2021 02:20:55 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:20:59 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 18 Jun 2021 02:21:01 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 18 Jun 2021 02:21:12 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:21:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a1bc3198fa2c8f13d7918a57de27a3e5868287d63fc6e20e38bf402882c25e`  
		Last Modified: Fri, 18 Jun 2021 02:31:45 GMT  
		Size: 111.3 MB (111311288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5911aa1c02a1c34479532f8f41b572e12bcf853e4f137a0c54c80f6ff9a5e873`  
		Last Modified: Fri, 18 Jun 2021 02:31:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0686fbc9c641341de82871906bd9aa2caae8ea9b2b0ee99bb6df16c88ba2ac55`  
		Last Modified: Fri, 18 Jun 2021 02:31:22 GMT  
		Size: 1.9 KB (1923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda45ff3056f8d24d069c4b06913fe229a180a9c2e8a1241e7517e2900df0b40`  
		Last Modified: Fri, 18 Jun 2021 02:31:23 GMT  
		Size: 541.9 KB (541865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b9a6fe8235330d6f3178558c3484d24b7f82b1ca6fbb64a24b0da038890661`  
		Last Modified: Fri, 18 Jun 2021 02:31:31 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c3fc659dfb0232cf2ba8e7de6e6bc4918b59fd091ac3a318b5217f7622a1f`  
		Last Modified: Fri, 18 Jun 2021 02:31:22 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33e53fada89b44854349e1ad0fc01fd2d4567af20a3e3d3342bd7ca6d3164d5`  
		Last Modified: Fri, 18 Jun 2021 02:31:22 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:507e1035cc29e1bdcd8e78449776cffaab2e75a92f438e6e621046f27ca23445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:e4ebdb5a2a0e356dd252923af9fa35c900c7ef8a1fba5a20c303eedcce1a3b0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230721245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d54967ebb0c47f4b1439fb06fc6a3a42fee866eb48486447a970acdd454d50`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:21:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 02:26:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:26:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:26:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:26:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:26:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:27:06 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:27:12 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:27:21 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:27:26 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 18 Jun 2021 02:27:31 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 18 Jun 2021 02:27:34 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 02:27:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:27:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 02:27:49 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 02:28:00 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 02:28:01 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 18 Jun 2021 02:28:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 18 Jun 2021 02:28:25 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 02:28:35 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 02:28:40 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:28:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 02:28:51 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:28:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c113c1ae7dc0dc313c204f9ea9d49012a00e73130cca1db6d19ff3ece5ff2e1f`  
		Last Modified: Fri, 18 Jun 2021 02:32:16 GMT  
		Size: 86.4 MB (86395400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d984d51010082df8d61be12d8020b2d44f690e07fb07b9a9b9630ee86ebf4c5`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411376b8dfae1e17abca2b5147246aeedc03374283b137c7bccec6324e95ff89`  
		Last Modified: Fri, 18 Jun 2021 02:32:00 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212579edc8cb831f0bb8e60071b4de21345dc08bea4efca91980f86ee8a11dc2`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 541.9 KB (541862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e6f4356691caf534ddd7670726a9fb628742b3804b2aee68dcb1ed3094b789`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77471469cf0854950d8d1899ced5c6e136404a8a994d6c47956765d88cf9d5c`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209e790cdaf4e8c552004915d72a84eafcd8d6b6ee49458edc2647733f8ebb9b`  
		Last Modified: Fri, 18 Jun 2021 02:32:05 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74eb41f442418505739c3d736ce91f06b094e442f9da2d76b8b25c50b555c5`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:507e1035cc29e1bdcd8e78449776cffaab2e75a92f438e6e621046f27ca23445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:e4ebdb5a2a0e356dd252923af9fa35c900c7ef8a1fba5a20c303eedcce1a3b0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230721245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d54967ebb0c47f4b1439fb06fc6a3a42fee866eb48486447a970acdd454d50`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:21:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 02:26:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:26:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:26:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:26:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:26:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:27:06 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:27:12 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:27:21 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:27:26 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 18 Jun 2021 02:27:31 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 18 Jun 2021 02:27:34 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 02:27:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:27:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 02:27:49 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 02:28:00 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 02:28:01 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 18 Jun 2021 02:28:14 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 18 Jun 2021 02:28:25 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 02:28:35 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 02:28:40 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:28:43 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 02:28:51 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:28:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c113c1ae7dc0dc313c204f9ea9d49012a00e73130cca1db6d19ff3ece5ff2e1f`  
		Last Modified: Fri, 18 Jun 2021 02:32:16 GMT  
		Size: 86.4 MB (86395400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d984d51010082df8d61be12d8020b2d44f690e07fb07b9a9b9630ee86ebf4c5`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411376b8dfae1e17abca2b5147246aeedc03374283b137c7bccec6324e95ff89`  
		Last Modified: Fri, 18 Jun 2021 02:32:00 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212579edc8cb831f0bb8e60071b4de21345dc08bea4efca91980f86ee8a11dc2`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 541.9 KB (541862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e6f4356691caf534ddd7670726a9fb628742b3804b2aee68dcb1ed3094b789`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77471469cf0854950d8d1899ced5c6e136404a8a994d6c47956765d88cf9d5c`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209e790cdaf4e8c552004915d72a84eafcd8d6b6ee49458edc2647733f8ebb9b`  
		Last Modified: Fri, 18 Jun 2021 02:32:05 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d74eb41f442418505739c3d736ce91f06b094e442f9da2d76b8b25c50b555c5`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:a0160dd5fea19184ebd54faf3eadf2cba823a05d2f928fc756b0fcfd407534d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:153bd4671f7ad09ee2716016ee8ad3d43694423122ebaa4c12a2cd6549671ae7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233788879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:804c0871b0cb80fb64ffcd30d8be5a38f225dda3cd2522cbc11fb907beb8b7bc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:21:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 02:26:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:26:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:26:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:26:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:26:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:29:20 GMT
ARG BRANDING_VERSION
# Fri, 18 Jun 2021 02:29:24 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:29:27 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:29:33 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:29:37 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 18 Jun 2021 02:29:43 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 18 Jun 2021 02:29:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 18 Jun 2021 02:29:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:29:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:30:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:30:07 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 02:30:16 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 02:30:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 18 Jun 2021 02:30:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 18 Jun 2021 02:30:44 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 02:30:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 02:30:55 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:30:57 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 02:31:00 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:31:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c113c1ae7dc0dc313c204f9ea9d49012a00e73130cca1db6d19ff3ece5ff2e1f`  
		Last Modified: Fri, 18 Jun 2021 02:32:16 GMT  
		Size: 86.4 MB (86395400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d984d51010082df8d61be12d8020b2d44f690e07fb07b9a9b9630ee86ebf4c5`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411376b8dfae1e17abca2b5147246aeedc03374283b137c7bccec6324e95ff89`  
		Last Modified: Fri, 18 Jun 2021 02:32:00 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212579edc8cb831f0bb8e60071b4de21345dc08bea4efca91980f86ee8a11dc2`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 541.9 KB (541862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa19053e375465e65088596f3b21a5bbd55d803e7aaa0561d9344a82720350e`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1516cbee7ebb6721e42ee2d2b4c65fc7dbfd24f4f5c4125f6710842e209717`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914bd3d46ee1158c57fd7f2367ed8e728a3789fab081c0346a59c1b07ce9092`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515bf202b48d0ae2be88189c04ca348be78331dc29469edecd1fa67c434da3c`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:a0160dd5fea19184ebd54faf3eadf2cba823a05d2f928fc756b0fcfd407534d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:153bd4671f7ad09ee2716016ee8ad3d43694423122ebaa4c12a2cd6549671ae7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233788879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:804c0871b0cb80fb64ffcd30d8be5a38f225dda3cd2522cbc11fb907beb8b7bc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:21:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 02:26:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:26:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:26:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:26:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:26:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:29:20 GMT
ARG BRANDING_VERSION
# Fri, 18 Jun 2021 02:29:24 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:29:27 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:29:33 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:29:37 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 18 Jun 2021 02:29:43 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 18 Jun 2021 02:29:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 18 Jun 2021 02:29:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:29:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:30:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:30:07 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 02:30:16 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 02:30:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 18 Jun 2021 02:30:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 18 Jun 2021 02:30:44 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 02:30:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 02:30:55 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:30:57 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 02:31:00 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:31:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c113c1ae7dc0dc313c204f9ea9d49012a00e73130cca1db6d19ff3ece5ff2e1f`  
		Last Modified: Fri, 18 Jun 2021 02:32:16 GMT  
		Size: 86.4 MB (86395400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d984d51010082df8d61be12d8020b2d44f690e07fb07b9a9b9630ee86ebf4c5`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411376b8dfae1e17abca2b5147246aeedc03374283b137c7bccec6324e95ff89`  
		Last Modified: Fri, 18 Jun 2021 02:32:00 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212579edc8cb831f0bb8e60071b4de21345dc08bea4efca91980f86ee8a11dc2`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 541.9 KB (541862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa19053e375465e65088596f3b21a5bbd55d803e7aaa0561d9344a82720350e`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1516cbee7ebb6721e42ee2d2b4c65fc7dbfd24f4f5c4125f6710842e209717`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914bd3d46ee1158c57fd7f2367ed8e728a3789fab081c0346a59c1b07ce9092`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515bf202b48d0ae2be88189c04ca348be78331dc29469edecd1fa67c434da3c`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:a0160dd5fea19184ebd54faf3eadf2cba823a05d2f928fc756b0fcfd407534d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull bonita@sha256:153bd4671f7ad09ee2716016ee8ad3d43694423122ebaa4c12a2cd6549671ae7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233788879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:804c0871b0cb80fb64ffcd30d8be5a38f225dda3cd2522cbc11fb907beb8b7bc`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:21:38 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 02:26:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:26:30 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 02:26:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 02:26:53 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 02:26:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 02:29:20 GMT
ARG BRANDING_VERSION
# Fri, 18 Jun 2021 02:29:24 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 02:29:27 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 02:29:33 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 02:29:37 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 18 Jun 2021 02:29:43 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 18 Jun 2021 02:29:48 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 18 Jun 2021 02:29:52 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:29:56 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 02:30:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 02:30:07 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 02:30:16 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 02:30:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 18 Jun 2021 02:30:32 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 18 Jun 2021 02:30:44 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 02:30:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 02:30:55 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 02:30:57 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 02:31:00 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 02:31:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c113c1ae7dc0dc313c204f9ea9d49012a00e73130cca1db6d19ff3ece5ff2e1f`  
		Last Modified: Fri, 18 Jun 2021 02:32:16 GMT  
		Size: 86.4 MB (86395400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d984d51010082df8d61be12d8020b2d44f690e07fb07b9a9b9630ee86ebf4c5`  
		Last Modified: Fri, 18 Jun 2021 02:32:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411376b8dfae1e17abca2b5147246aeedc03374283b137c7bccec6324e95ff89`  
		Last Modified: Fri, 18 Jun 2021 02:32:00 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212579edc8cb831f0bb8e60071b4de21345dc08bea4efca91980f86ee8a11dc2`  
		Last Modified: Fri, 18 Jun 2021 02:31:57 GMT  
		Size: 541.9 KB (541862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa19053e375465e65088596f3b21a5bbd55d803e7aaa0561d9344a82720350e`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1516cbee7ebb6721e42ee2d2b4c65fc7dbfd24f4f5c4125f6710842e209717`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914bd3d46ee1158c57fd7f2367ed8e728a3789fab081c0346a59c1b07ce9092`  
		Last Modified: Fri, 18 Jun 2021 02:32:36 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515bf202b48d0ae2be88189c04ca348be78331dc29469edecd1fa67c434da3c`  
		Last Modified: Fri, 18 Jun 2021 02:32:27 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
