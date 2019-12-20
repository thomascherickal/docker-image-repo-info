## `bonita:latest`

```console
$ docker pull bonita@sha256:ab5debb9d6e2e42298e85b791f68c7d2645464a6704dc7e5b336db27486e350d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:29db850781d1b92d6b0dbc42a4171e6c138ff0d4adbb23d951900420f5520df7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.9 MB (226909701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feb05bcdbb14b89820225e70437f3f99de46aa59faf4a81def45c2608c10fc55`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:52:42 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 06:53:40 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:53:41 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 06:53:42 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 06:53:44 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 06:53:44 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 06:53:45 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 23:19:31 GMT
ARG BASE_URL
# Thu, 19 Dec 2019 23:19:31 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 23:19:31 GMT
ENV BONITA_VERSION=7.10.0
# Thu, 19 Dec 2019 23:19:31 GMT
ENV BONITA_SHA256=5ca0a60e3dfd9aa5d82485836b99f08d3f56b4a432ed742a74c51c1e76de3e12
# Thu, 19 Dec 2019 23:19:31 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Thu, 19 Dec 2019 23:19:31 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.0.zip
# Thu, 19 Dec 2019 23:19:32 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 19 Dec 2019 23:19:40 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 19 Dec 2019 23:19:41 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 19 Dec 2019 23:19:43 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 19 Dec 2019 23:19:43 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 23:19:43 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Thu, 19 Dec 2019 23:19:43 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 23:19:44 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 23:19:44 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170227ec870627cbe82ad7fd58b3ab28188e5dcd2cd0455f05ac68824901db1`  
		Last Modified: Thu, 19 Dec 2019 06:54:59 GMT  
		Size: 101.7 MB (101742034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db661a6e0825e45f53aea1d3e30cc53bb0e7a942e300b477337216ba6bf490`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90f396ca202aa29dfb69fdd7256afef6cac8396b9ab3d0b55dde2acb96f0266`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 1.9 KB (1910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e70cbaa2126eb2ddf509ea37cbbab4e42220e63afba09527db1da4035fc9c01`  
		Last Modified: Thu, 19 Dec 2019 06:54:40 GMT  
		Size: 572.4 KB (572378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2149ef1c5bd0694cc861cd28c5932894c24d01e8b94d0599eb7f7ad055115f7a`  
		Last Modified: Thu, 19 Dec 2019 23:20:03 GMT  
		Size: 97.9 MB (97858117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd528df484c5c6cb44495a897ef41c1fbd182465510c2e30531325730078a77f`  
		Last Modified: Thu, 19 Dec 2019 23:19:52 GMT  
		Size: 7.6 KB (7594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7acd21b23082583b5b31e00a2657b3f5db87246987a8e621cbef0dd1e117cc9d`  
		Last Modified: Thu, 19 Dec 2019 23:19:52 GMT  
		Size: 1.6 KB (1624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:d0b3b612c878f973271feca21a88036d714138acf7c410df9b9aa0f4cdb6c93c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214926470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:222ccc9494b47bc57a0f9b410f36153780591396bcceba21024d15ea95412a6a`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 03:49:55 GMT
ADD file:1f180a3d70349350f43f477e4053af7a5fbc4d62d4e76ada091884500bfb6ee1 in / 
# Thu, 19 Dec 2019 03:50:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:50:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:50:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:50:20 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 08:01:24 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 08:02:50 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 08:03:03 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 08:03:06 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 08:03:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 08:03:13 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 08:03:14 GMT
ARG BONITA_SHA256
# Fri, 20 Dec 2019 00:11:08 GMT
ARG BASE_URL
# Fri, 20 Dec 2019 00:11:09 GMT
ARG BONITA_URL
# Fri, 20 Dec 2019 00:11:09 GMT
ENV BONITA_VERSION=7.10.0
# Fri, 20 Dec 2019 00:11:10 GMT
ENV BONITA_SHA256=5ca0a60e3dfd9aa5d82485836b99f08d3f56b4a432ed742a74c51c1e76de3e12
# Fri, 20 Dec 2019 00:11:11 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 20 Dec 2019 00:11:12 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.0.zip
# Fri, 20 Dec 2019 00:11:14 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 20 Dec 2019 00:11:27 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 20 Dec 2019 00:11:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 20 Dec 2019 00:11:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 20 Dec 2019 00:11:39 GMT
VOLUME [/opt/bonita]
# Fri, 20 Dec 2019 00:11:40 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 20 Dec 2019 00:11:42 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 20 Dec 2019 00:11:44 GMT
EXPOSE 8080
# Fri, 20 Dec 2019 00:11:46 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:083ab90813fd405397dbca2b021972603ae62211e401e42b4e928dff050de9c2`  
		Last Modified: Mon, 02 Dec 2019 15:30:26 GMT  
		Size: 23.7 MB (23718714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87467c9ed1fdecf80ce31dc51b980ebd7b2391419ff6113f32e4d170c9f4c4b6`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7a1b2b6a922bf6c8024e2f9276928ed5e5538fd58bf3f0ba6a4a193d515ee7`  
		Last Modified: Thu, 19 Dec 2019 03:55:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69de117a966f92306b4142bdfbccb0b74cbef319ce8b1c6652cf92ce28b0ddf1`  
		Last Modified: Thu, 19 Dec 2019 03:55:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443a608c3163dadc992c54bcdcff7aa6a5523d4d43f1dcd9551d1e3ee18486ba`  
		Last Modified: Thu, 19 Dec 2019 08:04:56 GMT  
		Size: 92.8 MB (92760193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62c646ea143b7a7dd976a5770f9857c4ea11c36e72f33bbf762bf277b80f42`  
		Last Modified: Thu, 19 Dec 2019 08:04:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfe768061a33d6c6421f1a53866b8074abcb686b3f7f2a77bc815d5a6461ab9`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 1.9 KB (1919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6b6b39701aa9bc350a8722c4aadba85f69bb1d21f02c9e93707a3215b1dc4`  
		Last Modified: Thu, 19 Dec 2019 08:04:28 GMT  
		Size: 541.8 KB (541819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c107ae89c8774bc04bf0542e2745917e8c47dfd3020fb455b2a3e9a851184236`  
		Last Modified: Fri, 20 Dec 2019 00:12:12 GMT  
		Size: 97.9 MB (97858161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd1d5dd45d59d2399dc4e062c90ac51e0310e247b95e88ef8831d886d4c8f28`  
		Last Modified: Fri, 20 Dec 2019 00:12:00 GMT  
		Size: 7.6 KB (7621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c713b4dd045d6c9993ac6af5d1a81b56ab02478ed2c1466d09c788cc995407`  
		Last Modified: Fri, 20 Dec 2019 00:12:00 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:0fd466cb165379ee1f70b5033731bc575d2b446f68c9b9ad322e132bf72288c3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223604744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc82e24bac9fa623f4216a87c2fe09fa31738dd9235cc676dcb290c2c28a992`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 19 Dec 2019 04:17:50 GMT
ADD file:04095d1b229274e65c9beb48f6cf33050e58d8ee2cd59c0063d23301a1b68f40 in / 
# Thu, 19 Dec 2019 04:17:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:18:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:18:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:18:08 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:05:50 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 19 Dec 2019 09:07:52 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 09:07:58 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 19 Dec 2019 09:08:04 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 19 Dec 2019 09:08:12 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 19 Dec 2019 09:08:14 GMT
ARG BONITA_VERSION
# Thu, 19 Dec 2019 09:08:16 GMT
ARG BONITA_SHA256
# Thu, 19 Dec 2019 23:38:26 GMT
ARG BASE_URL
# Thu, 19 Dec 2019 23:38:29 GMT
ARG BONITA_URL
# Thu, 19 Dec 2019 23:38:33 GMT
ENV BONITA_VERSION=7.10.0
# Thu, 19 Dec 2019 23:38:35 GMT
ENV BONITA_SHA256=5ca0a60e3dfd9aa5d82485836b99f08d3f56b4a432ed742a74c51c1e76de3e12
# Thu, 19 Dec 2019 23:38:37 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Thu, 19 Dec 2019 23:38:39 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.0.zip
# Thu, 19 Dec 2019 23:38:46 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 19 Dec 2019 23:41:29 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 19 Dec 2019 23:41:38 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 19 Dec 2019 23:41:45 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 19 Dec 2019 23:41:49 GMT
VOLUME [/opt/bonita]
# Thu, 19 Dec 2019 23:41:53 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Thu, 19 Dec 2019 23:41:54 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 19 Dec 2019 23:41:56 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 23:41:59 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:fc185e8867852536dd99638d9087ed0059bd4d581436d4c2aac0d0e17666457a`  
		Last Modified: Mon, 02 Dec 2019 15:30:19 GMT  
		Size: 30.4 MB (30400283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e561dfe3fdb898460f7652cbe0a7bb83e64b240d2504cec93d1b4a1cff37951`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5731b4e21c4ef8f9ab7c0d9535bc069ed88e51e1701f2c89b9260bbabc3ab4`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c7d0deb99d27ed750b5a40c0b038d79913a8644af69d2954631935aab9d88`  
		Last Modified: Thu, 19 Dec 2019 04:24:04 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67a74488fd80b101ca952140e3ef48dbd39197f1d7f0dd349ca7b8160ef81af`  
		Last Modified: Thu, 19 Dec 2019 09:10:46 GMT  
		Size: 94.8 MB (94757160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e66c98cb74b4efc907e66b9b991aeecf8de984a4d0cf5e935b6468be2bb3a0`  
		Last Modified: Thu, 19 Dec 2019 09:10:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c5f99428d6d73821011b103a3b1bd656701141e8d054d615890c06c4caa8b5`  
		Last Modified: Thu, 19 Dec 2019 09:10:23 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56404ca74743e278ac37ae9c2f1394d3169131600ac3f91291af13f6568d8901`  
		Last Modified: Thu, 19 Dec 2019 09:10:24 GMT  
		Size: 541.5 KB (541543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9564a25ce58f9d46a39fc84a58fa8932816a15f89d2981906249232c305bafe`  
		Last Modified: Thu, 19 Dec 2019 23:42:23 GMT  
		Size: 97.9 MB (97858161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35251164a1d7d2a4a1404ae698167175c92c988ea94f7f06272ee708310558`  
		Last Modified: Thu, 19 Dec 2019 23:42:18 GMT  
		Size: 7.6 KB (7621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7423dbaa8862a5313dd49a502b2e7c5aef07a2928209f9e74a22f2ab0380017e`  
		Last Modified: Thu, 19 Dec 2019 23:42:16 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
