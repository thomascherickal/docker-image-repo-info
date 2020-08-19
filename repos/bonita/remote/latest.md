## `bonita:latest`

```console
$ docker pull bonita@sha256:91443639968582f04ce81ac1ca897b91bf17dd2e0f0cc36f7e3817a68a416c65
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
$ docker pull bonita@sha256:e343c2d43266ed2349188d1934a3ffb938707aa14ab79ff67dfd6eeba4fef8ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230553531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb8ca6b9a851f934ab8a9af5b7e394a6167c97da81c794660f8417bd6ecedfa`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Wed, 19 Aug 2020 21:29:47 GMT
ADD file:b8316fc82a2cf230ce4af7dcf02ec1d7e56b156cf610af8ed23b64509c77c799 in / 
# Wed, 19 Aug 2020 21:29:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:29:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:29:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:29:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:58:48 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Wed, 19 Aug 2020 22:59:53 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:00:03 GMT
RUN mkdir /opt/custom-init.d/
# Wed, 19 Aug 2020 23:00:07 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Wed, 19 Aug 2020 23:00:14 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Wed, 19 Aug 2020 23:00:15 GMT
ARG BONITA_VERSION
# Wed, 19 Aug 2020 23:00:16 GMT
ARG BONITA_SHA256
# Wed, 19 Aug 2020 23:01:12 GMT
ARG BASE_URL
# Wed, 19 Aug 2020 23:01:21 GMT
ARG BONITA_URL
# Wed, 19 Aug 2020 23:01:57 GMT
ENV BONITA_VERSION=7.11.1
# Wed, 19 Aug 2020 23:01:58 GMT
ENV BONITA_SHA256=d2874ada41c0549a6620ef8095c6eb7480e45d8b8143af5f983a06df62a7243d
# Wed, 19 Aug 2020 23:01:59 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Wed, 19 Aug 2020 23:02:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.1/BonitaCommunity-7.11.1.zip
# Wed, 19 Aug 2020 23:02:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Wed, 19 Aug 2020 23:02:08 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 23:02:11 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Wed, 19 Aug 2020 23:02:14 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Wed, 19 Aug 2020 23:02:15 GMT
VOLUME [/opt/bonita]
# Wed, 19 Aug 2020 23:02:15 GMT
COPY dir:6c801c025cd750ee96a4e29676afb9ba394d4bc647bb82010816896eefc044ed in /opt/files 
# Wed, 19 Aug 2020 23:02:16 GMT
COPY dir:173a816fed2c2b9f191c45b4238f2062102518ab7cf02e5e7c4ca6bd9caeb849 in /opt/templates 
# Wed, 19 Aug 2020 23:02:17 GMT
EXPOSE 8080
# Wed, 19 Aug 2020 23:02:18 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:237528ba509b2abcdba1ff1344bab27ad56235cdb3c1c131d3587f6fba4d92c9`  
		Last Modified: Sat, 08 Aug 2020 00:25:26 GMT  
		Size: 23.7 MB (23721798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b96f31d8b2bf3ce9eb4ac49e6c7411defa4057c1791f02f54c14f2de298ec`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 35.2 KB (35203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82b0e39008d2fa246a0dca4cfa5feb15db58591582a839bd69d5000aa2e96d`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ca375b8d34c9bc764ae24791184cba22510f0c002815b4f9766dd0463f5f5e`  
		Last Modified: Wed, 19 Aug 2020 21:32:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa499328d88181b610bd321169ddfae79cc062685c2d814fc9ee9e0f64f48884`  
		Last Modified: Wed, 19 Aug 2020 23:03:00 GMT  
		Size: 93.0 MB (93008962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77dbb04e2b187ba986d33551f147b9dbb5ec706a39c4f8bce3fd4030344ff40`  
		Last Modified: Wed, 19 Aug 2020 23:02:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb109b5149ad75097e05a807148cfc09d6176e7d6d7bb7c74097c3252ec530b`  
		Last Modified: Wed, 19 Aug 2020 23:02:34 GMT  
		Size: 1.9 KB (1917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df301e3dd9a6b4d32ddb4c040e2ed8d7524d49e9df38f146ec3bfb755b382a1`  
		Last Modified: Wed, 19 Aug 2020 23:02:33 GMT  
		Size: 541.8 KB (541807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c0dec10d76eebbfbcf57df8216e9b61671e46a847775ff384611ff67773c2`  
		Last Modified: Wed, 19 Aug 2020 23:03:36 GMT  
		Size: 113.2 MB (113233285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7408b558153f44c75f6b8e79cad243b4f0cea0426903ca2be074394f6b3d6019`  
		Last Modified: Wed, 19 Aug 2020 23:03:31 GMT  
		Size: 7.7 KB (7660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17327412fdf69f8c81f20c4e5253fbc6915dd7e1d2640ab266c6a97c831438a8`  
		Last Modified: Wed, 19 Aug 2020 23:03:31 GMT  
		Size: 1.7 KB (1702 bytes)  
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
