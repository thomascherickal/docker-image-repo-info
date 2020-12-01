## `bonita:latest`

```console
$ docker pull bonita@sha256:7a886a1479432de9b5a6c21b849096f6d5f0c63b57264e5867fc26afb82f0c9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:2fe282a833e9b519992e3d4a0913f30d0b84db488b77d55319488acadbd628a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234623482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57fecf24791e75f308190a6ff5f222176e6d803b55afaddaff2d97b22108c4ee`
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
# Thu, 26 Nov 2020 01:20:58 GMT
ENV BONITA_VERSION=7.11.3
# Thu, 26 Nov 2020 01:20:59 GMT
ENV BONITA_SHA256=01300373642b7bfcc1fea717e1fd9caf460779ea1f35548d6eed61281f2e6068
# Thu, 26 Nov 2020 01:20:59 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.3.zip
# Thu, 26 Nov 2020 01:20:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 26 Nov 2020 01:20:59 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.3/BonitaCommunity-7.11.3.zip
# Thu, 26 Nov 2020 01:21:00 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 26 Nov 2020 01:21:01 GMT
RUN mkdir /opt/files
# Thu, 26 Nov 2020 01:21:01 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 26 Nov 2020 01:21:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 26 Nov 2020 01:21:06 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 26 Nov 2020 01:21:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 26 Nov 2020 01:21:08 GMT
VOLUME [/opt/bonita]
# Thu, 26 Nov 2020 01:21:08 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 26 Nov 2020 01:21:09 GMT
EXPOSE 8080
# Thu, 26 Nov 2020 01:21:09 GMT
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
	-	`sha256:5607d6bcd6438d406a2598a01e01f688c3577bf4f2107b2bb5a49b9edb82fd98`  
		Last Modified: Thu, 26 Nov 2020 01:21:56 GMT  
		Size: 111.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882f0a1b165d2d7144f2f4448a4a014d2bee8af06e620d3ad97c0c613a08f870`  
		Last Modified: Thu, 26 Nov 2020 01:21:56 GMT  
		Size: 6.9 KB (6858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82cb89f54226e7d3d8b13573bb52c74c76bdf3fd29eef0d3b1329e5ee1abd1`  
		Last Modified: Thu, 26 Nov 2020 01:22:03 GMT  
		Size: 113.3 MB (113340347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1ec79eff5afcb505adbba143964d68c6f6954a1236c3e3c55a8f9cfcdc9c4a`  
		Last Modified: Thu, 26 Nov 2020 01:21:56 GMT  
		Size: 1.7 KB (1684 bytes)  
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
$ docker pull bonita@sha256:ea2717d4194c5be17dd01021b5a6536b7708b24be774b8732b43cf51fd7698fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.2 MB (230230767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4523bd5d56a81ffb412d5ca30123f339f045eef5b024569ff58cba20225d647d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 25 Nov 2020 22:21:42 GMT
ADD file:35026c42092857a1d20d4def6ac147d678e1e692decdc43f85d8f738ba889120 in / 
# Wed, 25 Nov 2020 22:22:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:22:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:22:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:22:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:38:41 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Wed, 25 Nov 2020 23:43:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:57 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 25 Nov 2020 23:44:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 25 Nov 2020 23:44:40 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 25 Nov 2020 23:44:43 GMT
ARG BONITA_VERSION
# Wed, 25 Nov 2020 23:44:50 GMT
ARG BONITA_SHA256
# Wed, 25 Nov 2020 23:44:57 GMT
ARG BASE_URL
# Wed, 25 Nov 2020 23:45:00 GMT
ARG BONITA_URL
# Wed, 25 Nov 2020 23:45:06 GMT
ENV BONITA_VERSION=7.11.3
# Wed, 25 Nov 2020 23:45:10 GMT
ENV BONITA_SHA256=01300373642b7bfcc1fea717e1fd9caf460779ea1f35548d6eed61281f2e6068
# Wed, 25 Nov 2020 23:45:14 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.3.zip
# Wed, 25 Nov 2020 23:45:18 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 25 Nov 2020 23:45:23 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.3/BonitaCommunity-7.11.3.zip
# Wed, 25 Nov 2020 23:45:31 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Wed, 25 Nov 2020 23:45:43 GMT
RUN mkdir /opt/files
# Wed, 25 Nov 2020 23:45:48 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Wed, 25 Nov 2020 23:46:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Wed, 25 Nov 2020 23:46:16 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Wed, 25 Nov 2020 23:46:27 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Wed, 25 Nov 2020 23:46:30 GMT
VOLUME [/opt/bonita]
# Wed, 25 Nov 2020 23:46:32 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Wed, 25 Nov 2020 23:46:38 GMT
EXPOSE 8080
# Wed, 25 Nov 2020 23:46:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:83bc949c367f4f6e035dbcaa7d079a2e9f1e2e7a5db662f86772224750819827`  
		Last Modified: Mon, 23 Nov 2020 18:41:36 GMT  
		Size: 30.4 MB (30421462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f6dea43dc0eb34aefcf5ef670e0bfbea3537a558b8760508df497341d5e637`  
		Last Modified: Wed, 25 Nov 2020 22:27:16 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913c73cb17025027afd384c5bd2b5f57add2dc2a5af20be1743da56431b9c5c0`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf09a00b46a9ae066e670fb5a52cf118bbcb7db6c7d13acb539532396f936d`  
		Last Modified: Wed, 25 Nov 2020 23:48:42 GMT  
		Size: 85.9 MB (85915553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81ab6424ca5f5113e433250a89bd46285d1d8ddbbeb7cd7071e34b41419dea1`  
		Last Modified: Wed, 25 Nov 2020 23:48:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470d50a3838e0388b3408306eddd0f545bc5db702691ab2fd82de66c186b30c0`  
		Last Modified: Wed, 25 Nov 2020 23:48:25 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d815f9a029d943ea9c83d5714504ccf0a448bd10c8ea947d80ed6e384de52`  
		Last Modified: Wed, 25 Nov 2020 23:48:22 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ec3b83f44ac69970669ff762c7fcd43a9c6194d87b5c8de7c72d87a354d28c`  
		Last Modified: Wed, 25 Nov 2020 23:48:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7588b0a37a41b6dba6259a5bce5d136036a713693bc622699b915b9bf7c837a`  
		Last Modified: Wed, 25 Nov 2020 23:48:22 GMT  
		Size: 6.9 KB (6895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a207247b4534a79d9b13ec1ebb24c6d6f878e5f5844c8497b8d31c95f0129463`  
		Last Modified: Wed, 25 Nov 2020 23:48:32 GMT  
		Size: 113.3 MB (113340349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d29568baa144577a344149f99a9e5d4059417892f2b3ff788ba6870b805fcc1`  
		Last Modified: Wed, 25 Nov 2020 23:48:22 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
