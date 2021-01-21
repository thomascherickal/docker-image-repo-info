## `bonita:latest`

```console
$ docker pull bonita@sha256:db1af584c35f730a25670e2b35d005ea6a46af197a0cc8db269f75b78815ccfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:781f06fe6179273cb59ae2cc6d8f44cd41601172d87f29a2f57299af164be8d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234630969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb739c1ecf68aa7260a9a9c980cf85dc0d6fd73669acfa855c8ab9fbc6dc0a6c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:20:30 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 26 Nov 2020 01:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:20:55 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 26 Nov 2020 01:20:56 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 26 Nov 2020 01:20:57 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 26 Nov 2020 01:20:58 GMT
ARG BONITA_VERSION
# Thu, 26 Nov 2020 01:20:58 GMT
ARG BONITA_SHA256
# Thu, 26 Nov 2020 01:20:58 GMT
ARG BASE_URL
# Thu, 26 Nov 2020 01:20:58 GMT
ARG BONITA_URL
# Tue, 01 Dec 2020 23:25:36 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 01 Dec 2020 23:25:36 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 01 Dec 2020 23:25:37 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 01 Dec 2020 23:25:37 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 01 Dec 2020 23:25:37 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 01 Dec 2020 23:25:38 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 01 Dec 2020 23:25:39 GMT
RUN mkdir /opt/files
# Tue, 01 Dec 2020 23:25:39 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 01 Dec 2020 23:25:43 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 01 Dec 2020 23:25:45 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 01 Dec 2020 23:25:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 01 Dec 2020 23:25:46 GMT
VOLUME [/opt/bonita]
# Tue, 01 Dec 2020 23:25:47 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 01 Dec 2020 23:25:47 GMT
EXPOSE 8080
# Tue, 01 Dec 2020 23:25:47 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b85168e6a8b5cdbc4769e21c5a241e07e5472f0cfa530fa1a7bad488e41ff9c`  
		Last Modified: Thu, 26 Nov 2020 01:22:14 GMT  
		Size: 94.0 MB (93991041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40259c64edf46fa9394646de5814cbe53c324ab74789f558d2a39ea61e5897fb`  
		Last Modified: Thu, 26 Nov 2020 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e02d62b18d017fec47ab529ccf26d7e96d1564a3abb6e81cc4e61fda578f2a`  
		Last Modified: Thu, 26 Nov 2020 01:21:58 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e64c6efb7e1c559398788ec003653014f843c1138ab75fd42da2f2e9ebeb2a`  
		Last Modified: Thu, 26 Nov 2020 01:21:56 GMT  
		Size: 572.4 KB (572370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dfeb55f4bade68c36db6f10a4c5b8f777033c739d13116ec0036054727d609`  
		Last Modified: Tue, 01 Dec 2020 23:25:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb39d172a64a0199b49dd7bc6e0496a83ff219a2ae91e5e8fbb12f57dceeb3e`  
		Last Modified: Tue, 01 Dec 2020 23:25:59 GMT  
		Size: 6.9 KB (6859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713d93a62bcbb1730ac94a4c4c26d5f637d51cd24c0a29cd8e00f1a667c71584`  
		Last Modified: Tue, 01 Dec 2020 23:26:04 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b593171bcab93e980914300c579afcacb8571ec8a00581ad87db860a9f8675db`  
		Last Modified: Tue, 01 Dec 2020 23:25:58 GMT  
		Size: 1.7 KB (1687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:3913a2367d686cee94696828ab5226be60569283b787b2869268f4c3024676ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.9 MB (222924098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880b2e3442d59907f72c69a90cb9cb9a8effb9c8f1207553875cda64abda060b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:22:27 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 25 Nov 2020 23:23:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:23:12 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 25 Nov 2020 23:23:14 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 25 Nov 2020 23:23:17 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 25 Nov 2020 23:23:18 GMT
ARG BONITA_VERSION
# Wed, 25 Nov 2020 23:23:19 GMT
ARG BONITA_SHA256
# Wed, 25 Nov 2020 23:23:20 GMT
ARG BASE_URL
# Wed, 25 Nov 2020 23:23:20 GMT
ARG BONITA_URL
# Tue, 01 Dec 2020 22:40:04 GMT
ENV BONITA_VERSION=7.11.4
# Tue, 01 Dec 2020 22:40:04 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Tue, 01 Dec 2020 22:40:05 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Tue, 01 Dec 2020 22:40:06 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 01 Dec 2020 22:40:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Tue, 01 Dec 2020 22:40:08 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Tue, 01 Dec 2020 22:40:10 GMT
RUN mkdir /opt/files
# Tue, 01 Dec 2020 22:40:11 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Tue, 01 Dec 2020 22:40:18 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Tue, 01 Dec 2020 22:40:21 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Tue, 01 Dec 2020 22:40:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Tue, 01 Dec 2020 22:40:24 GMT
VOLUME [/opt/bonita]
# Tue, 01 Dec 2020 22:40:25 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Tue, 01 Dec 2020 22:40:26 GMT
EXPOSE 8080
# Tue, 01 Dec 2020 22:40:26 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3335ad1be83802b9f36928a96aa3a203e1f531d22653bdeff056b041e3bc0c`  
		Last Modified: Wed, 25 Nov 2020 23:25:16 GMT  
		Size: 85.3 MB (85289407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d8f8d85c5729d26e222dafc8d445ff4381b1afa3aef91df27ec421dd3490fc`  
		Last Modified: Wed, 25 Nov 2020 23:24:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0fa485948e28ade7253e1e39f15ce35450083f6f490dfa4b16cd16d45b1ae1`  
		Last Modified: Wed, 25 Nov 2020 23:24:56 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da1ea701841366686df534cbdb465cd768dfd42b68dd63782cc0f11f1757c4c`  
		Last Modified: Wed, 25 Nov 2020 23:24:54 GMT  
		Size: 541.8 KB (541828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa9100fa1a9da5ca225b632c107896eed448bb8deb56a8236ba56f1eae7dbac`  
		Last Modified: Tue, 01 Dec 2020 22:40:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee59255f6b39e11ce6454259f4d4b9136f7cbe4c27c6b091e55fd73bc1b6544`  
		Last Modified: Tue, 01 Dec 2020 22:40:42 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f5e2ddb44072fd0219951e68b8e4d0ef0f444aa1b817d46ec6afbd57da5003`  
		Last Modified: Tue, 01 Dec 2020 22:40:53 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caff92d9e4664536e931be0b7c69462c9a0a16e67c13d9ee17b12ee81bb5bdf`  
		Last Modified: Tue, 01 Dec 2020 22:40:42 GMT  
		Size: 1.7 KB (1713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:1775b31bd091990c8ee76d8008a159f6c4fdfffa75e296fcc182e834a21544d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.2 MB (230241157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fe55d84a7f19877b8d13a999ae20f712b89fc2e506fa927710ba8b61013d12`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 04:23:39 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 21 Jan 2021 04:27:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 04:28:04 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 21 Jan 2021 04:28:10 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 21 Jan 2021 04:28:18 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 21 Jan 2021 04:28:22 GMT
ARG BONITA_VERSION
# Thu, 21 Jan 2021 04:28:26 GMT
ARG BONITA_SHA256
# Thu, 21 Jan 2021 04:28:30 GMT
ARG BASE_URL
# Thu, 21 Jan 2021 04:28:32 GMT
ARG BONITA_URL
# Thu, 21 Jan 2021 04:28:37 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 21 Jan 2021 04:28:41 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 21 Jan 2021 04:28:44 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 21 Jan 2021 04:28:47 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 21 Jan 2021 04:28:49 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 21 Jan 2021 04:28:55 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 21 Jan 2021 04:29:05 GMT
RUN mkdir /opt/files
# Thu, 21 Jan 2021 04:29:07 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 21 Jan 2021 04:29:23 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 21 Jan 2021 04:29:30 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 21 Jan 2021 04:29:40 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 21 Jan 2021 04:29:43 GMT
VOLUME [/opt/bonita]
# Thu, 21 Jan 2021 04:29:51 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 21 Jan 2021 04:29:55 GMT
EXPOSE 8080
# Thu, 21 Jan 2021 04:29:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13b45af58aa295d275be3fb2ee2cdae02906032f23429acfe6e350037d8ab93`  
		Last Modified: Thu, 21 Jan 2021 04:31:44 GMT  
		Size: 85.9 MB (85917102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b382bfd13fccaece5a5a9972badb85c89b4e5d49d62b01a5c56586d69dff55`  
		Last Modified: Thu, 21 Jan 2021 04:31:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b765dbe8b65a01b5e7a6c6bcf266a3f252f9ecab42044078374cd592222b75c1`  
		Last Modified: Thu, 21 Jan 2021 04:31:25 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9bc546cf88c8886a652c41a34d2b48be1bdf5a74182087aea7df14653843a8`  
		Last Modified: Thu, 21 Jan 2021 04:31:21 GMT  
		Size: 541.5 KB (541539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c93abec29ddc090408885bdbc819a7f8683da1f890a9715fb57444c54a13d7`  
		Last Modified: Thu, 21 Jan 2021 04:31:21 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58af7537f4df108a07f0bee0e14a66013e96015a9c6a6158c3781fe7b67b8370`  
		Last Modified: Thu, 21 Jan 2021 04:31:21 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247670b29b11f8ee3a4863d091ecc7144ccbd59c145ea12b2a9a276df91e24a7`  
		Last Modified: Thu, 21 Jan 2021 04:31:30 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645d94b6347d9ee25f4b3df7bdef0a0864af5427b7fd61aaf5dad4c479fc54d3`  
		Last Modified: Thu, 21 Jan 2021 04:31:20 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
