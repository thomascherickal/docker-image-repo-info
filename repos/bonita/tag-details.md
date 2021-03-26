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
$ docker pull bonita@sha256:252b0188a02ffaef870ffece068c173564a5e2efeef27b48389526c247d69656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:2021.1` - linux; amd64

```console
$ docker pull bonita@sha256:bec7c62bfa26447c37ea9a71f638671f52400db14f9229eeee8e7df6a6a299b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238893974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce2c8eced3ba09353d4f974632f31ecce2489fc06865b589740531b2abbd1d3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:54:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 26 Mar 2021 09:54:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:54:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:54:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BRANDING_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 26 Mar 2021 09:54:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 26 Mar 2021 09:55:00 GMT
RUN mkdir /opt/files
# Fri, 26 Mar 2021 09:55:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 26 Mar 2021 09:55:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 26 Mar 2021 09:55:07 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 26 Mar 2021 09:55:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 26 Mar 2021 09:55:09 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:55:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 26 Mar 2021 09:55:09 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:55:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e534248c77c94586396089f5fe1e6ef3445619f3b25b01e3788c31a39246de`  
		Last Modified: Fri, 26 Mar 2021 09:56:17 GMT  
		Size: 95.2 MB (95182928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51fffa5c2969e00e61b80759c01c7b29a445487471b69cab746c2912685b51`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0795bb218aad676992e4855a54a7a8fbf0139bdb13b12a54e94c512da7714`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef20992b153c738c647dc0b493b155dc50a750365be70fcf88cfe88ce28b63d`  
		Last Modified: Fri, 26 Mar 2021 09:56:00 GMT  
		Size: 573.0 KB (572988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab13c0cfd407a99af4475a201b0e82ef59eb70270e887c1d76519a390f6df46`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fef7e4f41959abb0200ce52dbf1df79a3a1c6e2135817fa0b950601145d24a`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa40d92e0791bad639df8e2c95739cc01e6fc08a1c47bac8675668516852dba`  
		Last Modified: Fri, 26 Mar 2021 09:56:37 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dbd4b7563e31dcb93c41f4ddce6c2216761188046dc480a97cd1199207e72`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:214a951cf59a227aa245a53af6280fe9480bc2e429c293439717957bd24b0e84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226971792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30040d57cf072ea3506cc843473269c0fb303942ea3b5fbcd38121e86942f10d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:55:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 04:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:56:18 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:56:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:56:24 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:57:05 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 04:57:06 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:57:08 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 04:57:09 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 04:57:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 04:57:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 04:57:18 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 04:57:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 04:57:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 04:57:27 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 04:57:30 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 04:57:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:57:32 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 04:57:33 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:57:33 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c83eec9a08ca31b0967928280b24307ee3da07363b8b020fbcb8ef55e84f33c`  
		Last Modified: Thu, 04 Mar 2021 04:58:43 GMT  
		Size: 86.3 MB (86270625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51117579b7f1169aaeab24891e96baf3415884368d15c152a65af49d5cfe9d1e`  
		Last Modified: Thu, 04 Mar 2021 04:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3cac34d3604f9625bfd3599da48dcf450e69ef5fb5de231c031f012054b70`  
		Last Modified: Thu, 04 Mar 2021 04:58:24 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dafedb36e501fe29a3e4e4324415ccddc0dc0e435bf8b824d7fbc309e79706`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 541.8 KB (541823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8100ff6f916893fb3924689e93c9c3e2859d0ffd4bec28e0b1284443372e4546`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484e759bc1c1ec7509a26f4c7878c04074c5958ac5336be202beb41500d2eed8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b9e7d444fb6ada0affc11160806862ee09e60b2fa7893b2d79e8ef49b9c3e`  
		Last Modified: Thu, 04 Mar 2021 04:58:59 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037423ea62eef570b500fcddd4ee54bb39817bdef407c218d6bc612b50a881e8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:2021.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:fa8da3b85935ea08dccb0e33f371c55ff6eb77fa3b848079f619b92e3f4ce1d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234577335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e9fc3702494f2ccec59668d5597b8ac6f2de2580fff1064b1086c9ad83f99ff`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:45:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 05:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:52:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:52:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:52:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:53:07 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:56:20 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 05:56:34 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:56:45 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:56:56 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:57:14 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 05:57:22 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 05:57:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 05:57:37 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:57:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:57:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:58:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 05:58:29 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 05:58:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 05:58:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 05:59:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 05:59:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 05:59:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:59:37 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 05:59:41 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:59:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5e22014470e3a0e33866d21001d1a638200e5d56c24c202f909de087a56bba`  
		Last Modified: Thu, 04 Mar 2021 06:01:39 GMT  
		Size: 87.2 MB (87187404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc56e644a17ce5a16b1fbcf26423ce252b5449b7aa9676ae35fa15de72babc0`  
		Last Modified: Thu, 04 Mar 2021 06:01:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08478a27e00e84d03e0711f150ecb392e9d57a85e568caabc250c0bc8214c7`  
		Last Modified: Thu, 04 Mar 2021 06:01:22 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3fab24756c5027d0b09cf6985b200d62c2ae0691ab4e19343babaf0756e71d`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 541.5 KB (541535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dfcc00939b4b6da9eb8e590933846fb345ccec05d50aa2a94e128e5d980e7c`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68b66bcb708201a8b22b6d73394f5b3850ae756f17e04a1bc44bcfa7d68751`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc5702d8d451399c87cff54266b5b9be4d3d70d34fa990e23c0a90c99f659a`  
		Last Modified: Thu, 04 Mar 2021 06:02:01 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef8e80ee863e5edc79546f700ae8d966adc43c717ed117518a4e66b78357070`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10`

```console
$ docker pull bonita@sha256:a3b426b66a0919dacf6b9008afff51121382224a25b9ce27244ff567ce6b4b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10` - linux; amd64

```console
$ docker pull bonita@sha256:68c1b07825e2b49ec7e2f5d09d0bb9cb1124dd5cd413e04990f43769902a6742
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.0 MB (243983655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b247e4e0e753c3f92e346681550706afe418876d318ef882dfd1e7c6a2c9956`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:52:33 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 26 Mar 2021 09:53:56 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:53:57 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:53:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:00 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:01 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 26 Mar 2021 09:54:01 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 26 Mar 2021 09:54:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 26 Mar 2021 09:54:03 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 26 Mar 2021 09:54:06 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 26 Mar 2021 09:54:08 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 26 Mar 2021 09:54:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 26 Mar 2021 09:54:09 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:54:10 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 26 Mar 2021 09:54:10 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 26 Mar 2021 09:54:10 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:54:10 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758aa4bda331f1a79eeaa9ef209ea761536760099648e00edb1dc97da5cbab99`  
		Last Modified: Fri, 26 Mar 2021 09:55:45 GMT  
		Size: 118.7 MB (118713514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0288caa263e5157f91590e85aaf9bc0137e0a6b9cc17c40fea8e82bf7a8026`  
		Last Modified: Fri, 26 Mar 2021 09:55:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e783d95bec0ad604e56da21bd7a41ff9e8e5eec5154dc13ce6136a5cddb491ff`  
		Last Modified: Fri, 26 Mar 2021 09:55:26 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ac2c18c4374d15acff76cd5f82ef507fec3cd3843175a5d5a34c42eca5d839`  
		Last Modified: Fri, 26 Mar 2021 09:55:27 GMT  
		Size: 573.0 KB (572991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cccb95ba60806e8bd9f1abd297ea7c30e082e5d40416583f8f1fb7a4452986`  
		Last Modified: Fri, 26 Mar 2021 09:55:30 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d07ada1cef794cb91ebc12c7b9e8c144b323aa8b2607160f2341bea2648b96`  
		Last Modified: Fri, 26 Mar 2021 09:55:25 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5427824d2e3e2398968d0bdcdcc2b7a9d23bbe2b9e61bcfe2e8c6a587d9e8898`  
		Last Modified: Fri, 26 Mar 2021 09:55:27 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5970b135dc1801e779699365e7c1f7268fe5c857d99e1bcbb1d6485474840865
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231689713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e943b37d9d51b54e051b95c114f44b407bce3349c70fbbc61a913fe10ac2268e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:53:43 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 04 Mar 2021 04:54:45 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:54:50 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:54:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:54:56 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:54:57 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:54:58 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:54:58 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:54:59 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:55:00 GMT
ENV BONITA_VERSION=7.10.6
# Thu, 04 Mar 2021 04:55:00 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Thu, 04 Mar 2021 04:55:01 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:55:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Thu, 04 Mar 2021 04:55:04 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 04 Mar 2021 04:55:07 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 04:55:10 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 04:55:13 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 04 Mar 2021 04:55:13 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:55:14 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Thu, 04 Mar 2021 04:55:15 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 04 Mar 2021 04:55:16 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:55:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e48c339cd25e9d07ab867281bafcc478d369888383aa9dc0c3776027e79070`  
		Last Modified: Thu, 04 Mar 2021 04:58:15 GMT  
		Size: 109.4 MB (109429477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596ff443a0163f00202e670a28f453fac0c35685fa61521a6cf9d0de926db35`  
		Last Modified: Thu, 04 Mar 2021 04:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7ebc0fa1a20384945073e2cf4745fc38b7afe333744ca110da53d3e805eb94`  
		Last Modified: Thu, 04 Mar 2021 04:57:49 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76dc240b10b7ef3f54a61c0e63a7db7ab706cba58a6c8e2ddeb25e2d5fa2f8d`  
		Last Modified: Thu, 04 Mar 2021 04:57:50 GMT  
		Size: 541.8 KB (541808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07f519aeb84b8094289cdcf5e668c684db6c69ecd0af4464722e674655a24c8`  
		Last Modified: Thu, 04 Mar 2021 04:57:57 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12f76eb31419bd45909ff32b3fe4c64426e5a30ecae8addf2eaec6586259af8`  
		Last Modified: Thu, 04 Mar 2021 04:57:49 GMT  
		Size: 7.7 KB (7655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff722f43773e24f08dfe195f463fa4b3e45487ddba3e7776638c1a35f7bc33f`  
		Last Modified: Thu, 04 Mar 2021 04:57:49 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10` - linux; ppc64le

```console
$ docker pull bonita@sha256:daea60cdb58db57e00d9dd342ea58c3e415c2aa75aefbeec935690d512200d12
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241065369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b455cf56680d1e8421a76197d4ab63c0441c3f245880db462398127708018b5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:33:00 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 04 Mar 2021 05:42:17 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:42:38 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:42:55 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:43:14 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:43:18 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:43:23 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:43:32 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:43:41 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:43:49 GMT
ENV BONITA_VERSION=7.10.6
# Thu, 04 Mar 2021 05:43:56 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Thu, 04 Mar 2021 05:44:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:44:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Thu, 04 Mar 2021 05:44:20 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 04 Mar 2021 05:44:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 05:44:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 05:45:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 04 Mar 2021 05:45:12 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:45:16 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Thu, 04 Mar 2021 05:45:22 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 04 Mar 2021 05:45:30 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:45:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202c876494bbd25aa8f2cf7f292408c939394af69801683159e0c8edebbc3a2`  
		Last Modified: Thu, 04 Mar 2021 06:01:07 GMT  
		Size: 112.1 MB (112116337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c859aeb4f38230b401800fa96a6cd8ade57386a890ec6b3341a277afa466820c`  
		Last Modified: Thu, 04 Mar 2021 06:00:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e0a0f6fc0653289b986397af9f66a9b38e32c24d926f823d254e8ad87f3b8c`  
		Last Modified: Thu, 04 Mar 2021 06:00:40 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6a7813c055f4d51ae63652be4a4400243f34f97991f91fda968542e451ad37`  
		Last Modified: Thu, 04 Mar 2021 06:00:40 GMT  
		Size: 541.6 KB (541552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100f151d422e6528159ee98fd51a983e76eb90e5cc7a699ba485916711e9ab28`  
		Last Modified: Thu, 04 Mar 2021 06:00:48 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907be0e52daf4733660784fa362da2e3f4e0b7917bfcb82d600383af23373b1f`  
		Last Modified: Thu, 04 Mar 2021 06:00:40 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296feabd4cf698dfaacfdbccb99bbcf8efc63ca2840cb0f0e4a6f0da6c606d31`  
		Last Modified: Thu, 04 Mar 2021 06:00:39 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.10.6`

```console
$ docker pull bonita@sha256:a3b426b66a0919dacf6b9008afff51121382224a25b9ce27244ff567ce6b4b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.10.6` - linux; amd64

```console
$ docker pull bonita@sha256:68c1b07825e2b49ec7e2f5d09d0bb9cb1124dd5cd413e04990f43769902a6742
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.0 MB (243983655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b247e4e0e753c3f92e346681550706afe418876d318ef882dfd1e7c6a2c9956`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:52:33 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Fri, 26 Mar 2021 09:53:56 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:53:57 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:53:58 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:00 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:01 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:01 GMT
ENV BONITA_VERSION=7.10.6
# Fri, 26 Mar 2021 09:54:01 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Fri, 26 Mar 2021 09:54:02 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Fri, 26 Mar 2021 09:54:03 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Fri, 26 Mar 2021 09:54:06 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 26 Mar 2021 09:54:08 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Fri, 26 Mar 2021 09:54:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Fri, 26 Mar 2021 09:54:09 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:54:10 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Fri, 26 Mar 2021 09:54:10 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Fri, 26 Mar 2021 09:54:10 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:54:10 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758aa4bda331f1a79eeaa9ef209ea761536760099648e00edb1dc97da5cbab99`  
		Last Modified: Fri, 26 Mar 2021 09:55:45 GMT  
		Size: 118.7 MB (118713514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0288caa263e5157f91590e85aaf9bc0137e0a6b9cc17c40fea8e82bf7a8026`  
		Last Modified: Fri, 26 Mar 2021 09:55:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e783d95bec0ad604e56da21bd7a41ff9e8e5eec5154dc13ce6136a5cddb491ff`  
		Last Modified: Fri, 26 Mar 2021 09:55:26 GMT  
		Size: 1.9 KB (1909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ac2c18c4374d15acff76cd5f82ef507fec3cd3843175a5d5a34c42eca5d839`  
		Last Modified: Fri, 26 Mar 2021 09:55:27 GMT  
		Size: 573.0 KB (572991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cccb95ba60806e8bd9f1abd297ea7c30e082e5d40416583f8f1fb7a4452986`  
		Last Modified: Fri, 26 Mar 2021 09:55:30 GMT  
		Size: 98.0 MB (97973960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d07ada1cef794cb91ebc12c7b9e8c144b323aa8b2607160f2341bea2648b96`  
		Last Modified: Fri, 26 Mar 2021 09:55:25 GMT  
		Size: 7.7 KB (7654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5427824d2e3e2398968d0bdcdcc2b7a9d23bbe2b9e61bcfe2e8c6a587d9e8898`  
		Last Modified: Fri, 26 Mar 2021 09:55:27 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:5970b135dc1801e779699365e7c1f7268fe5c857d99e1bcbb1d6485474840865
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231689713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e943b37d9d51b54e051b95c114f44b407bce3349c70fbbc61a913fe10ac2268e`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:53:43 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 04 Mar 2021 04:54:45 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:54:50 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:54:53 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:54:56 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:54:57 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:54:58 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:54:58 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:54:59 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:55:00 GMT
ENV BONITA_VERSION=7.10.6
# Thu, 04 Mar 2021 04:55:00 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Thu, 04 Mar 2021 04:55:01 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:55:02 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Thu, 04 Mar 2021 04:55:04 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 04 Mar 2021 04:55:07 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 04:55:10 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 04:55:13 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 04 Mar 2021 04:55:13 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:55:14 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Thu, 04 Mar 2021 04:55:15 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 04 Mar 2021 04:55:16 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:55:17 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e48c339cd25e9d07ab867281bafcc478d369888383aa9dc0c3776027e79070`  
		Last Modified: Thu, 04 Mar 2021 04:58:15 GMT  
		Size: 109.4 MB (109429477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596ff443a0163f00202e670a28f453fac0c35685fa61521a6cf9d0de926db35`  
		Last Modified: Thu, 04 Mar 2021 04:57:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7ebc0fa1a20384945073e2cf4745fc38b7afe333744ca110da53d3e805eb94`  
		Last Modified: Thu, 04 Mar 2021 04:57:49 GMT  
		Size: 1.9 KB (1918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76dc240b10b7ef3f54a61c0e63a7db7ab706cba58a6c8e2ddeb25e2d5fa2f8d`  
		Last Modified: Thu, 04 Mar 2021 04:57:50 GMT  
		Size: 541.8 KB (541808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07f519aeb84b8094289cdcf5e668c684db6c69ecd0af4464722e674655a24c8`  
		Last Modified: Thu, 04 Mar 2021 04:57:57 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12f76eb31419bd45909ff32b3fe4c64426e5a30ecae8addf2eaec6586259af8`  
		Last Modified: Thu, 04 Mar 2021 04:57:49 GMT  
		Size: 7.7 KB (7655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff722f43773e24f08dfe195f463fa4b3e45487ddba3e7776638c1a35f7bc33f`  
		Last Modified: Thu, 04 Mar 2021 04:57:49 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.10.6` - linux; ppc64le

```console
$ docker pull bonita@sha256:daea60cdb58db57e00d9dd342ea58c3e415c2aa75aefbeec935690d512200d12
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241065369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b455cf56680d1e8421a76197d4ab63c0441c3f245880db462398127708018b5`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:33:00 GMT
MAINTAINER Jérémy Jacquier-Roux <jeremy.jacquier-roux@bonitasoft.org>
# Thu, 04 Mar 2021 05:42:17 GMT
RUN apt-get update && apt-get install -y   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:42:38 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:42:55 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:43:14 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:43:18 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:43:23 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:43:32 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:43:41 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:43:49 GMT
ENV BONITA_VERSION=7.10.6
# Thu, 04 Mar 2021 05:43:56 GMT
ENV BONITA_SHA256=aaf61a044e7a8d9ec95d2b5d0c315a6d01d9c93ba01d753fcb008e2cfbbb725f
# Thu, 04 Mar 2021 05:44:00 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:44:06 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.10.6/BonitaCommunity-7.10.6.zip
# Thu, 04 Mar 2021 05:44:20 GMT
RUN echo "Downloading Bonita from url: $BONITA_URL"
# Thu, 04 Mar 2021 05:44:36 GMT
RUN mkdir /opt/files   && curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 05:44:55 GMT
RUN sha256sum /opt/files/BonitaCommunity-${BONITA_VERSION}.zip
# Thu, 04 Mar 2021 05:45:08 GMT
RUN echo "$BONITA_SHA256" /opt/files/BonitaCommunity-${BONITA_VERSION}.zip | sha256sum -c -
# Thu, 04 Mar 2021 05:45:12 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:45:16 GMT
COPY dir:46816633cc37ba9fd23af260c8c2384c15f3b4385b5752d6b42577967959f7f0 in /opt/files 
# Thu, 04 Mar 2021 05:45:22 GMT
COPY dir:157c135edc1215565cc6815861e1a1728bdf09f6cfceca03c1639b2262f1cd65 in /opt/templates 
# Thu, 04 Mar 2021 05:45:30 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:45:36 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202c876494bbd25aa8f2cf7f292408c939394af69801683159e0c8edebbc3a2`  
		Last Modified: Thu, 04 Mar 2021 06:01:07 GMT  
		Size: 112.1 MB (112116337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c859aeb4f38230b401800fa96a6cd8ade57386a890ec6b3341a277afa466820c`  
		Last Modified: Thu, 04 Mar 2021 06:00:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e0a0f6fc0653289b986397af9f66a9b38e32c24d926f823d254e8ad87f3b8c`  
		Last Modified: Thu, 04 Mar 2021 06:00:40 GMT  
		Size: 1.9 KB (1916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6a7813c055f4d51ae63652be4a4400243f34f97991f91fda968542e451ad37`  
		Last Modified: Thu, 04 Mar 2021 06:00:40 GMT  
		Size: 541.6 KB (541552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100f151d422e6528159ee98fd51a983e76eb90e5cc7a699ba485916711e9ab28`  
		Last Modified: Thu, 04 Mar 2021 06:00:48 GMT  
		Size: 98.0 MB (97973956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907be0e52daf4733660784fa362da2e3f4e0b7917bfcb82d600383af23373b1f`  
		Last Modified: Thu, 04 Mar 2021 06:00:40 GMT  
		Size: 7.7 KB (7653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296feabd4cf698dfaacfdbccb99bbcf8efc63ca2840cb0f0e4a6f0da6c606d31`  
		Last Modified: Thu, 04 Mar 2021 06:00:39 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11`

```console
$ docker pull bonita@sha256:0a27616c580c01e34fdc8c4bcd9304f83d2b69ad156de00f0af5d095d3e59775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11` - linux; amd64

```console
$ docker pull bonita@sha256:b694e19ef9ac650a23887d2c22c36276b9f48993eed040886e30b147c9b88ea8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235826347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd1d641447e311f7e0cd7a0dd4672a56e5d7c6d2a49334a909ee29f9f41cf6fd`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:54:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 26 Mar 2021 09:54:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:54:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:54:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 26 Mar 2021 09:54:39 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 26 Mar 2021 09:54:40 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 26 Mar 2021 09:54:41 GMT
RUN mkdir /opt/files
# Fri, 26 Mar 2021 09:54:41 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 26 Mar 2021 09:54:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 26 Mar 2021 09:54:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 26 Mar 2021 09:54:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 26 Mar 2021 09:54:51 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:54:51 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 26 Mar 2021 09:54:51 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:54:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e534248c77c94586396089f5fe1e6ef3445619f3b25b01e3788c31a39246de`  
		Last Modified: Fri, 26 Mar 2021 09:56:17 GMT  
		Size: 95.2 MB (95182928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51fffa5c2969e00e61b80759c01c7b29a445487471b69cab746c2912685b51`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0795bb218aad676992e4855a54a7a8fbf0139bdb13b12a54e94c512da7714`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef20992b153c738c647dc0b493b155dc50a750365be70fcf88cfe88ce28b63d`  
		Last Modified: Fri, 26 Mar 2021 09:56:00 GMT  
		Size: 573.0 KB (572988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342ed4cdb3bb862f5ee7bebbc9876f88377e7143203e1d9356aa2ad597373dc`  
		Last Modified: Fri, 26 Mar 2021 09:55:59 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ade80e567ac70f7da85f2303331a1637cb679e23c1c02fcd30ad8b60fc5ea`  
		Last Modified: Fri, 26 Mar 2021 09:55:59 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e4b5d9808791fa19090b61806ed17ea0c9fdc6a9d0f96f815830d9fe297251`  
		Last Modified: Fri, 26 Mar 2021 09:56:05 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfb68eeef2f54c5a0c542b65ba7fc90440c48b38740396b882c0e8d356613cb`  
		Last Modified: Fri, 26 Mar 2021 09:55:59 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9dd42508841a3f375aa5b3f0e5ead7062c14801929b7f9a8ff9a61ed93b6d4d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223904167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f5ad9ead0abb0e0d18b019ac669921f0176098d64537311a3cca8a9daf077c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:55:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 04:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:56:18 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:56:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:56:24 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:56:25 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:56:26 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:56:26 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:56:28 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 04 Mar 2021 04:56:29 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 04 Mar 2021 04:56:30 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 04:56:31 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:56:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 04:56:35 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 04:56:38 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 04:56:39 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 04 Mar 2021 04:56:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 04 Mar 2021 04:56:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 04:56:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 04:56:52 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:56:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 04:56:55 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:56:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c83eec9a08ca31b0967928280b24307ee3da07363b8b020fbcb8ef55e84f33c`  
		Last Modified: Thu, 04 Mar 2021 04:58:43 GMT  
		Size: 86.3 MB (86270625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51117579b7f1169aaeab24891e96baf3415884368d15c152a65af49d5cfe9d1e`  
		Last Modified: Thu, 04 Mar 2021 04:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3cac34d3604f9625bfd3599da48dcf450e69ef5fb5de231c031f012054b70`  
		Last Modified: Thu, 04 Mar 2021 04:58:24 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dafedb36e501fe29a3e4e4324415ccddc0dc0e435bf8b824d7fbc309e79706`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 541.8 KB (541823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a0f24e4821dbf50388ccf9152b4ed68b3360f8159203b309deba312c5e1623`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e898cc1ff802d14e5898a7ac295792ad446d2fa47415fb68420a838a1dbbea37`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb143758b6d8efaa13a38b2238d171ed6b10ea027a51a5d28a894e7e67469a5`  
		Last Modified: Thu, 04 Mar 2021 04:58:30 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9b616f8ca880f366a3d637dc18321caf7bce6a8cb0953fb6b738ad5640d9d0`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11` - linux; ppc64le

```console
$ docker pull bonita@sha256:6d482e1a9e8ff6bcf053de4feefff6b644e7e03630b827a036e8f8fe591300e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a625fc56f0ed882580a1ec29e73430e366ea09bc32f6557f0676815d940d6b52`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:45:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 05:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:52:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:52:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:52:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:53:07 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:53:13 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:53:20 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:53:26 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:53:30 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 04 Mar 2021 05:53:35 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 04 Mar 2021 05:53:41 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 05:53:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:54:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 05:54:13 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 05:54:28 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 05:54:30 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 04 Mar 2021 05:54:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 04 Mar 2021 05:55:06 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 05:55:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 05:55:41 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:55:44 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 05:55:51 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:55:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5e22014470e3a0e33866d21001d1a638200e5d56c24c202f909de087a56bba`  
		Last Modified: Thu, 04 Mar 2021 06:01:39 GMT  
		Size: 87.2 MB (87187404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc56e644a17ce5a16b1fbcf26423ce252b5449b7aa9676ae35fa15de72babc0`  
		Last Modified: Thu, 04 Mar 2021 06:01:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08478a27e00e84d03e0711f150ecb392e9d57a85e568caabc250c0bc8214c7`  
		Last Modified: Thu, 04 Mar 2021 06:01:22 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3fab24756c5027d0b09cf6985b200d62c2ae0691ab4e19343babaf0756e71d`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 541.5 KB (541535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be368ca743dd0541c18b70c7fd4be07819f41e1ab9ae9a1420eb536fac8cab70`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef65ab37b2f073afda64c74705cc91f699e4153157280b65df4d491bce857bf7`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175ee2d9d2d1ce7c2340e0a64e4ff6affb367c20d584a7b46a5a1f96a88ae6a`  
		Last Modified: Thu, 04 Mar 2021 06:01:28 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48edf254570016c0c9f66ff82f313675125d6073386dee64443bc95ec89f4a`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.11.4`

```console
$ docker pull bonita@sha256:0a27616c580c01e34fdc8c4bcd9304f83d2b69ad156de00f0af5d095d3e59775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.11.4` - linux; amd64

```console
$ docker pull bonita@sha256:b694e19ef9ac650a23887d2c22c36276b9f48993eed040886e30b147c9b88ea8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.8 MB (235826347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd1d641447e311f7e0cd7a0dd4672a56e5d7c6d2a49334a909ee29f9f41cf6fd`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:54:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 26 Mar 2021 09:54:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:54:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:54:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BONITA_VERSION=7.11.4
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Fri, 26 Mar 2021 09:54:39 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:39 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Fri, 26 Mar 2021 09:54:40 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 26 Mar 2021 09:54:41 GMT
RUN mkdir /opt/files
# Fri, 26 Mar 2021 09:54:41 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Fri, 26 Mar 2021 09:54:47 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Fri, 26 Mar 2021 09:54:49 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 26 Mar 2021 09:54:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 26 Mar 2021 09:54:51 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:54:51 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 26 Mar 2021 09:54:51 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:54:51 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e534248c77c94586396089f5fe1e6ef3445619f3b25b01e3788c31a39246de`  
		Last Modified: Fri, 26 Mar 2021 09:56:17 GMT  
		Size: 95.2 MB (95182928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51fffa5c2969e00e61b80759c01c7b29a445487471b69cab746c2912685b51`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0795bb218aad676992e4855a54a7a8fbf0139bdb13b12a54e94c512da7714`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef20992b153c738c647dc0b493b155dc50a750365be70fcf88cfe88ce28b63d`  
		Last Modified: Fri, 26 Mar 2021 09:56:00 GMT  
		Size: 573.0 KB (572988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342ed4cdb3bb862f5ee7bebbc9876f88377e7143203e1d9356aa2ad597373dc`  
		Last Modified: Fri, 26 Mar 2021 09:55:59 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8ade80e567ac70f7da85f2303331a1637cb679e23c1c02fcd30ad8b60fc5ea`  
		Last Modified: Fri, 26 Mar 2021 09:55:59 GMT  
		Size: 6.9 KB (6891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e4b5d9808791fa19090b61806ed17ea0c9fdc6a9d0f96f815830d9fe297251`  
		Last Modified: Fri, 26 Mar 2021 09:56:05 GMT  
		Size: 113.3 MB (113347828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfb68eeef2f54c5a0c542b65ba7fc90440c48b38740396b882c0e8d356613cb`  
		Last Modified: Fri, 26 Mar 2021 09:55:59 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:9dd42508841a3f375aa5b3f0e5ead7062c14801929b7f9a8ff9a61ed93b6d4d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223904167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f5ad9ead0abb0e0d18b019ac669921f0176098d64537311a3cca8a9daf077c`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:55:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 04:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:56:18 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:56:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:56:24 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:56:25 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:56:26 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:56:26 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:56:28 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 04 Mar 2021 04:56:29 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 04 Mar 2021 04:56:30 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 04:56:31 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:56:32 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 04:56:35 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 04:56:38 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 04:56:39 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 04 Mar 2021 04:56:44 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 04 Mar 2021 04:56:48 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 04:56:51 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 04:56:52 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:56:55 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 04:56:55 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:56:56 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c83eec9a08ca31b0967928280b24307ee3da07363b8b020fbcb8ef55e84f33c`  
		Last Modified: Thu, 04 Mar 2021 04:58:43 GMT  
		Size: 86.3 MB (86270625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51117579b7f1169aaeab24891e96baf3415884368d15c152a65af49d5cfe9d1e`  
		Last Modified: Thu, 04 Mar 2021 04:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3cac34d3604f9625bfd3599da48dcf450e69ef5fb5de231c031f012054b70`  
		Last Modified: Thu, 04 Mar 2021 04:58:24 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dafedb36e501fe29a3e4e4324415ccddc0dc0e435bf8b824d7fbc309e79706`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 541.8 KB (541823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a0f24e4821dbf50388ccf9152b4ed68b3360f8159203b309deba312c5e1623`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e898cc1ff802d14e5898a7ac295792ad446d2fa47415fb68420a838a1dbbea37`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb143758b6d8efaa13a38b2238d171ed6b10ea027a51a5d28a894e7e67469a5`  
		Last Modified: Thu, 04 Mar 2021 04:58:30 GMT  
		Size: 113.3 MB (113347830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9b616f8ca880f366a3d637dc18321caf7bce6a8cb0953fb6b738ad5640d9d0`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.11.4` - linux; ppc64le

```console
$ docker pull bonita@sha256:6d482e1a9e8ff6bcf053de4feefff6b644e7e03630b827a036e8f8fe591300e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231509710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a625fc56f0ed882580a1ec29e73430e366ea09bc32f6557f0676815d940d6b52`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:45:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 05:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:52:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:52:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:52:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:53:07 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:53:13 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:53:20 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:53:26 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:53:30 GMT
ENV BONITA_VERSION=7.11.4
# Thu, 04 Mar 2021 05:53:35 GMT
ENV BONITA_SHA256=5366b61bd36567b1fc62e8cb1d40a78a613c18c0d6eb894e9c414f57269b7d18
# Thu, 04 Mar 2021 05:53:41 GMT
ENV ZIP_FILE=BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 05:53:51 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:54:00 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/7.11.4/BonitaCommunity-7.11.4.zip
# Thu, 04 Mar 2021 05:54:13 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 05:54:28 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 05:54:30 GMT
COPY dir:224f3f698a7c2ba0960fd1c61d1b42d86ab0dee604621557635c99e6a0a6ec2d in /opt/files 
# Thu, 04 Mar 2021 05:54:45 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BONITA_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BONITA_VERSION}.zip; fi
# Thu, 04 Mar 2021 05:55:06 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 05:55:33 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 05:55:41 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:55:44 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 05:55:51 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:55:58 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5e22014470e3a0e33866d21001d1a638200e5d56c24c202f909de087a56bba`  
		Last Modified: Thu, 04 Mar 2021 06:01:39 GMT  
		Size: 87.2 MB (87187404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc56e644a17ce5a16b1fbcf26423ce252b5449b7aa9676ae35fa15de72babc0`  
		Last Modified: Thu, 04 Mar 2021 06:01:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08478a27e00e84d03e0711f150ecb392e9d57a85e568caabc250c0bc8214c7`  
		Last Modified: Thu, 04 Mar 2021 06:01:22 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3fab24756c5027d0b09cf6985b200d62c2ae0691ab4e19343babaf0756e71d`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 541.5 KB (541535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be368ca743dd0541c18b70c7fd4be07819f41e1ab9ae9a1420eb536fac8cab70`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef65ab37b2f073afda64c74705cc91f699e4153157280b65df4d491bce857bf7`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 6.9 KB (6893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175ee2d9d2d1ce7c2340e0a64e4ff6affb367c20d584a7b46a5a1f96a88ae6a`  
		Last Modified: Thu, 04 Mar 2021 06:01:28 GMT  
		Size: 113.3 MB (113347827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48edf254570016c0c9f66ff82f313675125d6073386dee64443bc95ec89f4a`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12`

```console
$ docker pull bonita@sha256:252b0188a02ffaef870ffece068c173564a5e2efeef27b48389526c247d69656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12` - linux; amd64

```console
$ docker pull bonita@sha256:bec7c62bfa26447c37ea9a71f638671f52400db14f9229eeee8e7df6a6a299b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238893974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce2c8eced3ba09353d4f974632f31ecce2489fc06865b589740531b2abbd1d3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:54:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 26 Mar 2021 09:54:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:54:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:54:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BRANDING_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 26 Mar 2021 09:54:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 26 Mar 2021 09:55:00 GMT
RUN mkdir /opt/files
# Fri, 26 Mar 2021 09:55:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 26 Mar 2021 09:55:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 26 Mar 2021 09:55:07 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 26 Mar 2021 09:55:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 26 Mar 2021 09:55:09 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:55:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 26 Mar 2021 09:55:09 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:55:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e534248c77c94586396089f5fe1e6ef3445619f3b25b01e3788c31a39246de`  
		Last Modified: Fri, 26 Mar 2021 09:56:17 GMT  
		Size: 95.2 MB (95182928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51fffa5c2969e00e61b80759c01c7b29a445487471b69cab746c2912685b51`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0795bb218aad676992e4855a54a7a8fbf0139bdb13b12a54e94c512da7714`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef20992b153c738c647dc0b493b155dc50a750365be70fcf88cfe88ce28b63d`  
		Last Modified: Fri, 26 Mar 2021 09:56:00 GMT  
		Size: 573.0 KB (572988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab13c0cfd407a99af4475a201b0e82ef59eb70270e887c1d76519a390f6df46`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fef7e4f41959abb0200ce52dbf1df79a3a1c6e2135817fa0b950601145d24a`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa40d92e0791bad639df8e2c95739cc01e6fc08a1c47bac8675668516852dba`  
		Last Modified: Fri, 26 Mar 2021 09:56:37 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dbd4b7563e31dcb93c41f4ddce6c2216761188046dc480a97cd1199207e72`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:214a951cf59a227aa245a53af6280fe9480bc2e429c293439717957bd24b0e84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226971792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30040d57cf072ea3506cc843473269c0fb303942ea3b5fbcd38121e86942f10d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:55:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 04:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:56:18 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:56:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:56:24 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:57:05 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 04:57:06 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:57:08 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 04:57:09 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 04:57:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 04:57:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 04:57:18 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 04:57:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 04:57:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 04:57:27 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 04:57:30 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 04:57:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:57:32 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 04:57:33 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:57:33 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c83eec9a08ca31b0967928280b24307ee3da07363b8b020fbcb8ef55e84f33c`  
		Last Modified: Thu, 04 Mar 2021 04:58:43 GMT  
		Size: 86.3 MB (86270625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51117579b7f1169aaeab24891e96baf3415884368d15c152a65af49d5cfe9d1e`  
		Last Modified: Thu, 04 Mar 2021 04:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3cac34d3604f9625bfd3599da48dcf450e69ef5fb5de231c031f012054b70`  
		Last Modified: Thu, 04 Mar 2021 04:58:24 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dafedb36e501fe29a3e4e4324415ccddc0dc0e435bf8b824d7fbc309e79706`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 541.8 KB (541823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8100ff6f916893fb3924689e93c9c3e2859d0ffd4bec28e0b1284443372e4546`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484e759bc1c1ec7509a26f4c7878c04074c5958ac5336be202beb41500d2eed8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b9e7d444fb6ada0affc11160806862ee09e60b2fa7893b2d79e8ef49b9c3e`  
		Last Modified: Thu, 04 Mar 2021 04:58:59 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037423ea62eef570b500fcddd4ee54bb39817bdef407c218d6bc612b50a881e8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12` - linux; ppc64le

```console
$ docker pull bonita@sha256:fa8da3b85935ea08dccb0e33f371c55ff6eb77fa3b848079f619b92e3f4ce1d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234577335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e9fc3702494f2ccec59668d5597b8ac6f2de2580fff1064b1086c9ad83f99ff`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:45:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 05:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:52:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:52:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:52:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:53:07 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:56:20 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 05:56:34 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:56:45 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:56:56 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:57:14 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 05:57:22 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 05:57:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 05:57:37 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:57:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:57:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:58:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 05:58:29 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 05:58:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 05:58:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 05:59:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 05:59:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 05:59:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:59:37 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 05:59:41 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:59:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5e22014470e3a0e33866d21001d1a638200e5d56c24c202f909de087a56bba`  
		Last Modified: Thu, 04 Mar 2021 06:01:39 GMT  
		Size: 87.2 MB (87187404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc56e644a17ce5a16b1fbcf26423ce252b5449b7aa9676ae35fa15de72babc0`  
		Last Modified: Thu, 04 Mar 2021 06:01:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08478a27e00e84d03e0711f150ecb392e9d57a85e568caabc250c0bc8214c7`  
		Last Modified: Thu, 04 Mar 2021 06:01:22 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3fab24756c5027d0b09cf6985b200d62c2ae0691ab4e19343babaf0756e71d`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 541.5 KB (541535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dfcc00939b4b6da9eb8e590933846fb345ccec05d50aa2a94e128e5d980e7c`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68b66bcb708201a8b22b6d73394f5b3850ae756f17e04a1bc44bcfa7d68751`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc5702d8d451399c87cff54266b5b9be4d3d70d34fa990e23c0a90c99f659a`  
		Last Modified: Thu, 04 Mar 2021 06:02:01 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef8e80ee863e5edc79546f700ae8d966adc43c717ed117518a4e66b78357070`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:7.12.1`

```console
$ docker pull bonita@sha256:252b0188a02ffaef870ffece068c173564a5e2efeef27b48389526c247d69656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:7.12.1` - linux; amd64

```console
$ docker pull bonita@sha256:bec7c62bfa26447c37ea9a71f638671f52400db14f9229eeee8e7df6a6a299b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238893974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce2c8eced3ba09353d4f974632f31ecce2489fc06865b589740531b2abbd1d3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:54:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 26 Mar 2021 09:54:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:54:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:54:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BRANDING_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 26 Mar 2021 09:54:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 26 Mar 2021 09:55:00 GMT
RUN mkdir /opt/files
# Fri, 26 Mar 2021 09:55:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 26 Mar 2021 09:55:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 26 Mar 2021 09:55:07 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 26 Mar 2021 09:55:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 26 Mar 2021 09:55:09 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:55:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 26 Mar 2021 09:55:09 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:55:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e534248c77c94586396089f5fe1e6ef3445619f3b25b01e3788c31a39246de`  
		Last Modified: Fri, 26 Mar 2021 09:56:17 GMT  
		Size: 95.2 MB (95182928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51fffa5c2969e00e61b80759c01c7b29a445487471b69cab746c2912685b51`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0795bb218aad676992e4855a54a7a8fbf0139bdb13b12a54e94c512da7714`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef20992b153c738c647dc0b493b155dc50a750365be70fcf88cfe88ce28b63d`  
		Last Modified: Fri, 26 Mar 2021 09:56:00 GMT  
		Size: 573.0 KB (572988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab13c0cfd407a99af4475a201b0e82ef59eb70270e887c1d76519a390f6df46`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fef7e4f41959abb0200ce52dbf1df79a3a1c6e2135817fa0b950601145d24a`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa40d92e0791bad639df8e2c95739cc01e6fc08a1c47bac8675668516852dba`  
		Last Modified: Fri, 26 Mar 2021 09:56:37 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dbd4b7563e31dcb93c41f4ddce6c2216761188046dc480a97cd1199207e72`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:214a951cf59a227aa245a53af6280fe9480bc2e429c293439717957bd24b0e84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226971792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30040d57cf072ea3506cc843473269c0fb303942ea3b5fbcd38121e86942f10d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:55:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 04:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:56:18 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:56:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:56:24 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:57:05 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 04:57:06 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:57:08 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 04:57:09 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 04:57:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 04:57:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 04:57:18 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 04:57:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 04:57:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 04:57:27 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 04:57:30 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 04:57:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:57:32 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 04:57:33 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:57:33 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c83eec9a08ca31b0967928280b24307ee3da07363b8b020fbcb8ef55e84f33c`  
		Last Modified: Thu, 04 Mar 2021 04:58:43 GMT  
		Size: 86.3 MB (86270625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51117579b7f1169aaeab24891e96baf3415884368d15c152a65af49d5cfe9d1e`  
		Last Modified: Thu, 04 Mar 2021 04:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3cac34d3604f9625bfd3599da48dcf450e69ef5fb5de231c031f012054b70`  
		Last Modified: Thu, 04 Mar 2021 04:58:24 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dafedb36e501fe29a3e4e4324415ccddc0dc0e435bf8b824d7fbc309e79706`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 541.8 KB (541823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8100ff6f916893fb3924689e93c9c3e2859d0ffd4bec28e0b1284443372e4546`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484e759bc1c1ec7509a26f4c7878c04074c5958ac5336be202beb41500d2eed8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b9e7d444fb6ada0affc11160806862ee09e60b2fa7893b2d79e8ef49b9c3e`  
		Last Modified: Thu, 04 Mar 2021 04:58:59 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037423ea62eef570b500fcddd4ee54bb39817bdef407c218d6bc612b50a881e8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:7.12.1` - linux; ppc64le

```console
$ docker pull bonita@sha256:fa8da3b85935ea08dccb0e33f371c55ff6eb77fa3b848079f619b92e3f4ce1d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234577335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e9fc3702494f2ccec59668d5597b8ac6f2de2580fff1064b1086c9ad83f99ff`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:45:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 05:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:52:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:52:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:52:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:53:07 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:56:20 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 05:56:34 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:56:45 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:56:56 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:57:14 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 05:57:22 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 05:57:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 05:57:37 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:57:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:57:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:58:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 05:58:29 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 05:58:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 05:58:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 05:59:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 05:59:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 05:59:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:59:37 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 05:59:41 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:59:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5e22014470e3a0e33866d21001d1a638200e5d56c24c202f909de087a56bba`  
		Last Modified: Thu, 04 Mar 2021 06:01:39 GMT  
		Size: 87.2 MB (87187404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc56e644a17ce5a16b1fbcf26423ce252b5449b7aa9676ae35fa15de72babc0`  
		Last Modified: Thu, 04 Mar 2021 06:01:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08478a27e00e84d03e0711f150ecb392e9d57a85e568caabc250c0bc8214c7`  
		Last Modified: Thu, 04 Mar 2021 06:01:22 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3fab24756c5027d0b09cf6985b200d62c2ae0691ab4e19343babaf0756e71d`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 541.5 KB (541535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dfcc00939b4b6da9eb8e590933846fb345ccec05d50aa2a94e128e5d980e7c`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68b66bcb708201a8b22b6d73394f5b3850ae756f17e04a1bc44bcfa7d68751`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc5702d8d451399c87cff54266b5b9be4d3d70d34fa990e23c0a90c99f659a`  
		Last Modified: Thu, 04 Mar 2021 06:02:01 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef8e80ee863e5edc79546f700ae8d966adc43c717ed117518a4e66b78357070`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `bonita:latest`

```console
$ docker pull bonita@sha256:252b0188a02ffaef870ffece068c173564a5e2efeef27b48389526c247d69656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `bonita:latest` - linux; amd64

```console
$ docker pull bonita@sha256:bec7c62bfa26447c37ea9a71f638671f52400db14f9229eeee8e7df6a6a299b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238893974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce2c8eced3ba09353d4f974632f31ecce2489fc06865b589740531b2abbd1d3`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:54:14 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Fri, 26 Mar 2021 09:54:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:54:35 GMT
RUN mkdir /opt/custom-init.d/
# Fri, 26 Mar 2021 09:54:36 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Fri, 26 Mar 2021 09:54:38 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Fri, 26 Mar 2021 09:54:38 GMT
ARG BONITA_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BRANDING_VERSION
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BONITA_SHA256
# Fri, 26 Mar 2021 09:54:56 GMT
ARG BASE_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ARG BONITA_URL
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_VERSION=7.12.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BRANDING_VERSION=2021.1
# Fri, 26 Mar 2021 09:54:57 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Fri, 26 Mar 2021 09:54:57 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Fri, 26 Mar 2021 09:54:58 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Fri, 26 Mar 2021 09:54:59 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Fri, 26 Mar 2021 09:55:00 GMT
RUN mkdir /opt/files
# Fri, 26 Mar 2021 09:55:00 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Fri, 26 Mar 2021 09:55:05 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Fri, 26 Mar 2021 09:55:07 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Fri, 26 Mar 2021 09:55:09 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Fri, 26 Mar 2021 09:55:09 GMT
VOLUME [/opt/bonita]
# Fri, 26 Mar 2021 09:55:09 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Fri, 26 Mar 2021 09:55:09 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 09:55:09 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e534248c77c94586396089f5fe1e6ef3445619f3b25b01e3788c31a39246de`  
		Last Modified: Fri, 26 Mar 2021 09:56:17 GMT  
		Size: 95.2 MB (95182928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51fffa5c2969e00e61b80759c01c7b29a445487471b69cab746c2912685b51`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0795bb218aad676992e4855a54a7a8fbf0139bdb13b12a54e94c512da7714`  
		Last Modified: Fri, 26 Mar 2021 09:56:02 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef20992b153c738c647dc0b493b155dc50a750365be70fcf88cfe88ce28b63d`  
		Last Modified: Fri, 26 Mar 2021 09:56:00 GMT  
		Size: 573.0 KB (572988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab13c0cfd407a99af4475a201b0e82ef59eb70270e887c1d76519a390f6df46`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fef7e4f41959abb0200ce52dbf1df79a3a1c6e2135817fa0b950601145d24a`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa40d92e0791bad639df8e2c95739cc01e6fc08a1c47bac8675668516852dba`  
		Last Modified: Fri, 26 Mar 2021 09:56:37 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4dbd4b7563e31dcb93c41f4ddce6c2216761188046dc480a97cd1199207e72`  
		Last Modified: Fri, 26 Mar 2021 09:56:29 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; arm64 variant v8

```console
$ docker pull bonita@sha256:214a951cf59a227aa245a53af6280fe9480bc2e429c293439717957bd24b0e84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (226971792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30040d57cf072ea3506cc843473269c0fb303942ea3b5fbcd38121e86942f10d`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:55:31 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 04:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:56:18 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 04:56:20 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 04:56:23 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 04:56:24 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 04:57:05 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 04:57:06 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 04:57:07 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 04:57:08 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 04:57:09 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 04:57:10 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 04:57:11 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 04:57:13 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 04:57:16 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 04:57:18 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 04:57:19 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 04:57:24 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 04:57:27 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 04:57:30 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 04:57:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 04:57:32 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 04:57:33 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 04:57:33 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c83eec9a08ca31b0967928280b24307ee3da07363b8b020fbcb8ef55e84f33c`  
		Last Modified: Thu, 04 Mar 2021 04:58:43 GMT  
		Size: 86.3 MB (86270625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51117579b7f1169aaeab24891e96baf3415884368d15c152a65af49d5cfe9d1e`  
		Last Modified: Thu, 04 Mar 2021 04:58:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3cac34d3604f9625bfd3599da48dcf450e69ef5fb5de231c031f012054b70`  
		Last Modified: Thu, 04 Mar 2021 04:58:24 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dafedb36e501fe29a3e4e4324415ccddc0dc0e435bf8b824d7fbc309e79706`  
		Last Modified: Thu, 04 Mar 2021 04:58:22 GMT  
		Size: 541.8 KB (541823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8100ff6f916893fb3924689e93c9c3e2859d0ffd4bec28e0b1284443372e4546`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484e759bc1c1ec7509a26f4c7878c04074c5958ac5336be202beb41500d2eed8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 6.9 KB (6945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b9e7d444fb6ada0affc11160806862ee09e60b2fa7893b2d79e8ef49b9c3e`  
		Last Modified: Thu, 04 Mar 2021 04:58:59 GMT  
		Size: 116.4 MB (116415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037423ea62eef570b500fcddd4ee54bb39817bdef407c218d6bc612b50a881e8`  
		Last Modified: Thu, 04 Mar 2021 04:58:49 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bonita:latest` - linux; ppc64le

```console
$ docker pull bonita@sha256:fa8da3b85935ea08dccb0e33f371c55ff6eb77fa3b848079f619b92e3f4ce1d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.6 MB (234577335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e9fc3702494f2ccec59668d5597b8ac6f2de2580fff1064b1086c9ad83f99ff`
-	Default Command: `["\/opt\/files\/startup.sh"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 05:45:46 GMT
LABEL maintainer=Bonitasoft Runtime team <rd.engine@bonitasoft.com>
# Thu, 04 Mar 2021 05:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends   curl   gnupg2   mysql-client-core-5.7   openjdk-11-jre-headless   postgresql-client   unzip   zip   && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 05:52:21 GMT
RUN mkdir /opt/custom-init.d/
# Thu, 04 Mar 2021 05:52:43 GMT
RUN groupadd -r bonita -g 1000   && useradd -u 1000 -r -g bonita -d /opt/bonita/ -s /sbin/nologin -c "Bonita User" bonita
# Thu, 04 Mar 2021 05:52:59 GMT
RUN (gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4   || gpg --keyserver ipv4.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4)   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture)" -o /usr/local/bin/gosu   && curl -fsSL "https://github.com/tianon/gosu/releases/download/1.10/gosu-$(dpkg --print-architecture).asc" -o /usr/local/bin/gosu.asc   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu
# Thu, 04 Mar 2021 05:53:07 GMT
ARG BONITA_VERSION
# Thu, 04 Mar 2021 05:56:20 GMT
ARG BRANDING_VERSION
# Thu, 04 Mar 2021 05:56:34 GMT
ARG BONITA_SHA256
# Thu, 04 Mar 2021 05:56:45 GMT
ARG BASE_URL
# Thu, 04 Mar 2021 05:56:56 GMT
ARG BONITA_URL
# Thu, 04 Mar 2021 05:57:14 GMT
ENV BONITA_VERSION=7.12.1
# Thu, 04 Mar 2021 05:57:22 GMT
ENV BRANDING_VERSION=2021.1
# Thu, 04 Mar 2021 05:57:27 GMT
ENV BONITA_SHA256=5342b18dd7f93bd3b2b64f8587504d0bf324f4f84d4259191b7291ee8f9ec693
# Thu, 04 Mar 2021 05:57:37 GMT
ENV ZIP_FILE=BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:57:48 GMT
ENV BASE_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download
# Thu, 04 Mar 2021 05:57:55 GMT
ENV BONITA_URL=https://github.com/bonitasoft/bonita-platform-releases/releases/download/2021.1/BonitaCommunity-2021.1.zip
# Thu, 04 Mar 2021 05:58:09 GMT
RUN echo "Downloading Bonita from url: ${BONITA_URL}"
# Thu, 04 Mar 2021 05:58:29 GMT
RUN mkdir /opt/files
# Thu, 04 Mar 2021 05:58:31 GMT
COPY dir:ceba4393fbbad2e791e9b0a75d4a81330c328bd9f67f35ff002adea48d26a677 in /opt/files 
# Thu, 04 Mar 2021 05:58:53 GMT
RUN if [ -f "/opt/files/BonitaCommunity-${BRANDING_VERSION}.zip" ]; then echo "File already present in /opt/files"; else curl -fsSL ${BONITA_URL} -o /opt/files/BonitaCommunity-${BRANDING_VERSION}.zip; fi
# Thu, 04 Mar 2021 05:59:08 GMT
RUN sha256sum /opt/files/${ZIP_FILE}
# Thu, 04 Mar 2021 05:59:19 GMT
RUN echo "$BONITA_SHA256" /opt/files/${ZIP_FILE} | sha256sum -c -
# Thu, 04 Mar 2021 05:59:31 GMT
VOLUME [/opt/bonita]
# Thu, 04 Mar 2021 05:59:37 GMT
COPY dir:c3e962ef70138930cdc6c114f07b10cd87f0a7897e828b1cf0f64aa4e7f29ecb in /opt/templates 
# Thu, 04 Mar 2021 05:59:41 GMT
EXPOSE 8080
# Thu, 04 Mar 2021 05:59:48 GMT
CMD ["/opt/files/startup.sh"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5e22014470e3a0e33866d21001d1a638200e5d56c24c202f909de087a56bba`  
		Last Modified: Thu, 04 Mar 2021 06:01:39 GMT  
		Size: 87.2 MB (87187404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc56e644a17ce5a16b1fbcf26423ce252b5449b7aa9676ae35fa15de72babc0`  
		Last Modified: Thu, 04 Mar 2021 06:01:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08478a27e00e84d03e0711f150ecb392e9d57a85e568caabc250c0bc8214c7`  
		Last Modified: Thu, 04 Mar 2021 06:01:22 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3fab24756c5027d0b09cf6985b200d62c2ae0691ab4e19343babaf0756e71d`  
		Last Modified: Thu, 04 Mar 2021 06:01:19 GMT  
		Size: 541.5 KB (541535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dfcc00939b4b6da9eb8e590933846fb345ccec05d50aa2a94e128e5d980e7c`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e68b66bcb708201a8b22b6d73394f5b3850ae756f17e04a1bc44bcfa7d68751`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 6.9 KB (6944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc5702d8d451399c87cff54266b5b9be4d3d70d34fa990e23c0a90c99f659a`  
		Last Modified: Thu, 04 Mar 2021 06:02:01 GMT  
		Size: 116.4 MB (116415402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef8e80ee863e5edc79546f700ae8d966adc43c717ed117518a4e66b78357070`  
		Last Modified: Thu, 04 Mar 2021 06:01:52 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
