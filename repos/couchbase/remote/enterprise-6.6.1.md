## `couchbase:enterprise-6.6.1`

```console
$ docker pull couchbase@sha256:ce27277fe7678f903b02438304ff57ff4455002bb9440844f2ff31a2eed2a2bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.1` - linux; amd64

```console
$ docker pull couchbase@sha256:8bae907adf53a82ae94c070752625dc94f9014807a26a232945d26eccdacbebb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528527045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b6f9c5715a276870475d948a55b433361fb63fab1c87dc085c57b563e089cda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:22:25 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:22:26 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_VERSION=6.6.1
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:25:10 GMT
ARG CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89
# Mon, 26 Jul 2021 22:25:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:25:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:26:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:26:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:26:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:26:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:26:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:26:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:26:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.1-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.1 CB_SHA256=4bd8210458905a5801e98bda0663d1214f6743465843f49ef9a52212636b5e89 CB_VERSION=6.6.1
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:26:26 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:26:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:26:26 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:26:27 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:26:27 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4e30704289595ec4268563ba339f4be2e264b88e79d255b680ccc550789ba`  
		Last Modified: Mon, 26 Jul 2021 22:41:09 GMT  
		Size: 7.4 MB (7373152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d99bab81201d5c70f8e51f9f400575173f81ff7b28365411dc726bd35ec58d`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab2f6ba05defbc278962d5c3675edb87a2a9aac298f764d149e8dfac6997210`  
		Last Modified: Mon, 26 Jul 2021 22:42:56 GMT  
		Size: 2.0 KB (1967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca281ad084b9caeb2bd4303f9ba708ebf5253a02428a14105ce61f4ad6c1649d`  
		Last Modified: Mon, 26 Jul 2021 22:43:52 GMT  
		Size: 494.3 MB (494322167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee6152ff40f616ef043558d6c3bdb575595e9dcef1fdd0861342cf30cf9ad83`  
		Last Modified: Mon, 26 Jul 2021 22:42:56 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8076a41dccc574445e6fe0e1c3da4ac85e5d04a288a65f361e88bba93f8608aa`  
		Last Modified: Mon, 26 Jul 2021 22:42:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6e027e9667d6d17e6ce6ac1a8893da041ed62683c31c582bdb8f1d738e50f8`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdbc0e5c5c39515362d1bb28bac1458a462fd9522995f866b1a24b4f5dd9063`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4512e7ea1b1be5ec7744ca0b9d0e4c3c0720ed6fb5b2055b3c10f583b3ed25b3`  
		Last Modified: Mon, 26 Jul 2021 22:42:54 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee32e5567f13959d200c1b58d732468142ea10d9e3e7a05bb249614074b6e05`  
		Last Modified: Mon, 26 Jul 2021 22:42:54 GMT  
		Size: 118.2 KB (118190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cc78198ad3662750502dc48a81a466e27e0ad29b7f8970f2acfc87524c0d50`  
		Last Modified: Mon, 26 Jul 2021 22:42:53 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
