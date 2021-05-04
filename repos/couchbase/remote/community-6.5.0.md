## `couchbase:community-6.5.0`

```console
$ docker pull couchbase@sha256:6e54b1e6afe72f227b028642a94216fcf0812c978f37c1d4756e031b637589dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community-6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:4b4d85e80dc33c239a3a5f5d49e38c1a28dc6de7c03921971b059c9e8bc3a8d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.9 MB (366868347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4091c0cc3b370804e8d91ab02f41a6afe63ee66ede7afac1b50ad7dbac1cdfef`
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
# Fri, 24 Apr 2020 13:55:51 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 24 Apr 2020 13:56:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 24 Apr 2020 13:57:22 GMT
ARG CB_VERSION=6.5.0
# Fri, 24 Apr 2020 13:57:22 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Fri, 24 Apr 2020 13:57:22 GMT
ARG CB_PACKAGE=couchbase-server-community_6.5.0-ubuntu16.04_amd64.deb
# Fri, 24 Apr 2020 13:57:22 GMT
ARG CB_SHA256=0b83b4861840392540c3c0b4f8ccc64f8f5adbebde4c05bd99b857dc3d528445
# Fri, 24 Apr 2020 13:57:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 24 Apr 2020 13:57:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=0b83b4861840392540c3c0b4f8ccc64f8f5adbebde4c05bd99b857dc3d528445 CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 24 Apr 2020 13:58:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=0b83b4861840392540c3c0b4f8ccc64f8f5adbebde4c05bd99b857dc3d528445 CB_VERSION=6.5.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 24 Apr 2020 13:58:07 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 24 Apr 2020 13:58:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=0b83b4861840392540c3c0b4f8ccc64f8f5adbebde4c05bd99b857dc3d528445 CB_VERSION=6.5.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 24 Apr 2020 13:58:08 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 24 Apr 2020 13:58:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=0b83b4861840392540c3c0b4f8ccc64f8f5adbebde4c05bd99b857dc3d528445 CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 24 Apr 2020 13:58:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=0b83b4861840392540c3c0b4f8ccc64f8f5adbebde4c05bd99b857dc3d528445 CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 24 Apr 2020 13:58:09 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 24 Apr 2020 13:58:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 13:58:10 GMT
CMD ["couchbase-server"]
# Fri, 24 Apr 2020 13:58:10 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 24 Apr 2020 13:58:10 GMT
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
	-	`sha256:e9d2aab75cd7283128edf9c135cc5472dec505d81af38ad20a38681f83a5da6a`  
		Last Modified: Fri, 24 Apr 2020 13:58:22 GMT  
		Size: 5.9 MB (5853660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108123180fa9daa23892a4628183ec969f6689cf5a0b4c660594b0e53cb1c659`  
		Last Modified: Fri, 24 Apr 2020 13:59:26 GMT  
		Size: 2.1 KB (2078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821631d1b9521b1c4dde972e34690892764225f3672f06d77e558b215f27046`  
		Last Modified: Fri, 24 Apr 2020 14:00:07 GMT  
		Size: 316.6 MB (316643734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bb83323165c8fe7f7578d41b93031df5aebf03e4b89fc1be416a7dc318e1cb`  
		Last Modified: Fri, 24 Apr 2020 13:59:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8804278100583d60e4b5a58e82b44476b07c13ac76d2059a374a95aff1f5e87`  
		Last Modified: Fri, 24 Apr 2020 13:59:25 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd92661dd9b078b75a35b2ed315726c94fc4dd95f086964a3c7f698b07dc067`  
		Last Modified: Fri, 24 Apr 2020 13:59:25 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a193e5fbf8c21b013f63dd60fef52a16b0d7c1d6f601f01eb28e6546c30a4f5a`  
		Last Modified: Fri, 24 Apr 2020 13:59:25 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f225f3217725820de11f9e2fc7f1ea40e8a4e9aaf52a07b778e37d723e389d30`  
		Last Modified: Fri, 24 Apr 2020 13:59:25 GMT  
		Size: 118.1 KB (118066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c0031d92ccf035880de989266e3f37436e85cf9530b3902a73ba20cb615cc0`  
		Last Modified: Fri, 24 Apr 2020 13:59:25 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
