## `bonita:latest`

```console
$ docker pull bonita@sha256:aaeab85c6cb12331ecc8caf0ec0c01ee8747b8c0ac95031ad9dc1880c4c78a95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:196a4ef6eb7abf2c13a3fcd5de4c756982085650dbae0457ba25a44e241fe903
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227043599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb833e80d9495cbef79b00fbfb080e444fde92f76462b6331dde33a34d0d5d1`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 20:04:24 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 20 Mar 2020 20:05:02 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 20:05:03 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 20 Mar 2020 20:05:04 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 20 Mar 2020 20:05:05 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 20 Mar 2020 20:05:06 GMT
ARG BONITA_VERSION
# Fri, 20 Mar 2020 20:05:06 GMT
ARG BONITA_SHA256
# Fri, 20 Mar 2020 20:05:28 GMT
ARG BASE_URL
# Fri, 20 Mar 2020 20:05:28 GMT
ARG BONITA_URL
# Thu, 02 Apr 2020 22:19:40 GMT
ENV BONITA_VERSION=7.10.4
# Thu, 02 Apr 2020 22:19:40 GMT
ENV BONITA_SHA256=dfc3d6d43a6fda7e0e57a60238e63c754d1a948f3c3e36f460f9c7867bf25d6d
# Thu, 02 Apr 2020 22:19:40 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Thu, 02 Apr 2020 22:19:40 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.4.zip
# Thu, 02 Apr 2020 22:19:41 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 02 Apr 2020 22:19:48 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 02 Apr 2020 22:19:49 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 02 Apr 2020 22:19:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 02 Apr 2020 22:19:51 GMT
VOLUME [/opt/bonita]
# Thu, 02 Apr 2020 22:19:51 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Thu, 02 Apr 2020 22:19:51 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 02 Apr 2020 22:19:51 GMT
EXPOSE 8080
# Thu, 02 Apr 2020 22:19:52 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e809724c76d3a847a2f3c13e147bbaa30a6f8a8afb3ac9e5761bbaec228dfb86`  
		Last Modified: Fri, 20 Mar 2020 20:06:06 GMT  
		Size: 101.8 MB (101838679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3783619c639b11c0b7c4dea91ba857489ba23f4ac67ebe001e5ebb4d280ebbe`  
		Last Modified: Fri, 20 Mar 2020 20:05:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2f88b6b917c1ca37d8be8e3e9b66915725bcc5c8a20874d45cc6ee734df32f`  
		Last Modified: Fri, 20 Mar 2020 20:05:48 GMT  
		Size: 1.9 KB (1911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c0ee29b3d9233947c695865ae65a327dc149476354edca5f705e731d055a7e`  
		Last Modified: Fri, 20 Mar 2020 20:05:49 GMT  
		Size: 572.4 KB (572392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022321ec40c93ec886faeff5e2eeca16250bd485ad7d23de121ace2a5565c080`  
		Last Modified: Thu, 02 Apr 2020 22:20:07 GMT  
		Size: 97.9 MB (97894308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8a7ddebbf572f59052ac9f6b2e81669c1d74c13ea326a7a1b34ee909ca32c6`  
		Last Modified: Thu, 02 Apr 2020 22:20:00 GMT  
		Size: 7.6 KB (7593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb9bf06a1ba8be756ce851b692dcecf44aec609b4d5cb71af8818a009b6b913`  
		Last Modified: Thu, 02 Apr 2020 22:20:00 GMT  
		Size: 1.6 KB (1625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5e3ab73d89b5394d0e981ce2ac94549a06ed1a76262e5198138a200c90415c1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.1 MB (215098289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7d8f981bf568189e3f1d4ea0ccf59f7c771c4921b0e8182d969063e79509e7`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 14:49:47 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Apr 2020 14:50:43 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 14:50:46 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Apr 2020 14:50:48 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Apr 2020 14:50:51 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Apr 2020 14:50:52 GMT
ARG BONITA_VERSION
# Fri, 24 Apr 2020 14:50:53 GMT
ARG BONITA_SHA256
# Fri, 24 Apr 2020 14:51:21 GMT
ARG BASE_URL
# Fri, 24 Apr 2020 14:51:22 GMT
ARG BONITA_URL
# Fri, 24 Apr 2020 14:51:22 GMT
ENV BONITA_VERSION=7.10.4
# Fri, 24 Apr 2020 14:51:23 GMT
ENV BONITA_SHA256=dfc3d6d43a6fda7e0e57a60238e63c754d1a948f3c3e36f460f9c7867bf25d6d
# Fri, 24 Apr 2020 14:51:23 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 24 Apr 2020 14:51:24 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.4.zip
# Fri, 24 Apr 2020 14:51:26 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 24 Apr 2020 14:51:33 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Apr 2020 14:51:35 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Apr 2020 14:51:38 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 24 Apr 2020 14:51:38 GMT
VOLUME [/opt/bonita]
# Fri, 24 Apr 2020 14:51:39 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 24 Apr 2020 14:51:40 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Apr 2020 14:51:40 GMT
EXPOSE 8080
# Fri, 24 Apr 2020 14:51:41 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2210822f61f96d7e745e40df9f543663e11257e30e222922939e493ce84391`  
		Last Modified: Fri, 24 Apr 2020 14:52:17 GMT  
		Size: 92.9 MB (92894148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da78a5d628eeced4dbcd79fa0e31b79eb98b03653ca4aac6cf5ec07f3bd1adbb`  
		Last Modified: Fri, 24 Apr 2020 14:51:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d5ac45fda3ff93dd1c8425e8142db093d713781507c31944c2272e36f41d63`  
		Last Modified: Fri, 24 Apr 2020 14:51:52 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4dc691455a24b37b3a825b3af8453c60a3bd369c126ed132efa3c93ddd45ec`  
		Last Modified: Fri, 24 Apr 2020 14:51:52 GMT  
		Size: 541.8 KB (541813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74ef6fa8c44c6d7a7262cea5643600646c3cd6143a3201dd397b94fab9fd497`  
		Last Modified: Fri, 24 Apr 2020 14:52:52 GMT  
		Size: 97.9 MB (97894347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732442ba8a617240da60ddab3494eb4639e3600bb03951f225a648742e04779f`  
		Last Modified: Fri, 24 Apr 2020 14:52:24 GMT  
		Size: 7.6 KB (7621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4cbc9dc278dda6da0df07664d2a1166d9f4cfefdb9983cce796cb2869ee4b`  
		Last Modified: Fri, 24 Apr 2020 14:52:25 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:7c32385effd35f026f4264c530280cf83a84f6920b3adf64a13cc73edd7c8a4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223761201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949920ba72aac0913ccff0e0e4005a0f353df3c00c00d5530acf3c30232c1850`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 23 Apr 2020 20:42:30 GMT
ADD file:726a32203fbcaae787c10740754e38dcb186778893e6d078db3cba0f49ee6b3c in / 
# Thu, 23 Apr 2020 20:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 20:42:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 20:42:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 20:42:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:12:14 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 24 Apr 2020 11:16:15 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:16:28 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 24 Apr 2020 11:16:38 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 24 Apr 2020 11:16:47 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 24 Apr 2020 11:16:50 GMT
ARG BONITA_VERSION
# Fri, 24 Apr 2020 11:16:54 GMT
ARG BONITA_SHA256
# Fri, 24 Apr 2020 11:18:40 GMT
ARG BASE_URL
# Fri, 24 Apr 2020 11:18:43 GMT
ARG BONITA_URL
# Fri, 24 Apr 2020 11:18:47 GMT
ENV BONITA_VERSION=7.10.4
# Fri, 24 Apr 2020 11:18:51 GMT
ENV BONITA_SHA256=dfc3d6d43a6fda7e0e57a60238e63c754d1a948f3c3e36f460f9c7867bf25d6d
# Fri, 24 Apr 2020 11:18:53 GMT
ENV BASE_URL=https://release.ow2.org/bonita
# Fri, 24 Apr 2020 11:18:56 GMT
ENV BONITA_URL=https://release.ow2.org/bonita/BonitaCommunity-7.10.4.zip
# Fri, 24 Apr 2020 11:19:02 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 24 Apr 2020 11:19:59 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Apr 2020 11:20:10 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 24 Apr 2020 11:20:17 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 24 Apr 2020 11:20:19 GMT
VOLUME [/opt/bonita]
# Fri, 24 Apr 2020 11:20:21 GMT
COPY dir:6d2b12bd97418487ddd1a174f34d85d11b3e6487e01e6d3f80d99fffcff78e82 in /opt/files 
# Fri, 24 Apr 2020 11:20:23 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 24 Apr 2020 11:20:25 GMT
EXPOSE 8080
# Fri, 24 Apr 2020 11:20:29 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:beed3bd0a281cacead564771f079ed9ee8b272a2ed0e28f533e188f3d21fee6e`  
		Last Modified: Mon, 06 Apr 2020 15:40:20 GMT  
		Size: 30.4 MB (30400298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14d2411b83450b8afe92058b998540c56ec42f1ddd7581e8e9fe629c442f89`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82678240be3a5c783512ff7336f2b10837ae126958bc6bd1b476a8d039c08771`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7307ad4f24078fd763b41ec7c1772f2fd5238fed1bae36c5d42d28ec9adbffb9`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96de0feba41ae36c2f30772848962f761fa86bea2d5b169395a3bc3c7132e49`  
		Last Modified: Fri, 24 Apr 2020 11:21:16 GMT  
		Size: 94.9 MB (94877414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303b05a46843da9faa969b2426e50688c52e4265f8d3a8d36e56295bafc2ef6d`  
		Last Modified: Fri, 24 Apr 2020 11:20:58 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cb31d4b93a32f72177ac1374e4fa0804d31b6ac40854dd644fbd53a4a6512e`  
		Last Modified: Fri, 24 Apr 2020 11:20:54 GMT  
		Size: 1.9 KB (1920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b95753237ab572b5fc1131a7c1680219f4a1946af444435a1aff47d35e5eef`  
		Last Modified: Fri, 24 Apr 2020 11:20:54 GMT  
		Size: 541.6 KB (541554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8828b620936bffe307201eada6d468ac9b080f513f12937c5bbf4c0f5a79f14`  
		Last Modified: Fri, 24 Apr 2020 11:21:36 GMT  
		Size: 97.9 MB (97894347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00099f3eb606359b7a2365add166dfb5e6d395de29ca02390c32f24c9a0a977e`  
		Last Modified: Fri, 24 Apr 2020 11:21:29 GMT  
		Size: 7.6 KB (7623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d127f5d545caa1e2928e4980c55cf550ad7fec5e131ed9475f0bd698a72ec9c6`  
		Last Modified: Fri, 24 Apr 2020 11:21:29 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
