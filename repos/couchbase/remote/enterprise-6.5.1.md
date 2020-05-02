## `couchbase:enterprise-6.5.1`

```console
$ docker pull couchbase@sha256:059365e37a618f31a1b379e6047e6c1ad4eb4076456d9931cdee462112cd5fb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.5.1` - linux; amd64

```console
$ docker pull couchbase@sha256:58ff9e691dde64ae2c7b2e2807659b67789f63714704b077ae8ad205a914118c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.2 MB (515238912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0215190196397077da0e96d8ae41ebb73ba1f71c003612dab40d7e72ea615e1b`
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
# Sat, 02 May 2020 01:19:44 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb
# Sat, 02 May 2020 01:19:44 GMT
ARG CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66
# Sat, 02 May 2020 01:19:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 May 2020 01:19:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 May 2020 01:20:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Sat, 02 May 2020 01:20:40 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Sat, 02 May 2020 01:20:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN chown -R couchbase:couchbase /etc/service
# Sat, 02 May 2020 01:20:41 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 May 2020 01:20:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 May 2020 01:20:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.1-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.1 CB_SHA256=80427193137e5cb5a4795b2675b1c450c1af8cf1a5c634d917f6c416f2047e66 CB_VERSION=6.5.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 02 May 2020 01:20:43 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 02 May 2020 01:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 May 2020 01:20:43 GMT
CMD ["couchbase-server"]
# Sat, 02 May 2020 01:20:43 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 02 May 2020 01:20:43 GMT
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
	-	`sha256:57a7a0cfb17009254c097cbb76b299dc79e7aa6ea604413a5f8246f6e043a51e`  
		Last Modified: Sat, 02 May 2020 01:23:10 GMT  
		Size: 2.1 KB (2073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef6b4690dba4d981bf1939d9d634eaa08ee896c97a35b9ea41094d6d23b06f3`  
		Last Modified: Sat, 02 May 2020 01:24:07 GMT  
		Size: 465.0 MB (465014313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b195a0a56ba73085b66644237b0e82ca98a10845d672a1b49c89719f9d9a9b78`  
		Last Modified: Sat, 02 May 2020 01:23:09 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5ea149961075296ae745932af8af1f14d0274df59b55a77c444070159bca76`  
		Last Modified: Sat, 02 May 2020 01:23:09 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e386ee257b627c967ad929dba2c12800db7ffddc95b917b234aabbe52bad4460`  
		Last Modified: Sat, 02 May 2020 01:23:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0177a2d2805b3926b8d5186c21fc46b1d8fbbc58f0352af93a30f8585dfb5ee`  
		Last Modified: Sat, 02 May 2020 01:23:08 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38311719d6f716bacab895d923f5d702eec08754ebf1fed8e9f6eb54df73557`  
		Last Modified: Sat, 02 May 2020 01:23:08 GMT  
		Size: 118.1 KB (118068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b7b5edf67c9914938a0b1c05727e5b4c7e57311e48e76f4962463051430b2`  
		Last Modified: Sat, 02 May 2020 01:23:08 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
