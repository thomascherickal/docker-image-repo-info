## `couchbase:community`

```console
$ docker pull couchbase@sha256:1536191c7edb988af249104711eeeac8b40f5a465ea68e1f1c6dc62fcbd648bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:f8df503702af663b8cb48bf601d63c416c45de075f023c2f36068bcc76376fca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.2 MB (367215456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4487640b6d8b45fc3b39d4fbc15728eda320e5fcbf9392020962d45d4db05cb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Sat, 02 May 2020 01:19:23 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Sat, 02 May 2020 01:19:43 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 May 2020 01:19:44 GMT
ARG CB_VERSION=6.5.1
# Sat, 02 May 2020 01:19:44 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Sat, 02 May 2020 01:22:10 GMT
ARG CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu16.04_amd64.deb
# Sat, 02 May 2020 01:22:10 GMT
ARG CB_SHA256=baf65fb9cbcec87783d4e9c3ec067143a42cdeef13a884e1f917e8d2f14044b7
# Sat, 02 May 2020 01:22:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 May 2020 01:22:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=baf65fb9cbcec87783d4e9c3ec067143a42cdeef13a884e1f917e8d2f14044b7 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 May 2020 01:22:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=baf65fb9cbcec87783d4e9c3ec067143a42cdeef13a884e1f917e8d2f14044b7 CB_VERSION=6.5.1
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Sat, 02 May 2020 01:22:54 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Sat, 02 May 2020 01:22:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=baf65fb9cbcec87783d4e9c3ec067143a42cdeef13a884e1f917e8d2f14044b7 CB_VERSION=6.5.1
RUN chown -R couchbase:couchbase /etc/service
# Sat, 02 May 2020 01:22:55 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 May 2020 01:22:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=baf65fb9cbcec87783d4e9c3ec067143a42cdeef13a884e1f917e8d2f14044b7 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 May 2020 01:22:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=baf65fb9cbcec87783d4e9c3ec067143a42cdeef13a884e1f917e8d2f14044b7 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 02 May 2020 01:22:57 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 02 May 2020 01:22:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 May 2020 01:22:57 GMT
CMD ["couchbase-server"]
# Sat, 02 May 2020 01:22:57 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 02 May 2020 01:22:58 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f93bd3ca98a1033873ba74ef3f96fac728247e95ebcbbb5488c87e0ed868e97`  
		Last Modified: Sat, 02 May 2020 01:23:11 GMT  
		Size: 5.9 MB (5853645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6f55801e789caaba7edffb330101a364280f3605cd58ee1d5bc30f99b20ec1`  
		Last Modified: Sat, 02 May 2020 01:25:19 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d95797ac8be45eaa45f44684522b1fe3ca9c4289956a8fdf374e927536fea0`  
		Last Modified: Sat, 02 May 2020 01:26:00 GMT  
		Size: 317.0 MB (316990863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c9f7c45c7b2db2f9806a84aad453399851372024b2ee22b293fbe9cc7e0c9c`  
		Last Modified: Sat, 02 May 2020 01:25:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a22c69f50a4888e7c5858167b354105215521a87fcae5a043a2f4377dca3f02`  
		Last Modified: Sat, 02 May 2020 01:25:18 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34542aefec114d3b2f31a843296336901f04427cc32c1a18997253e8bb7541c`  
		Last Modified: Sat, 02 May 2020 01:25:18 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8013908c06d96ae79474fe3266b73ef3987b529dd751269ce656e893ec063bbe`  
		Last Modified: Sat, 02 May 2020 01:25:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8164d0c9624d1178f37e0d7e9694681e3988a2876445b566a6826f7153f8be9b`  
		Last Modified: Sat, 02 May 2020 01:25:18 GMT  
		Size: 118.1 KB (118068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070c8464ae0116a58666d50f0e346c775147608fb201c24e83e1b42e0e7ab0ed`  
		Last Modified: Sat, 02 May 2020 01:25:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
