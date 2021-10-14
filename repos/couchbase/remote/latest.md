## `couchbase:latest`

```console
$ docker pull couchbase@sha256:cb3a2faeeef0345c70690485274096efc2174f194046ded5700426479a741fc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:e7e452512f4a7b26d5ab0ed852891537e755165763cb9a2e2fd8cf267f34908f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.3 MB (653331667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ac58ce87a857e475c914b1aa0ef31338e0e2f03f65396c5414fa0580ce7746f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:41:23 GMT
LABEL maintainer=docker@couchbase.com
# Fri, 01 Oct 2021 02:41:49 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 01 Oct 2021 02:41:50 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Thu, 14 Oct 2021 19:22:24 GMT
ARG CB_VERSION=7.0.2
# Thu, 14 Oct 2021 19:22:24 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Thu, 14 Oct 2021 19:22:24 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb
# Thu, 14 Oct 2021 19:22:24 GMT
ARG CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15
# Thu, 14 Oct 2021 19:22:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Thu, 14 Oct 2021 19:22:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15 CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Thu, 14 Oct 2021 19:23:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15 CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Thu, 14 Oct 2021 19:23:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15 CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Thu, 14 Oct 2021 19:23:42 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Thu, 14 Oct 2021 19:23:43 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15 CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Thu, 14 Oct 2021 19:23:43 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Thu, 14 Oct 2021 19:23:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15 CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Thu, 14 Oct 2021 19:23:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=208fa1e4bf89e34f0f83abbd75cd720a18dd2de490b0154b42baaed690c36d15 CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Thu, 14 Oct 2021 19:23:45 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Thu, 14 Oct 2021 19:23:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 19:23:46 GMT
CMD ["couchbase-server"]
# Thu, 14 Oct 2021 19:23:46 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Thu, 14 Oct 2021 19:23:46 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613d9cf3c7de3b660067509bdefdbe2edc5d448de2122399663ad4f10564ff7`  
		Last Modified: Fri, 01 Oct 2021 02:49:55 GMT  
		Size: 6.3 MB (6262599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f6d1844f56aa2609795f15f46bc684d4d477f33fc1c0a486595f0449d80d14`  
		Last Modified: Fri, 01 Oct 2021 02:49:50 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc23c72f800c40df01eaad5797a378a480f3e05ce797964616ea6888ba89c44`  
		Last Modified: Thu, 14 Oct 2021 19:25:34 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41532c6d51fe9ed004563a0384ceb6e1e71f6e1bb43a64c8e6b69712ee9bfaa6`  
		Last Modified: Thu, 14 Oct 2021 19:26:38 GMT  
		Size: 618.4 MB (618366147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5600a8e0b74f96b7a35e650f2e1f8350633a2d1d901349297a387010776a1d8e`  
		Last Modified: Thu, 14 Oct 2021 19:25:34 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502fcc91de4f96ba57ef4e0665a15ebdc89f4fc0b9531987bb230abc59edbf5`  
		Last Modified: Thu, 14 Oct 2021 19:25:34 GMT  
		Size: 604.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e05776916fe06fd202b24ccef0c5bce44e25903ba31689f8b792e1e27a14eaf`  
		Last Modified: Thu, 14 Oct 2021 19:25:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab83f55f9bf108dbec532437af912e5f146d236da9c0cf70ffca91a10d84e17c`  
		Last Modified: Thu, 14 Oct 2021 19:25:32 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4e9d2017b132ac8db4ec278df1fe7c6b13433fba9ff422fe9e61739c18e2e1`  
		Last Modified: Thu, 14 Oct 2021 19:25:32 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8eaeee51366c1c624a21199bfb31475ffdf3f990c6fc4ced72b765a9b8169`  
		Last Modified: Thu, 14 Oct 2021 19:25:32 GMT  
		Size: 129.5 KB (129509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c4e57676bda38aad0f14ffd8be8beea14d730158ac3deb8a8c8175888155fb`  
		Last Modified: Thu, 14 Oct 2021 19:25:32 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
