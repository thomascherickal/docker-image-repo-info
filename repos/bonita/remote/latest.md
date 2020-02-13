## `bonita:latest`

```console
$ docker pull bonita@sha256:265872888975d6770031137e4ecdac87199e80b8ceef7048fb8dab43a35a334a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:89bb3eb3484a36ee1bca0ffa5d426699c60ce58ac5f3d1c5dea0a7d106ecf993
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.9 MB (226944418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dae2e187f2eacc7137c8eedaf335858aa41a6ecb8d47ba6e4545d98923ad0a7`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:45:53 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 16 Jan 2020 02:46:29 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:46:30 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Jan 2020 02:46:31 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Jan 2020 02:46:32 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Jan 2020 02:46:33 GMT
ARG BONITA_VERSION
# Thu, 16 Jan 2020 02:46:33 GMT
ARG BONITA_SHA256
# Thu, 16 Jan 2020 02:47:22 GMT
ARG BASE_URL
# Thu, 16 Jan 2020 02:47:22 GMT
ARG BONITA_URL
# Wed, 12 Feb 2020 23:19:34 GMT
ENV BONITA_VERSION=7.10.1
# Wed, 12 Feb 2020 23:19:34 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Wed, 12 Feb 2020 23:19:35 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 12 Feb 2020 23:19:35 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Wed, 12 Feb 2020 23:19:37 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 12 Feb 2020 23:19:47 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 12 Feb 2020 23:19:49 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 12 Feb 2020 23:19:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 12 Feb 2020 23:19:53 GMT
VOLUME [/opt/bonita]
# Wed, 12 Feb 2020 23:19:53 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 12 Feb 2020 23:19:54 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 12 Feb 2020 23:19:54 GMT
EXPOSE 8080
# Wed, 12 Feb 2020 23:19:54 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c18bfa76311e5747106c3e6e3c8f4028ebfa060f6d9fbcad4f227630c1c68e1`  
		Last Modified: Thu, 16 Jan 2020 02:48:59 GMT  
		Size: 101.7 MB (101742181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf219ff31782c773361f777b6b448888d0eebc89d355bb0e7806af87f6c47d`  
		Last Modified: Thu, 16 Jan 2020 02:48:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc9788a374ab6fa3c497221a369549e4e7100230f1ca11d5691ff530a7c475`  
		Last Modified: Thu, 16 Jan 2020 02:48:40 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45caa22221f8258a786e79aad2d3aa050a2a81502e1de4940f2c4760fb5863ed`  
		Last Modified: Thu, 16 Jan 2020 02:48:40 GMT  
		Size: 572.4 KB (572389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a109767492b255add0df84524354ce3e59f0017f25651769d3a3ad0027a9dc`  
		Last Modified: Wed, 12 Feb 2020 23:20:17 GMT  
		Size: 97.9 MB (97892036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cff49f516414255730cfff564310f6830791928557f828432533a612a9e98c2`  
		Last Modified: Wed, 12 Feb 2020 23:20:09 GMT  
		Size: 7.6 KB (7589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f497fb2ec58210a8b43e9c8a1509c9badbbb5cfa2fb871268b5054af5a21313`  
		Last Modified: Wed, 12 Feb 2020 23:20:09 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:e477b3addfd21445554fd47577c1f1d6e20a75aa0cd94f746552afd6b4950d48
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.0 MB (214959762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187440a3ebc67835a3c85afa41867a2c7cedc5d5391516c1612900a9626922f3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:05:11 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 16 Jan 2020 01:07:15 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:07:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Jan 2020 01:07:25 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Jan 2020 01:07:29 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Jan 2020 01:07:31 GMT
ARG BONITA_VERSION
# Thu, 16 Jan 2020 01:07:33 GMT
ARG BONITA_SHA256
# Thu, 16 Jan 2020 01:08:29 GMT
ARG BASE_URL
# Thu, 16 Jan 2020 01:08:30 GMT
ARG BONITA_URL
# Wed, 12 Feb 2020 22:39:38 GMT
ENV BONITA_VERSION=7.10.1
# Wed, 12 Feb 2020 22:39:39 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Wed, 12 Feb 2020 22:39:39 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 12 Feb 2020 22:39:40 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Wed, 12 Feb 2020 22:39:41 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 12 Feb 2020 22:39:52 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 12 Feb 2020 22:39:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 12 Feb 2020 22:39:57 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 12 Feb 2020 22:39:57 GMT
VOLUME [/opt/bonita]
# Wed, 12 Feb 2020 22:39:58 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 12 Feb 2020 22:39:58 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 12 Feb 2020 22:39:59 GMT
EXPOSE 8080
# Wed, 12 Feb 2020 22:40:00 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687f836221fe42e74c8f4bb70041ff36cc76ff6c86b858618c5b96496442d5a`  
		Last Modified: Thu, 16 Jan 2020 01:09:57 GMT  
		Size: 92.8 MB (92758792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29356b17816bab5922c8715cc0aded3ef7201afa977666aa9c5947e5fae6a44a`  
		Last Modified: Thu, 16 Jan 2020 01:09:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff9428617111ae510c9fb376d52730f7cb702deb824d4f5db22ea62ffeb8897`  
		Last Modified: Thu, 16 Jan 2020 01:09:28 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3405b1dc3ddc2f81f90d18ffdf6891bdebc7e75922450793cf07b6e87ecef310`  
		Last Modified: Thu, 16 Jan 2020 01:09:29 GMT  
		Size: 541.8 KB (541817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c5aeea3b89d9d8b033ef2cca4512cb81ec589719e3359e516bebb5ddfad02e`  
		Last Modified: Wed, 12 Feb 2020 22:40:22 GMT  
		Size: 97.9 MB (97892070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9838efc1b7b1670e2bdaa87de88b474ddd447f3a8ed2526c13aaf1b7980f494b`  
		Last Modified: Wed, 12 Feb 2020 22:40:12 GMT  
		Size: 7.6 KB (7620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a33bd3ebda964359b9031e361bde7dea454d7b2bddd922bf16e12e643b793`  
		Last Modified: Wed, 12 Feb 2020 22:40:12 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:19693c382921f2ec40411bac44c62263a0a5ed084410dfc00a4a06f1e8df202c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223639083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9530e10a29cdc9661e29fb404e8ece6082e4b1be688159d49047d9f72cfe46c4`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:56:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 16 Jan 2020 01:58:44 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:58:51 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 16 Jan 2020 01:58:55 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 16 Jan 2020 01:59:01 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 16 Jan 2020 01:59:02 GMT
ARG BONITA_VERSION
# Thu, 16 Jan 2020 01:59:04 GMT
ARG BONITA_SHA256
# Thu, 16 Jan 2020 02:00:30 GMT
ARG BASE_URL
# Thu, 16 Jan 2020 02:00:33 GMT
ARG BONITA_URL
# Wed, 12 Feb 2020 23:17:00 GMT
ENV BONITA_VERSION=7.10.1
# Wed, 12 Feb 2020 23:17:03 GMT
ENV BONITA_SHA256=29d79e96aa5ab094d758aeacc7e8d435327fe3d8b651554d1077bae03b14f585
# Wed, 12 Feb 2020 23:17:05 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 12 Feb 2020 23:17:08 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.1.zip
# Wed, 12 Feb 2020 23:17:12 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 12 Feb 2020 23:18:07 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 12 Feb 2020 23:18:17 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 12 Feb 2020 23:18:24 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 12 Feb 2020 23:18:26 GMT
VOLUME [/opt/bonita]
# Wed, 12 Feb 2020 23:18:28 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 12 Feb 2020 23:18:29 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 12 Feb 2020 23:18:32 GMT
EXPOSE 8080
# Wed, 12 Feb 2020 23:18:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825fa9d48eb8eea4b00d55e8661d4dc6958bb09fdd4a105a18d04bb0afca7a11`  
		Last Modified: Thu, 16 Jan 2020 02:02:36 GMT  
		Size: 94.8 MB (94757244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0160f86d8032121dc7b4305c25d6eeb3cc692313498bb9a938abc8fa39248f`  
		Last Modified: Thu, 16 Jan 2020 02:02:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241511acd908868c7e96bd24faa65acb5224bbb42926f40e5e22ab691865667f`  
		Last Modified: Thu, 16 Jan 2020 02:02:15 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037203616801241c9e8386145670697ec4c8821176ef468da9eeb5055946d877`  
		Last Modified: Thu, 16 Jan 2020 02:02:15 GMT  
		Size: 541.6 KB (541553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c881a8823b048655858df3403a0f2a4c2ee533f5a233e85bddb1e4ebfc12cf5b`  
		Last Modified: Wed, 12 Feb 2020 23:18:58 GMT  
		Size: 97.9 MB (97892071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ff2f601f3691f3de2e28628f92207a6effe51c5bceb5c21995980c378c0031`  
		Last Modified: Wed, 12 Feb 2020 23:18:51 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c15ed95aa9c0c7c8be69cbd39e8f6369602c963dd95312a9630b963cda487eb`  
		Last Modified: Wed, 12 Feb 2020 23:18:51 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
