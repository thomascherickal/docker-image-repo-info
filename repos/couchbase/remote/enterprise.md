## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:0382490b6adc64ce6af02301b9af17966c925ef7a041df863cd6f67d350fd7fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:24e688b1185af01abd56af4bc4f6c8fe430463c84ad64ea9b06a682c0aeb5552
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.2 MB (515238918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf82cb58b98c6339ebfa8ce5c0cc2653061d83cfabdf1ca502892ca2bd084b8`
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
# Fri, 24 Apr 2020 13:56:15 GMT
ARG CB_VERSION=6.5.1
# Fri, 24 Apr 2020 13:56:15 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1
# Fri, 24 Apr 2020 13:56:16 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb
# Fri, 24 Apr 2020 13:56:16 GMT
ARG CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66
# Fri, 24 Apr 2020 13:56:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 24 Apr 2020 13:56:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 24 Apr 2020 13:57:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 24 Apr 2020 13:57:09 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 24 Apr 2020 13:57:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN chown -R couchbase:couchbase /etc/service
# Fri, 24 Apr 2020 13:57:10 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 24 Apr 2020 13:57:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 24 Apr 2020 13:57:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 24 Apr 2020 13:57:12 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 24 Apr 2020 13:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 13:57:12 GMT
CMD ["couchbase-server"]
# Fri, 24 Apr 2020 13:57:13 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 24 Apr 2020 13:57:13 GMT
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
	-	`sha256:b7e155f518646f532d47ddd1c9052966d0da8c01cb732fff363c0f89d0714163`  
		Last Modified: Fri, 24 Apr 2020 13:58:21 GMT  
		Size: 2.1 KB (2075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f108373b8aa7c708bb1503d485411e68a9d49049e97ad5b37ad57d1616f56a90`  
		Last Modified: Fri, 24 Apr 2020 13:59:18 GMT  
		Size: 465.0 MB (465014302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e368a6612821a33a1bfb6a756e9115cf56d97ff572ca0fc2478777111575a8c`  
		Last Modified: Fri, 24 Apr 2020 13:58:21 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98d39ddb724f36a4fbfa76f17c9af98309508c8d552e82d048a860b42caafcc`  
		Last Modified: Fri, 24 Apr 2020 13:58:19 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b93852339d4baa6e3d700b32fa6bd07a91af19b74fc38abc99c2d4efcf3f23`  
		Last Modified: Fri, 24 Apr 2020 13:58:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a698b0882a0d68b5131ea7bf6f97a2e2926a9131b5d2b982df149172bc98aff9`  
		Last Modified: Fri, 24 Apr 2020 13:58:19 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d802c69d4bb2e5cd263f1ac91c54059acb47dd7ab8c90e24e3b3224f28bab3`  
		Last Modified: Fri, 24 Apr 2020 13:58:19 GMT  
		Size: 118.1 KB (118065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d495b9b4b570ec4e36c56c13d83642f2aecd6046a6718b938b7c1e8b6b096`  
		Last Modified: Fri, 24 Apr 2020 13:58:20 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
