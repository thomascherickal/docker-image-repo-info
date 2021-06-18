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
