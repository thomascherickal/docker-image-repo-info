## `couchbase:community`

```console
$ docker pull couchbase@sha256:82522b636913696db394b3257d1940d065870743aff79dc9278a0a8cd88933ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:fc836a7fdeb7d9393de2f6fffb26ac39f3527fcbd9a2cb7b02de6e70623533af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.0 MB (370040703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80b43f3207f2c43f78e655d2d155c5519680988dfbbb014de26e60afb9ea59a5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 25 Sep 2020 22:36:27 GMT
ADD file:23a55d7e93b396e490b6d0893137e5c13e3e0a234e0feaea8b1cfd4079fb1882 in / 
# Fri, 25 Sep 2020 22:36:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:36:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 22:36:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:36:29 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:44:15 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 25 Sep 2020 23:44:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 25 Sep 2020 23:44:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 25 Sep 2020 23:44:32 GMT
ARG CB_VERSION=6.6.0
# Fri, 25 Sep 2020 23:44:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 25 Sep 2020 23:45:46 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb
# Fri, 25 Sep 2020 23:45:46 GMT
ARG CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e
# Fri, 25 Sep 2020 23:45:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 25 Sep 2020 23:45:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 25 Sep 2020 23:46:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 25 Sep 2020 23:46:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 25 Sep 2020 23:46:30 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 25 Sep 2020 23:46:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 25 Sep 2020 23:46:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:46:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 25 Sep 2020 23:46:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 25 Sep 2020 23:46:33 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 25 Sep 2020 23:46:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 25 Sep 2020 23:46:33 GMT
CMD ["couchbase-server"]
# Fri, 25 Sep 2020 23:46:33 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 25 Sep 2020 23:46:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4f53fa4d2cf0e29c6a522433e0ac71a7ce0fdab158481052b2198b5518b83248`  
		Last Modified: Thu, 17 Sep 2020 13:19:58 GMT  
		Size: 44.5 MB (44517215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af7c939e38e8e3160fbbdcc26a32669529b962c79f7337df0a26bf0e9a76d59`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903d0ffd64f6ca1355d2b2df702fc674f5663981dfd100fe4588fb390dd3382c`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04feeed388b71fdca5cc3bce619d65a34f8a1a3e5b0ef03f8392d499970818eb`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13321097455f75b3a691364c922ef008a0f31ae48e80095437db909e1ec50278`  
		Last Modified: Fri, 25 Sep 2020 23:48:05 GMT  
		Size: 5.8 MB (5827091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475715eae3ed3eb82c617cd5b80f77835f9dc599ca0cd14302b796023bdc6d2`  
		Last Modified: Fri, 25 Sep 2020 23:49:25 GMT  
		Size: 2.1 KB (2071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6067f0604c2229ea73be7f5dcd793a1a2aca2a109566a3cd71b9350128371fdc`  
		Last Modified: Fri, 25 Sep 2020 23:50:06 GMT  
		Size: 319.6 MB (319572386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8825f297ded7ed73214946058e2811b14ffd52ec1d294935a17d0b42e8c224e7`  
		Last Modified: Fri, 25 Sep 2020 23:49:25 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dd7cb70c2b6c1de25b29a2128475347335f98235d3c429d8c4ebd292e8c6e4`  
		Last Modified: Fri, 25 Sep 2020 23:49:25 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92af5c8226ead8146bcc15a0fb6af128a8619f88f723d3d3f278312b3d08a67e`  
		Last Modified: Fri, 25 Sep 2020 23:49:24 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8f1563a9e00dd8a9bb3f76fd2ba4e85a0467d795d58d9739b87f36df146a1`  
		Last Modified: Fri, 25 Sep 2020 23:49:24 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08f4a288e366ef9ae6d0662d3f215c9d605d1feecef3b7fc1a9f1030d4b48c1`  
		Last Modified: Fri, 25 Sep 2020 23:49:24 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd6b0340cd84410874fb100516c64eedcb3bf9a73ed1c7355564e80bf443749`  
		Last Modified: Fri, 25 Sep 2020 23:49:26 GMT  
		Size: 118.1 KB (118073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa46955c2926c22d448edaeab37a366f3cb6099b642b62040885f112fca57114`  
		Last Modified: Fri, 25 Sep 2020 23:49:24 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
