## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:2befadeed5bbfd07b657995c9432dad470840d4b32d8757c4de44f1f8bdb0bf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533222654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c4c1a0b656b1893a5cc9277f0a39ac1771db24a19fcb5cd17e2c96f5b6f01d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:17:12 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:20:33 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:20:33 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_VERSION=6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb
# Mon, 26 Jul 2021 22:20:34 GMT
ARG CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc
# Mon, 26 Jul 2021 22:20:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:20:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:21:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:21:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:21:35 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:21:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:21:36 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:21:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:21:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.2 CB_SHA256=41c033e6c1e98b0844a5cb5768e3769e7012d8374a6bd235c86e10db33b17afc CB_VERSION=6.6.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:21:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:21:38 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:21:39 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:21:39 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d887c602d6e2b416c36a7344e07f41278a46971fa08be0eeb2fc78a75d7013b`  
		Last Modified: Mon, 26 Jul 2021 22:39:49 GMT  
		Size: 6.3 MB (6272568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b219d16ecda3370190c17757e31f650c0b2db8a483364cebc0add69c976f1fa`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3fec572429eea18c02afb8a6c9879b303a8fe54f24c598d70e76284d2e50`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc966ce6300d6331c07980d729ddad541989a337e6eb174cab32a6da22196a4b`  
		Last Modified: Mon, 26 Jul 2021 22:40:42 GMT  
		Size: 498.3 MB (498251893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb4c7a902a3d8673bde3e41bdcafb1f24b6bd970572a368d1d1c290bc0f0c5c`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef06a70d616a9d9e24737530889d9744fa42fa92f9c293f9a47ab5046769e4e5`  
		Last Modified: Mon, 26 Jul 2021 22:39:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a527aa307ea3cd1feffde8b7b71f90af3149dc21432afb9d9c9187c61017c5`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4233c8f62d720537a74a69707dd1d651286d9bfab88848bb8d41445266481254`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda6ae4667566d063e0d185b915cc7fe3d16ea8dd7504aa48ae246e35db9d509`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01243b96b0b7ddaf69634a7674356f0e483f5f24e91d57de48d161fcf28d65d0`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74aee4374d591a250acc5a5e8b2be6cacffceebba6ee89c2fe32ba3806144098`  
		Last Modified: Mon, 26 Jul 2021 22:39:42 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
