## `bonita:latest`

```console
$ docker pull bonita@sha256:f4c61e1ee86288a35d740cd1f994e843e8bdac6b39486b0ba65723bd9c3bb2a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:66d3e00c95c0c3dab8936204ce662968b51b7d56672c90d6a48753fe9a1a686a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237704991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b939a09fc953aed22622e28f3df4bd51be0e7818d41c5d973d9f97a602742835`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 07:38:40 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 21 Jan 2021 07:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 07:39:07 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 21 Jan 2021 07:39:08 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 21 Jan 2021 07:39:10 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 21 Jan 2021 07:39:10 GMT
ARG BONITA_VERSION
# Sat, 30 Jan 2021 01:35:45 GMT
ARG BRANDING_VERSION
# Sat, 30 Jan 2021 01:35:45 GMT
ARG BONITA_SHA256
# Sat, 30 Jan 2021 01:35:45 GMT
ARG BASE_URL
# Sat, 30 Jan 2021 01:35:45 GMT
ARG BONITA_URL
# Sat, 30 Jan 2021 01:35:46 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 30 Jan 2021 01:35:46 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 30 Jan 2021 01:35:46 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 30 Jan 2021 01:35:46 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 30 Jan 2021 01:35:46 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 30 Jan 2021 01:35:46 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 30 Jan 2021 01:35:48 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 30 Jan 2021 01:35:49 GMT
RUN mkdir /opt/files
# Sat, 30 Jan 2021 01:35:49 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 30 Jan 2021 01:35:52 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 30 Jan 2021 01:35:54 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 30 Jan 2021 01:35:56 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 30 Jan 2021 01:35:56 GMT
VOLUME [/opt/bonita]
# Sat, 30 Jan 2021 01:35:56 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 30 Jan 2021 01:35:56 GMT
EXPOSE 8080
# Sat, 30 Jan 2021 01:35:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46385fcca4697a1a6527be5be3b68441d5fa10fbd48fef7b76e39ca1263dc0b`  
		Last Modified: Thu, 21 Jan 2021 07:40:38 GMT  
		Size: 94.0 MB (93995767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d1917917e03a4d22cef4293a47535b3abf9cede0d6f7dd800d5909c45cc8d8`  
		Last Modified: Thu, 21 Jan 2021 07:40:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbbc0202f4806d0e2be4fbebabc128e61cd8ba45f63822418761157a7a8feed`  
		Last Modified: Thu, 21 Jan 2021 07:40:22 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13152e81156a493fa0acd51cf3e109ce2f731035592fef35dc16d512acc65ce2`  
		Last Modified: Thu, 21 Jan 2021 07:40:21 GMT  
		Size: 572.4 KB (572373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e438747c4ef1353981e4b748014b794907749c030be0b776079f7cfd588818e`  
		Last Modified: Sat, 30 Jan 2021 01:36:12 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fec74b585a3d36ce52e78fd3b8fff37743acab5dfebb1e9cd259c607a9ea64`  
		Last Modified: Sat, 30 Jan 2021 01:36:12 GMT  
		Size: 6.9 KB (6917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5e31010d670d2142f2fb7544aa316b486d421b8cb05c90dd05408312cc60d3`  
		Last Modified: Sat, 30 Jan 2021 01:36:18 GMT  
		Size: 116.4 MB (116415406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d985d5cd6ad402371bdc42d94841e8a0ae9f2c3bfcf38bade2767ef1dbedda`  
		Last Modified: Sat, 30 Jan 2021 01:36:13 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:042b27c155776c49fa827a611e68600e3ab7616ae5be3bbe45c57e5f8c41a4d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.0 MB (225999606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1473c8d2979e05f1c6fe37e1c2ef0c1c3f0d01b1d9b043222c585bd2f204ea03`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:28:20 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 21 Jan 2021 05:29:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:29:09 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 21 Jan 2021 05:29:11 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 21 Jan 2021 05:29:13 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 21 Jan 2021 05:29:14 GMT
ARG BONITA_VERSION
# Sat, 30 Jan 2021 00:53:50 GMT
ARG BRANDING_VERSION
# Sat, 30 Jan 2021 00:53:50 GMT
ARG BONITA_SHA256
# Sat, 30 Jan 2021 00:53:51 GMT
ARG BASE_URL
# Sat, 30 Jan 2021 00:53:51 GMT
ARG BONITA_URL
# Sat, 30 Jan 2021 00:53:52 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 30 Jan 2021 00:53:53 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 30 Jan 2021 00:53:53 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 30 Jan 2021 00:53:54 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 30 Jan 2021 00:53:54 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 30 Jan 2021 00:53:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 30 Jan 2021 00:53:57 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 30 Jan 2021 00:53:59 GMT
RUN mkdir /opt/files
# Sat, 30 Jan 2021 00:54:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 30 Jan 2021 00:54:06 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 30 Jan 2021 00:54:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 30 Jan 2021 00:54:11 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 30 Jan 2021 00:54:12 GMT
VOLUME [/opt/bonita]
# Sat, 30 Jan 2021 00:54:12 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 30 Jan 2021 00:54:13 GMT
EXPOSE 8080
# Sat, 30 Jan 2021 00:54:14 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8df92044c4b506076de6abc24afe1d5eac83a9e6cc5fb97a725daea7b5fb742`  
		Last Modified: Thu, 21 Jan 2021 05:31:28 GMT  
		Size: 85.3 MB (85297873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1abc3fcd55457d935f9da38456f79f5f4c394ff39f5f0bf92deb550a9c5d5a8`  
		Last Modified: Thu, 21 Jan 2021 05:31:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17a62d1dc9db97a189188b6263b79601d869b5f3813597d9c9990e9b1e67b0`  
		Last Modified: Thu, 21 Jan 2021 05:31:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af2268a1d88611b9add2dc44af567d1d121e316d036e49cbd1b3f54717c4019`  
		Last Modified: Thu, 21 Jan 2021 05:31:03 GMT  
		Size: 541.8 KB (541813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a6d9f507c165d2c3713ddc71f40686f7efab71e36563b00a38df6544f734a9`  
		Last Modified: Sat, 30 Jan 2021 00:54:31 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96b3ed213aa787365c4954d6c9d9f0f6339011bb25c1da83b930936e897408f`  
		Last Modified: Sat, 30 Jan 2021 00:54:31 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d407eacd2633e2d566bbdbc12ca4a0bfb1598bc401e81b0c7b2ac5789018614c`  
		Last Modified: Sat, 30 Jan 2021 00:54:41 GMT  
		Size: 116.4 MB (116415398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8263bbe0ad9c06ee5e05b8540e8b539f69ce8f36cd16c611f40d2a27977da5`  
		Last Modified: Sat, 30 Jan 2021 00:54:31 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:7cbc79ac9276eeb9ed45b37e7460eb8b82cd17ee65bf79366743255784a8fed5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.3 MB (233308791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2deb92cacf66527c2fdde8cdd3931695079b54e53a5882fc939be196f3fc36c`
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
# Sat, 30 Jan 2021 01:47:09 GMT
ARG BRANDING_VERSION
# Sat, 30 Jan 2021 01:47:17 GMT
ARG BONITA_SHA256
# Sat, 30 Jan 2021 01:47:23 GMT
ARG BASE_URL
# Sat, 30 Jan 2021 01:47:32 GMT
ARG BONITA_URL
# Sat, 30 Jan 2021 01:47:38 GMT
ENV BONITA_VERSION=7.12.1
# Sat, 30 Jan 2021 01:47:46 GMT
ENV BRANDING_VERSION=2021.1
# Sat, 30 Jan 2021 01:48:02 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Sat, 30 Jan 2021 01:48:07 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Sat, 30 Jan 2021 01:48:11 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Sat, 30 Jan 2021 01:48:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Sat, 30 Jan 2021 01:48:30 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Sat, 30 Jan 2021 01:48:55 GMT
RUN mkdir /opt/files
# Sat, 30 Jan 2021 01:48:59 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Sat, 30 Jan 2021 01:49:27 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Sat, 30 Jan 2021 01:49:41 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Sat, 30 Jan 2021 01:49:52 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Sat, 30 Jan 2021 01:49:57 GMT
VOLUME [/opt/bonita]
# Sat, 30 Jan 2021 01:50:00 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Sat, 30 Jan 2021 01:50:08 GMT
EXPOSE 8080
# Sat, 30 Jan 2021 01:50:13 GMT
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
	-	`sha256:3328d3e249051dfe4783d885b91ec5874d8d654b2c198cc6e62b5eee230942bf`  
		Last Modified: Sat, 30 Jan 2021 01:50:42 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0341326e395d84e7152c652f6370e970564a985e74835fe94d52123709c5ae13`  
		Last Modified: Sat, 30 Jan 2021 01:50:42 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b610564454d7cbfa5e7c6d19b44df37a3ff995fc38607f6154903eb2fde0914`  
		Last Modified: Sat, 30 Jan 2021 01:50:52 GMT  
		Size: 116.4 MB (116415407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06136d8ff274d12b9e1962bd89095c8930d5f735cb50f3942ae371b5128ff1af`  
		Last Modified: Sat, 30 Jan 2021 01:50:43 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
