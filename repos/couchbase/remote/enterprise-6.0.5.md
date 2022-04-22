## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:f73c0ae0bef46f9a04899090dd9f591a48da0dc8984c5e34fe2c1f427c3bcbd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:85d2882df82d69f38d8f9f68fef3ecc792d89ab879cab958c184060d14fc6daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466122488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf1b60b05db24224d7372489e555feac51d8ee9770fc506775fb4b10212a47e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:54:07 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 22 Apr 2022 01:56:51 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 22 Apr 2022 01:56:52 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 22 Apr 2022 01:56:52 GMT
ARG CB_VERSION=6.0.5
# Fri, 22 Apr 2022 01:56:52 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Fri, 22 Apr 2022 01:56:52 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Fri, 22 Apr 2022 01:56:52 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Fri, 22 Apr 2022 01:56:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 22 Apr 2022 01:56:53 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 22 Apr 2022 01:57:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 22 Apr 2022 01:57:54 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 22 Apr 2022 01:57:55 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 22 Apr 2022 01:57:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Fri, 22 Apr 2022 01:57:55 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 22 Apr 2022 01:57:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 22 Apr 2022 01:57:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 22 Apr 2022 01:57:56 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 22 Apr 2022 01:57:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 01:57:57 GMT
CMD ["couchbase-server"]
# Fri, 22 Apr 2022 01:57:57 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 22 Apr 2022 01:57:57 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c10f55cc78046081abe26d2f8c411b94a91e28c37752ea61b2785721349906b`  
		Last Modified: Fri, 22 Apr 2022 02:02:19 GMT  
		Size: 15.9 MB (15919369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c90991b486b0e91ccb34dacf710d98c75da6c8b8d7d71fab7bfa87cfec26abd`  
		Last Modified: Fri, 22 Apr 2022 02:02:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f1c86f7e1165e68fa48a1547525447f4263619ec750deac67459b4c1fe5e67`  
		Last Modified: Fri, 22 Apr 2022 02:02:15 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09faa4c4f951cca6127e28157fbd94238e2dffec73b45bcbfe80b67dd74c26cd`  
		Last Modified: Fri, 22 Apr 2022 02:02:54 GMT  
		Size: 423.4 MB (423363182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3a73ce3df82267699a3612145f180f6634e0d8471e0c87a71ba9d9d7a487c0`  
		Last Modified: Fri, 22 Apr 2022 02:02:14 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c27b821b9a4934647df3d04e7e022de2bd230e6c3f1cc410ee9965573b4cb42`  
		Last Modified: Fri, 22 Apr 2022 02:02:14 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7531fff3ca4057f25ba440d9b5c8dcaf21704304e64ac59a842b64e83e374edb`  
		Last Modified: Fri, 22 Apr 2022 02:02:12 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed3a3289b4ed56a5adc716f9643c5a9f082c7094eba3f843bd2c89bb6d7d289`  
		Last Modified: Fri, 22 Apr 2022 02:02:12 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480dde21ec542049d082e62a401b7c01d65255f79db465ad3bb5974f85e0fa40`  
		Last Modified: Fri, 22 Apr 2022 02:02:12 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554a4cf991aee1ebc5c881bbe3c8776b299b6ed9fae8c596ab2488f7d11e1726`  
		Last Modified: Fri, 22 Apr 2022 02:02:12 GMT  
		Size: 125.6 KB (125562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9a8105d7abc6d1e67d1c2c73bca1f9ea533ccd7fcf902691ebb0bced0d9876`  
		Last Modified: Fri, 22 Apr 2022 02:02:12 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
