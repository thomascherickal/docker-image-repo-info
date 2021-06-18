## `bonita:latest`

```console
$ docker pull bonita@sha256:9da696d8aa2a9206d0a9d98b862f8e796e07e44499088dd3a5ac6ed498536a12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:b84f85958a390b40b86763330c13d14d6359e22e2a3f3dd077c0bad762f48f9f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237169652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927c1dca82056d44db24e5ea8dce2274c231fdb3ee72640ab854a4747e737414`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:26:10 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 00:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:26:31 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 00:26:33 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 00:26:34 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 00:26:34 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 00:26:53 GMT
ARG BRANDING_VERSION
# Fri, 18 Jun 2021 00:26:53 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:26:54 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:26:54 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:26:54 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 18 Jun 2021 00:26:54 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 18 Jun 2021 00:26:54 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 18 Jun 2021 00:26:54 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 00:26:55 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:26:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 00:26:56 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 00:26:57 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 00:26:57 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 18 Jun 2021 00:27:00 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 18 Jun 2021 00:27:02 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 00:27:04 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 00:27:04 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:27:04 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 00:27:04 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:27:05 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee33f33e64d6aecd191d0e19accaf72783eab69bb9c93675455ff90891f83aa`  
		Last Modified: Fri, 18 Jun 2021 00:28:06 GMT  
		Size: 93.5 MB (93469706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1700a806c2418982c14db3308e332f83535885a5b041a47f7158da1bcd282`  
		Last Modified: Fri, 18 Jun 2021 00:27:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b941f53dc54d5f28dfcd18491129c3fb5d11abf4e56a53788fd872819fa40e`  
		Last Modified: Fri, 18 Jun 2021 00:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb14a90f0796d753c92edecde3c91fe96826bb35b5d22b869f94cf1dc67da014`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 573.0 KB (572994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df854c4d08cd1cbdd2f0f1ec489a64a60cbf002d3ded062c7e079800c8b2076`  
		Last Modified: Fri, 18 Jun 2021 00:28:16 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b190403a4ee0d0ef36529d617cf9974d25ba127ae69f42b5c2be8bc4fed0d9b`  
		Last Modified: Fri, 18 Jun 2021 00:28:16 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd2dbdcd060ce35b33a842b7e880780b619e40ad4a98260bb8d273592ebe786`  
		Last Modified: Fri, 18 Jun 2021 00:28:21 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9154588d5e2b8dfebab76cb2b6e9d6cc3a161fe817fdaefb6d4dbcc469f32e68`  
		Last Modified: Fri, 18 Jun 2021 00:28:16 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:1998085f48b5712ba5913d24e300f4e032f478d927ef6802f6ca9e2f8d3c79d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226282482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b245548d1f8560771ee1f036fd338d47e7fac71e82a1155afe05ddede2ff57d4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:28:19 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 18 Jun 2021 00:28:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:28:40 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 00:28:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 00:28:43 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 00:28:57 GMT
ARG BRANDING_VERSION
# Fri, 18 Jun 2021 00:28:57 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:28:57 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:28:58 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:28:58 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 18 Jun 2021 00:28:58 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 18 Jun 2021 00:28:58 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 18 Jun 2021 00:28:58 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 00:28:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:28:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 18 Jun 2021 00:28:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 00:29:00 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 00:29:01 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 18 Jun 2021 00:29:08 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 18 Jun 2021 00:29:10 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 00:29:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 00:29:11 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:29:11 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 00:29:12 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:29:12 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecf3189c00b0df3c00fa8bec7f3b427f05f8436fc3c9c777ec7592b4d6eb95`  
		Last Modified: Fri, 18 Jun 2021 00:30:28 GMT  
		Size: 85.6 MB (85585595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d8d044502233c64ae3114a1608b45b060356ec8d3202ffd5a02fac4915cb58`  
		Last Modified: Fri, 18 Jun 2021 00:30:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa02bf96b8f043e24d601e8ac4ca84333f6764a7649c36d4c9ad3da6eb16a57`  
		Last Modified: Fri, 18 Jun 2021 00:30:15 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1529d15e96c0ce029500274a840c3e559c0ab7d9f7563dff1ee53d131cd25276`  
		Last Modified: Fri, 18 Jun 2021 00:30:13 GMT  
		Size: 542.5 KB (542475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1e9bd0a001e0b5486af21fcc2f66444523646dfd6facc7113fda6765257887`  
		Last Modified: Fri, 18 Jun 2021 00:30:40 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4fb36b6489833dd7be22b4d933c07dbbe9fcfc9f3ac0e2d82a625cb2aa8f22`  
		Last Modified: Fri, 18 Jun 2021 00:30:40 GMT  
		Size: 6.9 KB (6942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d794ee6fb9904381a36d79e6556a5e05db5a30c82962c3ee448f47d0cb8a32e`  
		Last Modified: Fri, 18 Jun 2021 00:30:47 GMT  
		Size: 116.4 MB (116415403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79147da439f82dd50a734e1f0ad8a67d59f5bc36735e22c3aefa22de907a8a07`  
		Last Modified: Fri, 18 Jun 2021 00:30:40 GMT  
		Size: 1.7 KB (1707 bytes)  
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
