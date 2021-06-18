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
$ docker pull bonita@sha256:0053ea88b38c83e55d49f544b180559b83214bdf1761e8cf6605a587280962a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

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

### `bonita:2021.1` - linux; arm64 variant v8

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

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:09da2c521e70bac97002559c1ffe9aa27945133ad024f1b4dcaf09045d8fa1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233771062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec61d43b322fa845c74b454e498eacf30dfe3dc8c8f6ffe8ea879a1a9f20788d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:34:50 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 20 May 2021 00:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:39:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:39:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:39:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:39:46 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:43:33 GMT
ARG BRANDING_VERSION
# Thu, 20 May 2021 00:43:41 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:43:47 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:43:58 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:44:06 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 20 May 2021 00:44:12 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 20 May 2021 00:44:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 20 May 2021 00:44:21 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:44:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:40 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 20 May 2021 00:44:51 GMT
RUN mkdir /opt/files
# Thu, 20 May 2021 00:44:56 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 20 May 2021 00:45:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 20 May 2021 00:45:39 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 20 May 2021 00:45:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 20 May 2021 00:46:05 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:46:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 20 May 2021 00:46:14 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:46:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9e7ad0f0448e92fb16f76c603aecada15c40889d4f1da5923250604fdc460`  
		Last Modified: Thu, 20 May 2021 00:47:47 GMT  
		Size: 86.4 MB (86394726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ff6f34104a98707426da1f362155f111ef7bd4f46193af555901fbe011772b`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd99b523b212592de5647eedf6cad7470492839cbd8cb25bd386a5808114`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56876c96ca39f94c870355914abeb3d9caf5d6f3ccee59ca9329a11528645`  
		Last Modified: Thu, 20 May 2021 00:47:28 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ebc9951f8a6e042d6aa4d540a3c257fdc84113e4220e55017795b2f7ab3f2b`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e36ed62d5e55e1a0a7ee290d0eee7d9eebadfa7ed944102b57bbb72a0dd572`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b015e0aea1f89925140ec99156b48900b70ecd46a6fe170c7e58634db6db82d`  
		Last Modified: Thu, 20 May 2021 00:48:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b54f55048bca738773475353787939d3fec3a7e0b9f77c543fe7b5cf2aead1f`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10`

```console
$ docker pull bonita@sha256:0ec6db4854c1febd69239d83ac4642e88cb82301f2e94a237fc8a9d7ecbb90e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:35935305b4731cf7bf17388d25216aeb324cc072e694c58f70abcbda537c6454
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242287750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3a38362ab8ae89504f85daa31e91679ec8c876299299fabf8f33ed5e651b78a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:24:15 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 18 Jun 2021 00:25:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:25:42 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 00:25:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 00:25:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 00:25:45 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 00:25:45 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:25:45 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:25:46 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 18 Jun 2021 00:25:47 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 18 Jun 2021 00:25:51 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:25:52 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:25:54 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 18 Jun 2021 00:25:54 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:25:54 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 18 Jun 2021 00:25:54 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 18 Jun 2021 00:25:54 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:25:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5cf33d8a997d9835e64c3f23a107dec928b238d89f74285e02f346b500ad9d`  
		Last Modified: Fri, 18 Jun 2021 00:27:40 GMT  
		Size: 117.0 MB (117028710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f19eb1419d028bd24a0811d06056297eaad1d2e93ab40e819d6127c72b216`  
		Last Modified: Fri, 18 Jun 2021 00:27:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ba5073c63c4c7355d7949aaa99c6b7d620348380a9909f8f79eda73f3f000f`  
		Last Modified: Fri, 18 Jun 2021 00:27:21 GMT  
		Size: 1.9 KB (1908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6a4bcb4a547bc5007dd2e5167a9f1c992abb5e195efec9d725c1d4d1091e0e`  
		Last Modified: Fri, 18 Jun 2021 00:27:22 GMT  
		Size: 573.0 KB (573007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289a8ce473e558dc7cd99b4cbff9432e7be810e40b9c8017dc3d024a8f53864`  
		Last Modified: Fri, 18 Jun 2021 00:27:26 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e33b79f79b4a846ec471205478dbb72d958b803a53495e27afad6623a2ad7`  
		Last Modified: Fri, 18 Jun 2021 00:27:21 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7684f55978eb4019a36876b9fcd35472055db059ffc17322e7ba9d14bbcff8d`  
		Last Modified: Fri, 18 Jun 2021 00:27:21 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:0fd6a21415cb3f35adfc738e2395f83295d8df16b423fcf2a39a074bebd9d419
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230989530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d44292c71e22fe95cd176de65d21cf33de7c70e355bf18dc0a8b70bcbd8c7c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:27:27 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 18 Jun 2021 00:27:55 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:27:56 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 00:27:57 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 00:27:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 00:27:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 00:27:59 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:28:00 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:28:00 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:28:00 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 18 Jun 2021 00:28:00 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 18 Jun 2021 00:28:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:28:01 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 18 Jun 2021 00:28:01 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 18 Jun 2021 00:28:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:28:06 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:28:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 18 Jun 2021 00:28:07 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:28:08 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 18 Jun 2021 00:28:08 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 18 Jun 2021 00:28:08 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:28:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a326a111ccc10ba9bc4afb870b990cf972287f3a456db2edc4d9746a64187e55`  
		Last Modified: Fri, 18 Jun 2021 00:29:59 GMT  
		Size: 108.7 MB (108733520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb7da79e196d0c385c9a090b9fcb85dcf4bed23c368670a14c51a32dba5abc`  
		Last Modified: Fri, 18 Jun 2021 00:29:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01ca03f104ac070adf831f5f0062f55a7157ecc540af5dfa601a60a93ef9f6f`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eef0a241f25b6c68d6d42e390771a36e01d4ba94319f30bf786cc2dc7898c0`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 542.5 KB (542504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69347ac2dc61c0c4fa27c2b107e6a7d187ede87fb7f477974a494ae167b9a784`  
		Last Modified: Fri, 18 Jun 2021 00:29:44 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed6e953025df1412d2e9cd49dae2b04e3078eb1fc46c9ad34e22f42fbb3bc82`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d794b86ac4d7732fbe1f314067b26468bace78c75d1867214c1e1a9b12dba904`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:9a489b0919f8f1c664f1c9ad2c02d0c829cc244e1313865fd1a1b2e3adc6b7b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240247814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5746192bc425b7fcac5324c069409888237e3fe83a9e7c803513bc6f96c480`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:21:56 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 20 May 2021 00:31:59 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:32:12 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:32:31 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:32:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:32:50 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:32:55 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:33:03 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:33:05 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:33:10 GMT
ENV BONITA_VERSION=7.10.6
# Thu, 20 May 2021 00:33:13 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Thu, 20 May 2021 00:33:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:33:19 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Thu, 20 May 2021 00:33:33 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 20 May 2021 00:33:45 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 20 May 2021 00:33:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 20 May 2021 00:34:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 20 May 2021 00:34:17 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:34:24 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Thu, 20 May 2021 00:34:27 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 20 May 2021 00:34:32 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:34:37 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d3625bf57aa986338173635f8c468a0b3baebb7cb06bcf800cf33ea59243e`  
		Last Modified: Thu, 20 May 2021 00:47:16 GMT  
		Size: 111.3 MB (111312376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ddc65d68cd15a96d0138a966744a96e6f5f6d6e421d9e716c9d1fee58b402`  
		Last Modified: Thu, 20 May 2021 00:46:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d173c200e8e4c7d2bb8c65ff705b249d5f79a3169a1f659d604db8783c45d7ea`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c697cbb4143f247d5153cf82bd3730d843468e9b25da63fc50bf22fc560f9662`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8b327423d02ef49d83307155cf593fb3c1714c6ef2a349c5ce4e6a4c8dc556`  
		Last Modified: Thu, 20 May 2021 00:47:00 GMT  
		Size: 98.0 MB (97973964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea1f02f4df72a5e3b6ad0034411153e944bcab25a3794c1ab5fd5f0fd8bc7f`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 7.7 KB (7655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f15cf915ec8b010be881a6bab1acf880f036663afbc042282d19259ef8773`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:0ec6db4854c1febd69239d83ac4642e88cb82301f2e94a237fc8a9d7ecbb90e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.6` - linux; amd64

```console
$ docker pull bonita@sha256:35935305b4731cf7bf17388d25216aeb324cc072e694c58f70abcbda537c6454
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242287750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3a38362ab8ae89504f85daa31e91679ec8c876299299fabf8f33ed5e651b78a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:24:15 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 18 Jun 2021 00:25:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:25:42 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 00:25:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 00:25:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 00:25:45 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 00:25:45 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:25:45 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:25:46 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:25:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 18 Jun 2021 00:25:47 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 18 Jun 2021 00:25:51 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:25:52 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:25:54 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 18 Jun 2021 00:25:54 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:25:54 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 18 Jun 2021 00:25:54 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 18 Jun 2021 00:25:54 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:25:55 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5cf33d8a997d9835e64c3f23a107dec928b238d89f74285e02f346b500ad9d`  
		Last Modified: Fri, 18 Jun 2021 00:27:40 GMT  
		Size: 117.0 MB (117028710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f19eb1419d028bd24a0811d06056297eaad1d2e93ab40e819d6127c72b216`  
		Last Modified: Fri, 18 Jun 2021 00:27:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ba5073c63c4c7355d7949aaa99c6b7d620348380a9909f8f79eda73f3f000f`  
		Last Modified: Fri, 18 Jun 2021 00:27:21 GMT  
		Size: 1.9 KB (1908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6a4bcb4a547bc5007dd2e5167a9f1c992abb5e195efec9d725c1d4d1091e0e`  
		Last Modified: Fri, 18 Jun 2021 00:27:22 GMT  
		Size: 573.0 KB (573007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1289a8ce473e558dc7cd99b4cbff9432e7be810e40b9c8017dc3d024a8f53864`  
		Last Modified: Fri, 18 Jun 2021 00:27:26 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e33b79f79b4a846ec471205478dbb72d958b803a53495e27afad6623a2ad7`  
		Last Modified: Fri, 18 Jun 2021 00:27:21 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7684f55978eb4019a36876b9fcd35472055db059ffc17322e7ba9d14bbcff8d`  
		Last Modified: Fri, 18 Jun 2021 00:27:21 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:0fd6a21415cb3f35adfc738e2395f83295d8df16b423fcf2a39a074bebd9d419
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230989530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d44292c71e22fe95cd176de65d21cf33de7c70e355bf18dc0a8b70bcbd8c7c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:27:27 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 18 Jun 2021 00:27:55 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:27:56 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 18 Jun 2021 00:27:57 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 18 Jun 2021 00:27:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 18 Jun 2021 00:27:59 GMT
ARG BONITA_VERSION
# Fri, 18 Jun 2021 00:27:59 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:28:00 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:28:00 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:28:00 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 18 Jun 2021 00:28:00 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 18 Jun 2021 00:28:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:28:01 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 18 Jun 2021 00:28:01 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 18 Jun 2021 00:28:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:28:06 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 18 Jun 2021 00:28:07 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 18 Jun 2021 00:28:07 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:28:08 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 18 Jun 2021 00:28:08 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 18 Jun 2021 00:28:08 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:28:08 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a326a111ccc10ba9bc4afb870b990cf972287f3a456db2edc4d9746a64187e55`  
		Last Modified: Fri, 18 Jun 2021 00:29:59 GMT  
		Size: 108.7 MB (108733520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb7da79e196d0c385c9a090b9fcb85dcf4bed23c368670a14c51a32dba5abc`  
		Last Modified: Fri, 18 Jun 2021 00:29:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01ca03f104ac070adf831f5f0062f55a7157ecc540af5dfa601a60a93ef9f6f`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 1.9 KB (1913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eef0a241f25b6c68d6d42e390771a36e01d4ba94319f30bf786cc2dc7898c0`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 542.5 KB (542504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69347ac2dc61c0c4fa27c2b107e6a7d187ede87fb7f477974a494ae167b9a784`  
		Last Modified: Fri, 18 Jun 2021 00:29:44 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed6e953025df1412d2e9cd49dae2b04e3078eb1fc46c9ad34e22f42fbb3bc82`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d794b86ac4d7732fbe1f314067b26468bace78c75d1867214c1e1a9b12dba904`  
		Last Modified: Fri, 18 Jun 2021 00:29:38 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; ppc64le

```console
$ docker pull bonita@sha256:9a489b0919f8f1c664f1c9ad2c02d0c829cc244e1313865fd1a1b2e3adc6b7b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240247814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5746192bc425b7fcac5324c069409888237e3fe83a9e7c803513bc6f96c480`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:21:56 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 20 May 2021 00:31:59 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:32:12 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:32:31 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:32:45 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:32:50 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:32:55 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:33:03 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:33:05 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:33:10 GMT
ENV BONITA_VERSION=7.10.6
# Thu, 20 May 2021 00:33:13 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Thu, 20 May 2021 00:33:16 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:33:19 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Thu, 20 May 2021 00:33:33 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 20 May 2021 00:33:45 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 20 May 2021 00:33:57 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 20 May 2021 00:34:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 20 May 2021 00:34:17 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:34:24 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Thu, 20 May 2021 00:34:27 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 20 May 2021 00:34:32 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:34:37 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d3625bf57aa986338173635f8c468a0b3baebb7cb06bcf800cf33ea59243e`  
		Last Modified: Thu, 20 May 2021 00:47:16 GMT  
		Size: 111.3 MB (111312376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70ddc65d68cd15a96d0138a966744a96e6f5f6d6e421d9e716c9d1fee58b402`  
		Last Modified: Thu, 20 May 2021 00:46:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d173c200e8e4c7d2bb8c65ff705b249d5f79a3169a1f659d604db8783c45d7ea`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c697cbb4143f247d5153cf82bd3730d843468e9b25da63fc50bf22fc560f9662`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8b327423d02ef49d83307155cf593fb3c1714c6ef2a349c5ce4e6a4c8dc556`  
		Last Modified: Thu, 20 May 2021 00:47:00 GMT  
		Size: 98.0 MB (97973964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea1f02f4df72a5e3b6ad0034411153e944bcab25a3794c1ab5fd5f0fd8bc7f`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 7.7 KB (7655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f15cf915ec8b010be881a6bab1acf880f036663afbc042282d19259ef8773`  
		Last Modified: Thu, 20 May 2021 00:46:52 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:a6b499c2bd1afef3fdf5905dd99b6d075d8de96e26c2b3fb64679f9afa4f8cbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:5ddf07dd0c336712c654b6ca07f31b2be659ec845aca14db2f747f972d31a2d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234102019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885766d082b362d75d5f93364a3ab3e614f22e0af024cd8a8e8fa1b32c6a2a79`
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
# Fri, 18 Jun 2021 00:26:34 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:26:35 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:26:35 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:26:35 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 18 Jun 2021 00:26:35 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 18 Jun 2021 00:26:35 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:26:36 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:26:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:26:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 00:26:38 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 00:26:38 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 18 Jun 2021 00:26:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 18 Jun 2021 00:26:46 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 00:26:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 00:26:48 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:26:48 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 00:26:48 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:26:49 GMT
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
	-	`sha256:cb042c568676cef5a420a0151bf3d8bc2f30dccefa72d7bedfb575906927870e`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7ff0eade39ca8f65d0f62ed65b2d59066ef6519eb13fcd833a7def80ef3683`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c8dbea54febfae99bfdf08a8ee9e0c833532ef612cac278b3b66c3b960f06`  
		Last Modified: Fri, 18 Jun 2021 00:27:56 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4f017dabda584848b83e84bde0a9f9b42784c1bb74951030a67bba3ff47aa3`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c276d2cc231a10135b3fca83772295d8da22a449bd0e2972be7bf15fbde8d059
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223214858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:222652935d8b3839319b5d8a4c034e30aadb18b553f072f5219beff9f3448e36`
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
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 18 Jun 2021 00:28:44 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:28:45 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 00:28:46 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 00:28:46 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 18 Jun 2021 00:28:48 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 18 Jun 2021 00:28:50 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 00:28:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 00:28:51 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:28:52 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 00:28:52 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:28:52 GMT
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
	-	`sha256:6aebb7e116830cf11fe82ea90847a97ebeae6535c9eda0d7616360ccc913f4bd`  
		Last Modified: Fri, 18 Jun 2021 00:30:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e27d0aa27a428577d89efe02b5e60d6eeb3c41c75aa52d8532d32e9ce2382e`  
		Last Modified: Fri, 18 Jun 2021 00:30:12 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59952a8dadb223a521760917ff12f84d24958066749eb35188659385bc23e3eb`  
		Last Modified: Fri, 18 Jun 2021 00:30:20 GMT  
		Size: 113.3 MB (113347829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e805a01485ec5cba7be470d57dff6c8fe2fa77d945c362caa8361d24c227cd91`  
		Last Modified: Fri, 18 Jun 2021 00:30:12 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:3a0e9f9d2f2bf7a9802924e102b4b30425e5b9e4b9c428b3bcf3612a80916a76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230703426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06aa05271136d385134506aa3762425496cec715d104f82cbad3b407cacb78fb`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:34:50 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 20 May 2021 00:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:39:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:39:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:39:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:39:46 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:39:50 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:39:54 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:39:58 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:40:01 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 20 May 2021 00:40:08 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 20 May 2021 00:40:14 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 20 May 2021 00:40:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:40:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 20 May 2021 00:40:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 20 May 2021 00:41:28 GMT
RUN mkdir /opt/files
# Thu, 20 May 2021 00:41:32 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 20 May 2021 00:41:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 20 May 2021 00:42:14 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 20 May 2021 00:42:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 20 May 2021 00:43:03 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:43:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 20 May 2021 00:43:13 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:43:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9e7ad0f0448e92fb16f76c603aecada15c40889d4f1da5923250604fdc460`  
		Last Modified: Thu, 20 May 2021 00:47:47 GMT  
		Size: 86.4 MB (86394726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ff6f34104a98707426da1f362155f111ef7bd4f46193af555901fbe011772b`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd99b523b212592de5647eedf6cad7470492839cbd8cb25bd386a5808114`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56876c96ca39f94c870355914abeb3d9caf5d6f3ccee59ca9329a11528645`  
		Last Modified: Thu, 20 May 2021 00:47:28 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e8feeb8ed1ab8284c5d480339445b621b71d46d2371a16718a04f2e9c5870d`  
		Last Modified: Thu, 20 May 2021 00:47:27 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47243db540c7ff79ad2369746d5b3b1dc08e8b130a680c52b965858c912eb427`  
		Last Modified: Thu, 20 May 2021 00:47:27 GMT  
		Size: 6.9 KB (6890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff860e892d5bd2d0645cb8699bffbf6a02456d61d36fabdfc990809b3a7092ac`  
		Last Modified: Thu, 20 May 2021 00:47:37 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543ed613bddec83beb2f35ef640a48a6680f634cd8be353d098a1c933acd76bd`  
		Last Modified: Thu, 20 May 2021 00:47:27 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:a6b499c2bd1afef3fdf5905dd99b6d075d8de96e26c2b3fb64679f9afa4f8cbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:5ddf07dd0c336712c654b6ca07f31b2be659ec845aca14db2f747f972d31a2d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234102019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885766d082b362d75d5f93364a3ab3e614f22e0af024cd8a8e8fa1b32c6a2a79`
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
# Fri, 18 Jun 2021 00:26:34 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:26:35 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:26:35 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:26:35 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 18 Jun 2021 00:26:35 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 18 Jun 2021 00:26:35 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:26:36 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:26:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:26:37 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 00:26:38 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 00:26:38 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 18 Jun 2021 00:26:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 18 Jun 2021 00:26:46 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 00:26:48 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 00:26:48 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:26:48 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 00:26:48 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:26:49 GMT
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
	-	`sha256:cb042c568676cef5a420a0151bf3d8bc2f30dccefa72d7bedfb575906927870e`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7ff0eade39ca8f65d0f62ed65b2d59066ef6519eb13fcd833a7def80ef3683`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c8dbea54febfae99bfdf08a8ee9e0c833532ef612cac278b3b66c3b960f06`  
		Last Modified: Fri, 18 Jun 2021 00:27:56 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4f017dabda584848b83e84bde0a9f9b42784c1bb74951030a67bba3ff47aa3`  
		Last Modified: Fri, 18 Jun 2021 00:27:50 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:c276d2cc231a10135b3fca83772295d8da22a449bd0e2972be7bf15fbde8d059
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223214858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:222652935d8b3839319b5d8a4c034e30aadb18b553f072f5219beff9f3448e36`
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
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BONITA_SHA256
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BASE_URL
# Fri, 18 Jun 2021 00:28:43 GMT
ARG BONITA_URL
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 18 Jun 2021 00:28:44 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 18 Jun 2021 00:28:44 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 18 Jun 2021 00:28:45 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 18 Jun 2021 00:28:46 GMT
RUN mkdir /opt/files
# Fri, 18 Jun 2021 00:28:46 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 18 Jun 2021 00:28:48 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 18 Jun 2021 00:28:50 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 18 Jun 2021 00:28:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 18 Jun 2021 00:28:51 GMT
VOLUME [/opt/bonita]
# Fri, 18 Jun 2021 00:28:52 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 18 Jun 2021 00:28:52 GMT
EXPOSE 8080
# Fri, 18 Jun 2021 00:28:52 GMT
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
	-	`sha256:6aebb7e116830cf11fe82ea90847a97ebeae6535c9eda0d7616360ccc913f4bd`  
		Last Modified: Fri, 18 Jun 2021 00:30:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e27d0aa27a428577d89efe02b5e60d6eeb3c41c75aa52d8532d32e9ce2382e`  
		Last Modified: Fri, 18 Jun 2021 00:30:12 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59952a8dadb223a521760917ff12f84d24958066749eb35188659385bc23e3eb`  
		Last Modified: Fri, 18 Jun 2021 00:30:20 GMT  
		Size: 113.3 MB (113347829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e805a01485ec5cba7be470d57dff6c8fe2fa77d945c362caa8361d24c227cd91`  
		Last Modified: Fri, 18 Jun 2021 00:30:12 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:3a0e9f9d2f2bf7a9802924e102b4b30425e5b9e4b9c428b3bcf3612a80916a76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230703426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06aa05271136d385134506aa3762425496cec715d104f82cbad3b407cacb78fb`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:34:50 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 20 May 2021 00:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:39:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:39:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:39:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:39:46 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:39:50 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:39:54 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:39:58 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:40:01 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 20 May 2021 00:40:08 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 20 May 2021 00:40:14 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 20 May 2021 00:40:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:40:36 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 20 May 2021 00:40:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 20 May 2021 00:41:28 GMT
RUN mkdir /opt/files
# Thu, 20 May 2021 00:41:32 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 20 May 2021 00:41:57 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 20 May 2021 00:42:14 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 20 May 2021 00:42:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 20 May 2021 00:43:03 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:43:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 20 May 2021 00:43:13 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:43:20 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9e7ad0f0448e92fb16f76c603aecada15c40889d4f1da5923250604fdc460`  
		Last Modified: Thu, 20 May 2021 00:47:47 GMT  
		Size: 86.4 MB (86394726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ff6f34104a98707426da1f362155f111ef7bd4f46193af555901fbe011772b`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd99b523b212592de5647eedf6cad7470492839cbd8cb25bd386a5808114`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56876c96ca39f94c870355914abeb3d9caf5d6f3ccee59ca9329a11528645`  
		Last Modified: Thu, 20 May 2021 00:47:28 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e8feeb8ed1ab8284c5d480339445b621b71d46d2371a16718a04f2e9c5870d`  
		Last Modified: Thu, 20 May 2021 00:47:27 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47243db540c7ff79ad2369746d5b3b1dc08e8b130a680c52b965858c912eb427`  
		Last Modified: Thu, 20 May 2021 00:47:27 GMT  
		Size: 6.9 KB (6890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff860e892d5bd2d0645cb8699bffbf6a02456d61d36fabdfc990809b3a7092ac`  
		Last Modified: Thu, 20 May 2021 00:47:37 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543ed613bddec83beb2f35ef640a48a6680f634cd8be353d098a1c933acd76bd`  
		Last Modified: Thu, 20 May 2021 00:47:27 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:0053ea88b38c83e55d49f544b180559b83214bdf1761e8cf6605a587280962a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

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

### `bonita:7.12` - linux; arm64 variant v8

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

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:09da2c521e70bac97002559c1ffe9aa27945133ad024f1b4dcaf09045d8fa1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233771062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec61d43b322fa845c74b454e498eacf30dfe3dc8c8f6ffe8ea879a1a9f20788d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:34:50 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 20 May 2021 00:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:39:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:39:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:39:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:39:46 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:43:33 GMT
ARG BRANDING_VERSION
# Thu, 20 May 2021 00:43:41 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:43:47 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:43:58 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:44:06 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 20 May 2021 00:44:12 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 20 May 2021 00:44:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 20 May 2021 00:44:21 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:44:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:40 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 20 May 2021 00:44:51 GMT
RUN mkdir /opt/files
# Thu, 20 May 2021 00:44:56 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 20 May 2021 00:45:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 20 May 2021 00:45:39 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 20 May 2021 00:45:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 20 May 2021 00:46:05 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:46:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 20 May 2021 00:46:14 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:46:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9e7ad0f0448e92fb16f76c603aecada15c40889d4f1da5923250604fdc460`  
		Last Modified: Thu, 20 May 2021 00:47:47 GMT  
		Size: 86.4 MB (86394726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ff6f34104a98707426da1f362155f111ef7bd4f46193af555901fbe011772b`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd99b523b212592de5647eedf6cad7470492839cbd8cb25bd386a5808114`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56876c96ca39f94c870355914abeb3d9caf5d6f3ccee59ca9329a11528645`  
		Last Modified: Thu, 20 May 2021 00:47:28 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ebc9951f8a6e042d6aa4d540a3c257fdc84113e4220e55017795b2f7ab3f2b`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e36ed62d5e55e1a0a7ee290d0eee7d9eebadfa7ed944102b57bbb72a0dd572`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b015e0aea1f89925140ec99156b48900b70ecd46a6fe170c7e58634db6db82d`  
		Last Modified: Thu, 20 May 2021 00:48:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b54f55048bca738773475353787939d3fec3a7e0b9f77c543fe7b5cf2aead1f`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:0053ea88b38c83e55d49f544b180559b83214bdf1761e8cf6605a587280962a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

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

### `bonita:7.12.1` - linux; arm64 variant v8

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

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:09da2c521e70bac97002559c1ffe9aa27945133ad024f1b4dcaf09045d8fa1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233771062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec61d43b322fa845c74b454e498eacf30dfe3dc8c8f6ffe8ea879a1a9f20788d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:34:50 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 20 May 2021 00:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:39:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:39:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:39:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:39:46 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:43:33 GMT
ARG BRANDING_VERSION
# Thu, 20 May 2021 00:43:41 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:43:47 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:43:58 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:44:06 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 20 May 2021 00:44:12 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 20 May 2021 00:44:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 20 May 2021 00:44:21 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:44:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:40 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 20 May 2021 00:44:51 GMT
RUN mkdir /opt/files
# Thu, 20 May 2021 00:44:56 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 20 May 2021 00:45:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 20 May 2021 00:45:39 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 20 May 2021 00:45:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 20 May 2021 00:46:05 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:46:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 20 May 2021 00:46:14 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:46:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9e7ad0f0448e92fb16f76c603aecada15c40889d4f1da5923250604fdc460`  
		Last Modified: Thu, 20 May 2021 00:47:47 GMT  
		Size: 86.4 MB (86394726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ff6f34104a98707426da1f362155f111ef7bd4f46193af555901fbe011772b`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd99b523b212592de5647eedf6cad7470492839cbd8cb25bd386a5808114`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56876c96ca39f94c870355914abeb3d9caf5d6f3ccee59ca9329a11528645`  
		Last Modified: Thu, 20 May 2021 00:47:28 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ebc9951f8a6e042d6aa4d540a3c257fdc84113e4220e55017795b2f7ab3f2b`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e36ed62d5e55e1a0a7ee290d0eee7d9eebadfa7ed944102b57bbb72a0dd572`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b015e0aea1f89925140ec99156b48900b70ecd46a6fe170c7e58634db6db82d`  
		Last Modified: Thu, 20 May 2021 00:48:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b54f55048bca738773475353787939d3fec3a7e0b9f77c543fe7b5cf2aead1f`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:0053ea88b38c83e55d49f544b180559b83214bdf1761e8cf6605a587280962a1
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
$ docker pull bonita@sha256:09da2c521e70bac97002559c1ffe9aa27945133ad024f1b4dcaf09045d8fa1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233771062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec61d43b322fa845c74b454e498eacf30dfe3dc8c8f6ffe8ea879a1a9f20788d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 May 2021 21:28:00 GMT
ADD file:4aadf3091aaa7aa0a2de15a19b87dbd768ff54ebf3e30723905e804bafafa7d3 in / 
# Wed, 19 May 2021 21:28:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 21:28:33 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 21:28:46 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 21:28:53 GMT
CMD ["/bin/bash"]
# Thu, 20 May 2021 00:34:50 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 20 May 2021 00:38:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 20 May 2021 00:39:13 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 20 May 2021 00:39:28 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 20 May 2021 00:39:41 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 20 May 2021 00:39:46 GMT
ARG BONITA_VERSION
# Thu, 20 May 2021 00:43:33 GMT
ARG BRANDING_VERSION
# Thu, 20 May 2021 00:43:41 GMT
ARG BONITA_SHA256
# Thu, 20 May 2021 00:43:47 GMT
ARG BASE_URL
# Thu, 20 May 2021 00:43:58 GMT
ARG BONITA_URL
# Thu, 20 May 2021 00:44:06 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 20 May 2021 00:44:12 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 20 May 2021 00:44:17 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 20 May 2021 00:44:21 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:24 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 20 May 2021 00:44:30 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 20 May 2021 00:44:40 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 20 May 2021 00:44:51 GMT
RUN mkdir /opt/files
# Thu, 20 May 2021 00:44:56 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 20 May 2021 00:45:13 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 20 May 2021 00:45:39 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 20 May 2021 00:45:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 20 May 2021 00:46:05 GMT
VOLUME [/opt/bonita]
# Thu, 20 May 2021 00:46:07 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 20 May 2021 00:46:14 GMT
EXPOSE 8080
# Thu, 20 May 2021 00:46:25 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f13c2db25c9606e881665513b807199dbbcf16f443d6077d564a570b13d4cb4b`  
		Last Modified: Wed, 19 May 2021 21:34:00 GMT  
		Size: 30.4 MB (30407160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0c6d78eb67a510d3a36e870ac4a54aca62069696e64e0f309a1d692066ea6`  
		Last Modified: Wed, 19 May 2021 21:33:52 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7b6c37775ff2aaf526ca7ac92641488b18dadb59f8d00857213e0b8ae0e13e`  
		Last Modified: Wed, 19 May 2021 21:33:53 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9e7ad0f0448e92fb16f76c603aecada15c40889d4f1da5923250604fdc460`  
		Last Modified: Thu, 20 May 2021 00:47:47 GMT  
		Size: 86.4 MB (86394726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ff6f34104a98707426da1f362155f111ef7bd4f46193af555901fbe011772b`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd99b523b212592de5647eedf6cad7470492839cbd8cb25bd386a5808114`  
		Last Modified: Thu, 20 May 2021 00:47:31 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca56876c96ca39f94c870355914abeb3d9caf5d6f3ccee59ca9329a11528645`  
		Last Modified: Thu, 20 May 2021 00:47:28 GMT  
		Size: 541.9 KB (541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ebc9951f8a6e042d6aa4d540a3c257fdc84113e4220e55017795b2f7ab3f2b`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e36ed62d5e55e1a0a7ee290d0eee7d9eebadfa7ed944102b57bbb72a0dd572`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b015e0aea1f89925140ec99156b48900b70ecd46a6fe170c7e58634db6db82d`  
		Last Modified: Thu, 20 May 2021 00:48:08 GMT  
		Size: 116.4 MB (116415408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b54f55048bca738773475353787939d3fec3a7e0b9f77c543fe7b5cf2aead1f`  
		Last Modified: Thu, 20 May 2021 00:47:59 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
