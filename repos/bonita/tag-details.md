<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `bonita`

-	[`bonita:7.10`](#bonita710)
-	[`bonita:7.10.5`](#bonita7105)
-	[`bonita:7.11`](#bonita711)
-	[`bonita:7.11.1`](#bonita7111)
-	[`bonita:7.9`](#bonita79)
-	[`bonita:7.9.5`](#bonita795)
-	[`bonita:latest`](#bonitalatest)

## `bonita:7.10`

```console
$ docker pull bonita@sha256:1b530d51d236bccef51453d4002c0f1efdfcc38784e44353523af57fa2d81ed9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:9f7f991e2ba8e701aaab7510ff9ce9c0f25df3a80186bc4e80aec6bae32f9728
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.3 MB (227274164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81191dccc613c27a0a03cfd1f65b5a5a94693c7a294e496c1195303a7d73a92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:42 GMT
ARG BASE_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BONITA_VERSION=7.10.5
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Wed, 19 Aug 2020 21:56:44 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 19 Aug 2020 21:56:51 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:56:54 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:56:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:56:55 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:56:56 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 19 Aug 2020 21:56:56 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 19 Aug 2020 21:56:56 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:56:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c952befdc1b8194511084d8ad34f367d0954961e56905e3f1b490c2c866ac`  
		Last Modified: Wed, 19 Aug 2020 21:58:03 GMT  
		Size: 98.0 MB (97955939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e01956bf1f1770b2580860dde522423119a35469fa00383466953bc84f4e0`  
		Last Modified: Wed, 19 Aug 2020 21:57:39 GMT  
		Size: 7.6 KB (7595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7046b5008810d7be56dc69b02b05074492074826eff60075f7e3199782128c59`  
		Last Modified: Wed, 19 Aug 2020 21:57:39 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5747d88bd63623d7ac115a4a821988fabd30367471b1057075685ddd161a50eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.2 MB (215177534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186123517dee901ee750a7cf4b0389d355eea74dc749debe363cffdf2348ed42`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:45 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 18:36:46 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 18:36:48 GMT
ENV BONITA_VERSION=7.10.5
# Fri, 24 Jul 2020 18:36:49 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Fri, 24 Jul 2020 18:36:50 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 24 Jul 2020 18:36:50 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Fri, 24 Jul 2020 18:36:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 24 Jul 2020 18:37:00 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 18:37:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 18:37:05 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 24 Jul 2020 18:37:08 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 18:37:09 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 24 Jul 2020 18:37:10 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 18:37:10 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 18:37:11 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c7d6cdcb9829488e4673feffe614800d319d47a1188c48be80e76f5bcfd2a0`  
		Last Modified: Fri, 24 Jul 2020 18:38:38 GMT  
		Size: 98.0 MB (97955971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd8c1ac0b5238830ed33fe4608b28bf530720425622e7b4ca2bee9859dd70a3`  
		Last Modified: Fri, 24 Jul 2020 18:38:29 GMT  
		Size: 7.6 KB (7620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361b3feb3deef5236f296237726425c6c5bf96653713d7aea60af3636277b27e`  
		Last Modified: Fri, 24 Jul 2020 18:38:29 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:06295dbf11481d69f32b7d15f2dba20b31127271eab35ed5447310cf638a76e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223838363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45c9a1157fe2702c26783e376d61df025b4beae65d11f76a541becc39342b74`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:29:35 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 15:29:45 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 15:29:58 GMT
ENV BONITA_VERSION=7.10.5
# Fri, 24 Jul 2020 15:30:18 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Fri, 24 Jul 2020 15:30:37 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 24 Jul 2020 15:30:56 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Fri, 24 Jul 2020 15:31:14 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 24 Jul 2020 15:32:12 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 15:32:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 15:32:45 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 24 Jul 2020 15:32:51 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 15:32:57 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 24 Jul 2020 15:33:00 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 15:33:09 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 15:33:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2098aa6b882e16efea4df2aeb18a3b068dbcc097daa5b34c557b99145c3f7`  
		Last Modified: Fri, 24 Jul 2020 15:36:48 GMT  
		Size: 98.0 MB (97955971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe22f80a63eb8288a3c882d487381a5fda7d6a752e7008cef15082de832e7`  
		Last Modified: Fri, 24 Jul 2020 15:36:41 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e339a306b67bc7fd74f4303f47c4d461b3240cb050045a4abd0d491a34bc5dd8`  
		Last Modified: Fri, 24 Jul 2020 15:36:41 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.5`

```console
$ docker pull bonita@sha256:1b530d51d236bccef51453d4002c0f1efdfcc38784e44353523af57fa2d81ed9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.5` - linux; amd64

```console
$ docker pull bonita@sha256:9f7f991e2ba8e701aaab7510ff9ce9c0f25df3a80186bc4e80aec6bae32f9728
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.3 MB (227274164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81191dccc613c27a0a03cfd1f65b5a5a94693c7a294e496c1195303a7d73a92`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:42 GMT
ARG BASE_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BONITA_VERSION=7.10.5
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Wed, 19 Aug 2020 21:56:43 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Wed, 19 Aug 2020 21:56:44 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 19 Aug 2020 21:56:51 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:56:54 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:56:55 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:56:55 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:56:56 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Wed, 19 Aug 2020 21:56:56 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 19 Aug 2020 21:56:56 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:56:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c952befdc1b8194511084d8ad34f367d0954961e56905e3f1b490c2c866ac`  
		Last Modified: Wed, 19 Aug 2020 21:58:03 GMT  
		Size: 98.0 MB (97955939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e01956bf1f1770b2580860dde522423119a35469fa00383466953bc84f4e0`  
		Last Modified: Wed, 19 Aug 2020 21:57:39 GMT  
		Size: 7.6 KB (7595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7046b5008810d7be56dc69b02b05074492074826eff60075f7e3199782128c59`  
		Last Modified: Wed, 19 Aug 2020 21:57:39 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.5` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5747d88bd63623d7ac115a4a821988fabd30367471b1057075685ddd161a50eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.2 MB (215177534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186123517dee901ee750a7cf4b0389d355eea74dc749debe363cffdf2348ed42`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:45 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 18:36:46 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 18:36:48 GMT
ENV BONITA_VERSION=7.10.5
# Fri, 24 Jul 2020 18:36:49 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Fri, 24 Jul 2020 18:36:50 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 24 Jul 2020 18:36:50 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Fri, 24 Jul 2020 18:36:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 24 Jul 2020 18:37:00 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 18:37:02 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 18:37:05 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 24 Jul 2020 18:37:08 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 18:37:09 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 24 Jul 2020 18:37:10 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 18:37:10 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 18:37:11 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c7d6cdcb9829488e4673feffe614800d319d47a1188c48be80e76f5bcfd2a0`  
		Last Modified: Fri, 24 Jul 2020 18:38:38 GMT  
		Size: 98.0 MB (97955971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd8c1ac0b5238830ed33fe4608b28bf530720425622e7b4ca2bee9859dd70a3`  
		Last Modified: Fri, 24 Jul 2020 18:38:29 GMT  
		Size: 7.6 KB (7620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361b3feb3deef5236f296237726425c6c5bf96653713d7aea60af3636277b27e`  
		Last Modified: Fri, 24 Jul 2020 18:38:29 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.5` - linux; ppc64le

```console
$ docker pull bonita@sha256:06295dbf11481d69f32b7d15f2dba20b31127271eab35ed5447310cf638a76e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223838363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45c9a1157fe2702c26783e376d61df025b4beae65d11f76a541becc39342b74`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:29:35 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 15:29:45 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 15:29:58 GMT
ENV BONITA_VERSION=7.10.5
# Fri, 24 Jul 2020 15:30:18 GMT
ENV BONITA_SHA256=bc2bb1048df1b9d8a293635924fd1e7eb2cf0652f65d3fd64c0f1bc22e435dff
# Fri, 24 Jul 2020 15:30:37 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 24 Jul 2020 15:30:56 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.5.zip
# Fri, 24 Jul 2020 15:31:14 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 24 Jul 2020 15:32:12 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 15:32:31 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Jul 2020 15:32:45 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 24 Jul 2020 15:32:51 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 15:32:57 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 24 Jul 2020 15:33:00 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 15:33:09 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 15:33:15 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2098aa6b882e16efea4df2aeb18a3b068dbcc097daa5b34c557b99145c3f7`  
		Last Modified: Fri, 24 Jul 2020 15:36:48 GMT  
		Size: 98.0 MB (97955971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615fe22f80a63eb8288a3c882d487381a5fda7d6a752e7008cef15082de832e7`  
		Last Modified: Fri, 24 Jul 2020 15:36:41 GMT  
		Size: 7.6 KB (7618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e339a306b67bc7fd74f4303f47c4d461b3240cb050045a4abd0d491a34bc5dd8`  
		Last Modified: Fri, 24 Jul 2020 15:36:41 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:573d1331e16f72d4092b7e2717085d5a66ef5caf64996961377c404f7461748a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:702be33230c516826c0717c670725570d2ab726a82a6c1295fd0c258be5205fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242551562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c827df3c2bb731f6e7849ca3f86defef1c63e11bca8045f6910e05bc40802a3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:42 GMT
ARG BASE_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BONITA_VERSION=7.11.1
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 19 Aug 2020 21:57:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Wed, 19 Aug 2020 21:57:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 19 Aug 2020 21:57:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:57:07 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:57:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:57:08 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:57:09 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Wed, 19 Aug 2020 21:57:09 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Wed, 19 Aug 2020 21:57:09 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:57:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b5eac55a40c8b3cdac7fb81076d34e46e77de2aaee956e603fb289ca2f937e`  
		Last Modified: Wed, 19 Aug 2020 21:58:13 GMT  
		Size: 113.2 MB (113233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e62e1bd3478f449c5b3f04c4b7eca6abae67b07b71edb8514dac7e6e15ad193`  
		Last Modified: Wed, 19 Aug 2020 21:58:08 GMT  
		Size: 7.6 KB (7626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153621680648ed6568d3ebf58d76780af7e88f887a4e5179972700fb25f0f16`  
		Last Modified: Wed, 19 Aug 2020 21:58:08 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8c01dad6734f26028c6b140de76f1a60afdcf66c3a79f08909f8180fdf158a7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230454939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e01cc05832e6b7f271cb611727d26e9ef6ba626f5a832e14b98de2e33138867`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:45 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 18:36:46 GMT
ARG BONITA_URL
# Tue, 11 Aug 2020 19:43:27 GMT
ENV BONITA_VERSION=7.11.1
# Tue, 11 Aug 2020 19:43:28 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Tue, 11 Aug 2020 19:43:28 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 11 Aug 2020 19:43:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Tue, 11 Aug 2020 19:43:31 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 11 Aug 2020 19:43:41 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 19:43:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 19:43:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 11 Aug 2020 19:43:47 GMT
VOLUME [/opt/bonita]
# Tue, 11 Aug 2020 19:43:48 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Tue, 11 Aug 2020 19:43:48 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Tue, 11 Aug 2020 19:43:49 GMT
EXPOSE 8080
# Tue, 11 Aug 2020 19:43:50 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1a71e36dea7995351642f9e6283360224eec43f3edaa20c69293bcb667b226`  
		Last Modified: Tue, 11 Aug 2020 19:44:22 GMT  
		Size: 113.2 MB (113233287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcb9af7d9e74359515b021c960417ed4a43553d71f813ad12cf975e99217767`  
		Last Modified: Tue, 11 Aug 2020 19:44:03 GMT  
		Size: 7.7 KB (7659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db876ac2189dad6a40f9b71205d91c32a1f939cddf325f5d8ed5b7588b814a62`  
		Last Modified: Tue, 11 Aug 2020 19:44:04 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:46a12d62583064b20dc5dc5e464f855bae992df10570f9c8df1f94be43646d78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239115773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed8256341d30f9f3fc82988c1bff8c667d9db5ebfa2d70769b19e54d272664d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:29:35 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 15:29:45 GMT
ARG BONITA_URL
# Tue, 11 Aug 2020 20:32:59 GMT
ENV BONITA_VERSION=7.11.1
# Tue, 11 Aug 2020 20:33:12 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Tue, 11 Aug 2020 20:33:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 11 Aug 2020 20:33:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Tue, 11 Aug 2020 20:33:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 11 Aug 2020 20:34:21 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 20:34:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 20:34:50 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 11 Aug 2020 20:34:59 GMT
VOLUME [/opt/bonita]
# Tue, 11 Aug 2020 20:35:02 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Tue, 11 Aug 2020 20:35:05 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Tue, 11 Aug 2020 20:35:13 GMT
EXPOSE 8080
# Tue, 11 Aug 2020 20:35:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be42801dd677c8b8b03e2272fd48e918c74558f615368d64515e5253282277c`  
		Last Modified: Tue, 11 Aug 2020 20:35:53 GMT  
		Size: 113.2 MB (113233289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf0a66d388f71754edfc41324b75df7ce8f8b57b462c023adce8efbf933c036`  
		Last Modified: Tue, 11 Aug 2020 20:35:45 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afb022459ebd3e03885dc35798a8b27ea5348111b3e99cf2292f40a249e57bf`  
		Last Modified: Tue, 11 Aug 2020 20:35:45 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.1`

```console
$ docker pull bonita@sha256:573d1331e16f72d4092b7e2717085d5a66ef5caf64996961377c404f7461748a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.1` - linux; amd64

```console
$ docker pull bonita@sha256:702be33230c516826c0717c670725570d2ab726a82a6c1295fd0c258be5205fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242551562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c827df3c2bb731f6e7849ca3f86defef1c63e11bca8045f6910e05bc40802a3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:42 GMT
ARG BASE_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BONITA_VERSION=7.11.1
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 19 Aug 2020 21:57:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Wed, 19 Aug 2020 21:57:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 19 Aug 2020 21:57:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:57:07 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:57:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:57:08 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:57:09 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Wed, 19 Aug 2020 21:57:09 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Wed, 19 Aug 2020 21:57:09 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:57:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b5eac55a40c8b3cdac7fb81076d34e46e77de2aaee956e603fb289ca2f937e`  
		Last Modified: Wed, 19 Aug 2020 21:58:13 GMT  
		Size: 113.2 MB (113233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e62e1bd3478f449c5b3f04c4b7eca6abae67b07b71edb8514dac7e6e15ad193`  
		Last Modified: Wed, 19 Aug 2020 21:58:08 GMT  
		Size: 7.6 KB (7626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153621680648ed6568d3ebf58d76780af7e88f887a4e5179972700fb25f0f16`  
		Last Modified: Wed, 19 Aug 2020 21:58:08 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8c01dad6734f26028c6b140de76f1a60afdcf66c3a79f08909f8180fdf158a7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230454939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e01cc05832e6b7f271cb611727d26e9ef6ba626f5a832e14b98de2e33138867`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:45 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 18:36:46 GMT
ARG BONITA_URL
# Tue, 11 Aug 2020 19:43:27 GMT
ENV BONITA_VERSION=7.11.1
# Tue, 11 Aug 2020 19:43:28 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Tue, 11 Aug 2020 19:43:28 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 11 Aug 2020 19:43:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Tue, 11 Aug 2020 19:43:31 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 11 Aug 2020 19:43:41 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 19:43:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 19:43:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 11 Aug 2020 19:43:47 GMT
VOLUME [/opt/bonita]
# Tue, 11 Aug 2020 19:43:48 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Tue, 11 Aug 2020 19:43:48 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Tue, 11 Aug 2020 19:43:49 GMT
EXPOSE 8080
# Tue, 11 Aug 2020 19:43:50 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1a71e36dea7995351642f9e6283360224eec43f3edaa20c69293bcb667b226`  
		Last Modified: Tue, 11 Aug 2020 19:44:22 GMT  
		Size: 113.2 MB (113233287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcb9af7d9e74359515b021c960417ed4a43553d71f813ad12cf975e99217767`  
		Last Modified: Tue, 11 Aug 2020 19:44:03 GMT  
		Size: 7.7 KB (7659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db876ac2189dad6a40f9b71205d91c32a1f939cddf325f5d8ed5b7588b814a62`  
		Last Modified: Tue, 11 Aug 2020 19:44:04 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:46a12d62583064b20dc5dc5e464f855bae992df10570f9c8df1f94be43646d78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239115773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed8256341d30f9f3fc82988c1bff8c667d9db5ebfa2d70769b19e54d272664d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:29:35 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 15:29:45 GMT
ARG BONITA_URL
# Tue, 11 Aug 2020 20:32:59 GMT
ENV BONITA_VERSION=7.11.1
# Tue, 11 Aug 2020 20:33:12 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Tue, 11 Aug 2020 20:33:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 11 Aug 2020 20:33:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Tue, 11 Aug 2020 20:33:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 11 Aug 2020 20:34:21 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 20:34:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 20:34:50 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 11 Aug 2020 20:34:59 GMT
VOLUME [/opt/bonita]
# Tue, 11 Aug 2020 20:35:02 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Tue, 11 Aug 2020 20:35:05 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Tue, 11 Aug 2020 20:35:13 GMT
EXPOSE 8080
# Tue, 11 Aug 2020 20:35:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be42801dd677c8b8b03e2272fd48e918c74558f615368d64515e5253282277c`  
		Last Modified: Tue, 11 Aug 2020 20:35:53 GMT  
		Size: 113.2 MB (113233289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf0a66d388f71754edfc41324b75df7ce8f8b57b462c023adce8efbf933c036`  
		Last Modified: Tue, 11 Aug 2020 20:35:45 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afb022459ebd3e03885dc35798a8b27ea5348111b3e99cf2292f40a249e57bf`  
		Last Modified: Tue, 11 Aug 2020 20:35:45 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9`

```console
$ docker pull bonita@sha256:4f77b3fc8b8e253a523192dd403e8ed76c1de1b63229269572914d646cf5a0ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9` - linux; amd64

```console
$ docker pull bonita@sha256:c3c39d7bfc7180ca0fca2f7b83754b64bbf20f14255e2c9f14174561105a5e8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.3 MB (229343159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9caedf4cee4c454b15f1a5ea7b03441148a2e3e5ad4aa01ea1104d41f434f49b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:56:24 GMT
ENV BONITA_VERSION=7.9.5
# Wed, 19 Aug 2020 21:56:24 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Wed, 19 Aug 2020 21:56:24 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Wed, 19 Aug 2020 21:56:31 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 19 Aug 2020 21:56:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 19 Aug 2020 21:56:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:56:34 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:56:34 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Wed, 19 Aug 2020 21:56:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 19 Aug 2020 21:56:35 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:56:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245b523c370f44689f6c28869f2ce5e59965493ba70d3d7e6fe01525fb1bb91`  
		Last Modified: Wed, 19 Aug 2020 21:57:25 GMT  
		Size: 100.0 MB (100024964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ac0068fa3312a54f04bbb94cf8c35e52e4bdf82b6f4fa7e686480ebbe4627f`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2238c824bcc4b7ceaf130924d7c5e46114c172411139beeafee1d4a1df9ef7`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.6 KB (1627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ff7e9b8880ad74aefa8dd8233a06a22672446404dc00ef4b8ea794569f89a6b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217246533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87705f262e956438013c2bc2a7a60e71d490228ea42a5120754eba6ca607ac12`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:14 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 18:36:15 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 24 Jul 2020 18:36:16 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 24 Jul 2020 18:36:17 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 24 Jul 2020 18:36:26 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 18:36:29 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 18:36:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 24 Jul 2020 18:36:33 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 18:36:33 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 24 Jul 2020 18:36:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 18:36:35 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 18:36:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbcc9627255aba055f8e008354c24d8974770b38127357375cd45741cfdd367`  
		Last Modified: Fri, 24 Jul 2020 18:38:01 GMT  
		Size: 100.0 MB (100024999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89fd24dd1f90fed68bdcdfb6ed67af828cfeb61351103e7185412df1c2edb0c`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ed069328443be9a7db1dad5de04b1b4691738742ec6cf2459791a7b2a3217`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9` - linux; ppc64le

```console
$ docker pull bonita@sha256:70f404034dc99d4b0ffcb9196d9a79c33c87a63203a79de80603f89d4a55e8be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225907359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de581d98d5ebb7e96ffad56fe393b81a5862d16ddda0e6a8aa62444710f757a6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:21:43 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 15:22:38 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 24 Jul 2020 15:24:13 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 24 Jul 2020 15:24:33 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 24 Jul 2020 15:26:07 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 15:26:37 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 15:27:21 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 24 Jul 2020 15:27:39 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 15:27:56 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 24 Jul 2020 15:28:07 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 15:28:49 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 15:29:00 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c206c26a5d5560aa39e8751f0b9214cfec83b55ba77e486056f7dbcb2ad89`  
		Last Modified: Fri, 24 Jul 2020 15:35:59 GMT  
		Size: 100.0 MB (100024999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d427418fe29ed17ce10fad53ea5a532d577fcc7c3f6682e2edae074e8030608`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f5cd9afe65492761d758d82c92bb11ea3e453f94b6ae985edf8bae6266d4f6`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.9.5`

```console
$ docker pull bonita@sha256:4f77b3fc8b8e253a523192dd403e8ed76c1de1b63229269572914d646cf5a0ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.9.5` - linux; amd64

```console
$ docker pull bonita@sha256:c3c39d7bfc7180ca0fca2f7b83754b64bbf20f14255e2c9f14174561105a5e8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.3 MB (229343159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9caedf4cee4c454b15f1a5ea7b03441148a2e3e5ad4aa01ea1104d41f434f49b`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:56:24 GMT
ENV BONITA_VERSION=7.9.5
# Wed, 19 Aug 2020 21:56:24 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Wed, 19 Aug 2020 21:56:24 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Wed, 19 Aug 2020 21:56:31 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 19 Aug 2020 21:56:32 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Wed, 19 Aug 2020 21:56:34 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:56:34 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:56:34 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Wed, 19 Aug 2020 21:56:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Wed, 19 Aug 2020 21:56:35 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:56:35 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245b523c370f44689f6c28869f2ce5e59965493ba70d3d7e6fe01525fb1bb91`  
		Last Modified: Wed, 19 Aug 2020 21:57:25 GMT  
		Size: 100.0 MB (100024964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ac0068fa3312a54f04bbb94cf8c35e52e4bdf82b6f4fa7e686480ebbe4627f`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2238c824bcc4b7ceaf130924d7c5e46114c172411139beeafee1d4a1df9ef7`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.6 KB (1627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:ff7e9b8880ad74aefa8dd8233a06a22672446404dc00ef4b8ea794569f89a6b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.2 MB (217246533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87705f262e956438013c2bc2a7a60e71d490228ea42a5120754eba6ca607ac12`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:14 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 18:36:15 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 24 Jul 2020 18:36:16 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 24 Jul 2020 18:36:17 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 24 Jul 2020 18:36:26 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 18:36:29 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 18:36:32 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 24 Jul 2020 18:36:33 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 18:36:33 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 24 Jul 2020 18:36:34 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 18:36:35 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 18:36:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbcc9627255aba055f8e008354c24d8974770b38127357375cd45741cfdd367`  
		Last Modified: Fri, 24 Jul 2020 18:38:01 GMT  
		Size: 100.0 MB (100024999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89fd24dd1f90fed68bdcdfb6ed67af828cfeb61351103e7185412df1c2edb0c`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 7.6 KB (7588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ed069328443be9a7db1dad5de04b1b4691738742ec6cf2459791a7b2a3217`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 1.7 KB (1654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.9.5` - linux; ppc64le

```console
$ docker pull bonita@sha256:70f404034dc99d4b0ffcb9196d9a79c33c87a63203a79de80603f89d4a55e8be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225907359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de581d98d5ebb7e96ffad56fe393b81a5862d16ddda0e6a8aa62444710f757a6`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:21:43 GMT
ARG BONITA_URL
# Fri, 24 Jul 2020 15:22:38 GMT
ENV BONITA_VERSION=7.9.5
# Fri, 24 Jul 2020 15:24:13 GMT
ENV BONITA_SHA256=49620e505f072a4f20ebb936c9391e8665d441df9f650749a61a19a5c52e2932
# Fri, 24 Jul 2020 15:24:33 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.9.5-tomcat.zip
# Fri, 24 Jul 2020 15:26:07 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 15:26:37 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip
# Fri, 24 Jul 2020 15:27:21 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}-tomcat.zip | sha256sum -c -
# Fri, 24 Jul 2020 15:27:39 GMT
VOLUME [/opt/bonita]
# Fri, 24 Jul 2020 15:27:56 GMT
COPY dir:ef58daa6df201fe2eac6b87ad183ec81a5dbb212d47f61a3244b65faca8cb3c6 in /opt/files 
# Fri, 24 Jul 2020 15:28:07 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Jul 2020 15:28:49 GMT
EXPOSE 8080
# Fri, 24 Jul 2020 15:29:00 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c206c26a5d5560aa39e8751f0b9214cfec83b55ba77e486056f7dbcb2ad89`  
		Last Modified: Fri, 24 Jul 2020 15:35:59 GMT  
		Size: 100.0 MB (100024999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d427418fe29ed17ce10fad53ea5a532d577fcc7c3f6682e2edae074e8030608`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 7.6 KB (7587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f5cd9afe65492761d758d82c92bb11ea3e453f94b6ae985edf8bae6266d4f6`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:573d1331e16f72d4092b7e2717085d5a66ef5caf64996961377c404f7461748a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:702be33230c516826c0717c670725570d2ab726a82a6c1295fd0c258be5205fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242551562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c827df3c2bb731f6e7849ca3f86defef1c63e11bca8045f6910e05bc40802a3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:26 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 21:56:20 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:21 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 21:56:22 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 21:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 21:56:23 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 21:56:42 GMT
ARG BASE_URL
# Wed, 19 Aug 2020 21:56:43 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BONITA_VERSION=7.11.1
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Wed, 19 Aug 2020 21:57:01 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 19 Aug 2020 21:57:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Wed, 19 Aug 2020 21:57:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 19 Aug 2020 21:57:05 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:57:07 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 21:57:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 19 Aug 2020 21:57:08 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 21:57:09 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Wed, 19 Aug 2020 21:57:09 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Wed, 19 Aug 2020 21:57:09 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 21:57:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c77a59a669a0c61ac9d2bd35a23c82da32bf28da854ec2c365af6d8c790e697`  
		Last Modified: Wed, 19 Aug 2020 21:57:36 GMT  
		Size: 102.0 MB (101998135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cecdbf0b9eaa5b31892d87f6548de18cd639c85ec28a46afcf960f7590f7f8`  
		Last Modified: Wed, 19 Aug 2020 21:57:20 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fbaebc2d6911a11b1b1ab7881eea292044f738df73e2112f14aa37da7e8ed3`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 1.9 KB (1912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ee871ff91cd53148ba9ddd62bfa9c014591f448680b1d5e2bbd6441fad6ef`  
		Last Modified: Wed, 19 Aug 2020 21:57:19 GMT  
		Size: 572.4 KB (572369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b5eac55a40c8b3cdac7fb81076d34e46e77de2aaee956e603fb289ca2f937e`  
		Last Modified: Wed, 19 Aug 2020 21:58:13 GMT  
		Size: 113.2 MB (113233251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e62e1bd3478f449c5b3f04c4b7eca6abae67b07b71edb8514dac7e6e15ad193`  
		Last Modified: Wed, 19 Aug 2020 21:58:08 GMT  
		Size: 7.6 KB (7626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153621680648ed6568d3ebf58d76780af7e88f887a4e5179972700fb25f0f16`  
		Last Modified: Wed, 19 Aug 2020 21:58:08 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:8c01dad6734f26028c6b140de76f1a60afdcf66c3a79f08909f8180fdf158a7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230454939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e01cc05832e6b7f271cb611727d26e9ef6ba626f5a832e14b98de2e33138867`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 16:21:15 GMT
ADD file:146b4b3953060bbe623c06f374b3b3798872e4e1ddfef76071c7c4b69a834622 in / 
# Fri, 24 Jul 2020 16:21:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 16:21:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 16:23:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 16:23:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:34:44 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 18:36:01 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:36:06 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 18:36:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 18:36:11 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 18:36:12 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 18:36:13 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 18:36:45 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 18:36:46 GMT
ARG BONITA_URL
# Tue, 11 Aug 2020 19:43:27 GMT
ENV BONITA_VERSION=7.11.1
# Tue, 11 Aug 2020 19:43:28 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Tue, 11 Aug 2020 19:43:28 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 11 Aug 2020 19:43:29 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Tue, 11 Aug 2020 19:43:31 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 11 Aug 2020 19:43:41 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 19:43:44 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 19:43:46 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 11 Aug 2020 19:43:47 GMT
VOLUME [/opt/bonita]
# Tue, 11 Aug 2020 19:43:48 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Tue, 11 Aug 2020 19:43:48 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Tue, 11 Aug 2020 19:43:49 GMT
EXPOSE 8080
# Tue, 11 Aug 2020 19:43:50 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:a114936b480795ec46632c29c96e126744c314983ee0d83354804dc39d1afb46`  
		Last Modified: Mon, 13 Jul 2020 15:47:08 GMT  
		Size: 23.7 MB (23721122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ecf0d2a869e5d188121e6b38473e481b66599a26d8df24d22c9170f50bfa9`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 35.2 KB (35205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb48eb870f62ec1a7a4a2d753bf2b92dff62a6dbedaeff6db6e41cb33196bc`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f912b9bb20d998fd0f1a2526d5539f35d34a476da71c783d0041b25b78c0af5`  
		Last Modified: Fri, 24 Jul 2020 16:27:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7aace3625d8fa13cf8b7d77fe57408818354300e46353244fef2776362c56`  
		Last Modified: Fri, 24 Jul 2020 18:38:22 GMT  
		Size: 92.9 MB (92911044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9983df6425d8cd839e1b2ae6052ea46e5ddfd942e2e822f08b65fd37b92eb2a`  
		Last Modified: Fri, 24 Jul 2020 18:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97944ca16225583c86f445ec7811306935d93a1ac397d4c6853f2322b87ce0a4`  
		Last Modified: Fri, 24 Jul 2020 18:37:52 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f054d458bdf6ba532ab669977ad7f78bdddc9716ae73fde3b5f150fe598daf`  
		Last Modified: Fri, 24 Jul 2020 18:37:53 GMT  
		Size: 541.8 KB (541811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1a71e36dea7995351642f9e6283360224eec43f3edaa20c69293bcb667b226`  
		Last Modified: Tue, 11 Aug 2020 19:44:22 GMT  
		Size: 113.2 MB (113233287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcb9af7d9e74359515b021c960417ed4a43553d71f813ad12cf975e99217767`  
		Last Modified: Tue, 11 Aug 2020 19:44:03 GMT  
		Size: 7.7 KB (7659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db876ac2189dad6a40f9b71205d91c32a1f939cddf325f5d8ed5b7588b814a62`  
		Last Modified: Tue, 11 Aug 2020 19:44:04 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:46a12d62583064b20dc5dc5e464f855bae992df10570f9c8df1f94be43646d78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239115773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed8256341d30f9f3fc82988c1bff8c667d9db5ebfa2d70769b19e54d272664d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:57 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Jul 2020 15:15:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:18:17 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Jul 2020 15:18:41 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Jul 2020 15:19:19 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Jul 2020 15:20:18 GMT
ARG BONITA_VERSION
# Fri, 24 Jul 2020 15:21:14 GMT
ARG BONITA_SHA256
# Fri, 24 Jul 2020 15:29:35 GMT
ARG BASE_URL
# Fri, 24 Jul 2020 15:29:45 GMT
ARG BONITA_URL
# Tue, 11 Aug 2020 20:32:59 GMT
ENV BONITA_VERSION=7.11.1
# Tue, 11 Aug 2020 20:33:12 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Tue, 11 Aug 2020 20:33:21 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Tue, 11 Aug 2020 20:33:26 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Tue, 11 Aug 2020 20:33:52 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Tue, 11 Aug 2020 20:34:21 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 20:34:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Tue, 11 Aug 2020 20:34:50 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Tue, 11 Aug 2020 20:34:59 GMT
VOLUME [/opt/bonita]
# Tue, 11 Aug 2020 20:35:02 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Tue, 11 Aug 2020 20:35:05 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Tue, 11 Aug 2020 20:35:13 GMT
EXPOSE 8080
# Tue, 11 Aug 2020 20:35:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dc874fe32813212edae7830ebd9554906d3a9802e744a6530ed9a511570f21`  
		Last Modified: Fri, 24 Jul 2020 15:36:20 GMT  
		Size: 94.9 MB (94888298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eb40fa041d55b9cd41e2e2f1a15e457175cc3a2811e496e29307a862ec43d9`  
		Last Modified: Fri, 24 Jul 2020 15:35:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c80b30a08e97cf721509bb59ba0408d673fed65d3ed71f5db8036232c7504f`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 1.9 KB (1928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a203b158d8938914a6fe005c69beb448eb02aeecdf3e4966988855eda91435`  
		Last Modified: Fri, 24 Jul 2020 15:35:52 GMT  
		Size: 541.5 KB (541549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be42801dd677c8b8b03e2272fd48e918c74558f615368d64515e5253282277c`  
		Last Modified: Tue, 11 Aug 2020 20:35:53 GMT  
		Size: 113.2 MB (113233289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf0a66d388f71754edfc41324b75df7ce8f8b57b462c023adce8efbf933c036`  
		Last Modified: Tue, 11 Aug 2020 20:35:45 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afb022459ebd3e03885dc35798a8b27ea5348111b3e99cf2292f40a249e57bf`  
		Last Modified: Tue, 11 Aug 2020 20:35:45 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
