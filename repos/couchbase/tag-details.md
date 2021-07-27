<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.5`](#couchbase605)
-	[`couchbase:6.6.2`](#couchbase662)
-	[`couchbase:7.0.0`](#couchbase700)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.0`](#couchbasecommunity-700)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.5`](#couchbaseenterprise-605)
-	[`couchbase:enterprise-6.6.2`](#couchbaseenterprise-662)
-	[`couchbase:enterprise-7.0.0`](#couchbaseenterprise-700)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.5`

```console
$ docker pull couchbase@sha256:4076897f81ab96c69d27f42accb996d141dbd3a2e9023579841b2361597553c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:3a8ee070210558c8a7b4f42d1cef3d608db79a83510927b40eec0423ccbd23d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466124028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8db7615f18de1e06f508993a9d442ce0eafcea50895d938de595152a2123121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_VERSION=6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:23:57 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Mon, 26 Jul 2021 22:23:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:23:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:24:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:25:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:25:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:25:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:25:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:25:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:25:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:25:03 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:25:04 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:25:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:25:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f22272715b7ac39bdeb72247eb7c9d676e111cb87f716a6b7d9a3699677895`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272140edf88cd01360aac5bddc2d13a011276f72173b6d9ae176fe243afbcbe`  
		Last Modified: Mon, 26 Jul 2021 22:42:41 GMT  
		Size: 423.4 MB (423361988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78863e03e170d48a06840a1f3c0af08fc6a03998bd8b2cc5bd9d42146459335`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c75079115b27ecc729a3d9a6ea34ffbbf322b75074b937b0a88b311b44e09`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be88b035f8327fce982f782ee4d4f158a491292ab1a83ea9bec04510e2eeedf`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93191caa985b907966beca25f0640d7f64475b6f2662beaa3e13685df8684139`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7069e44f4669174a2e317fd06732143189d95777bc146d3897c070d52028`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d37421dd736067d67fc2e040630fd1bc247c1f2cfc75354428c93d6ace6ba3`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 125.6 KB (125559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4704f88c75024de08db79dc6908a3dc28f99ca5b88bb3d403b7410161fc66d`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.2`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.2` - linux; amd64

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

## `couchbase:7.0.0`

```console
$ docker pull couchbase@sha256:005fb3ba97c2362b9ccc9d96f0d94bf09c2fe784d889fe71c5a2ba475e4645a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.0` - linux; amd64

```console
$ docker pull couchbase@sha256:f2a81b4271f0bdec4d2e5f8f2b9e9febced79048b4cd9c144ff3b832272ba76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633083217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9022428339d4615af519685439630f4532bb43a64f4c82f29c299271e16d0e56`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 27 Jul 2021 19:19:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:19:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:20:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:20:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:20:58 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:20:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:20:59 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:21:01 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:21:01 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:21:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:21:01 GMT
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
	-	`sha256:a6cdc5f71c3710468544fa224018c4a47ccf6c406ead41085cedf89ef99d1775`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e678d3290280e91fe94b0fc2b0faff059cab446516e5fb869856421c7001f4e`  
		Last Modified: Tue, 27 Jul 2021 19:23:43 GMT  
		Size: 598.1 MB (598112447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6969abcd0ca4371e2769bc97077e2f43ced0451abd159601e138e1edf5b1e283`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa359b4f22f914a20e211ae281fe312fe947736087893320e7c6543ccae9be`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07230fb0fa2e887a74bad436262a80d194b7ffe238041586fd2b4130b1e9c0d9`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9404dfab9613ac5843b1093f86d2cbaba3da74f61f3f5afb689f34b58298c55a`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73844eba4f0814d5e3f122bcd4fe4af5b787a43cad92054aa50926896fea85`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce7876a709925e51b4b5d0cee4cf4e000bf2bda2719984b15d8977e5256d50`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 125.9 KB (125889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f13caac7cd9de24759a20e590d18b3ce3c085c8ce971e0a023b96f4ed12c4f`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:5209e8a3f6d820f51156b2d42022f1ad9ed307d06bed98200e9640104bc6903c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:1596930a8d36d5ccab44257d51e12b2af353f43b4c0578df69c0cf7a747be928
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.2 MB (422213968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb087be1f30a05c7a561653462f48398876552d038d6dfa0d8033bd565345108`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:21:17 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:21:17 GMT
ARG CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917
# Tue, 27 Jul 2021 19:21:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:21:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:22:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:22:10 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:22:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:22:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:22:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:22:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:22:13 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:22:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:22:13 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:22:13 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:22:13 GMT
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
	-	`sha256:a1cf83af44430a71943715b43e7c8f87d6ce82d8bdb88192cc20b73a87b43f33`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aaeb2cc13bed178c9e5e91c6ba3ecf54abb4454f39364d358a700f69d05bac`  
		Last Modified: Tue, 27 Jul 2021 19:24:50 GMT  
		Size: 387.2 MB (387243194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde7395f0568ff1c42d851212ce76a4f9bf40ec9a71afb1952aae67fc7bed1aa`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38df88bcf23d7f037db5fc4e006badc005366761c3c1cf420c3c7774f17f030`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d04a1e99ea14c12b42d9753fc2fdb631bdbbc9fff53fc6eab1ed040f779383`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54719ccd40bb0f33aea8d0a9c5df90325fb22efae883c578ac83f0de97750248`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a2045c058ad8acb998220d05cbf9de249e96103ed80d428da13e49913b6bf5`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ad80e471e34c27ed65fa8e3fde09a29a6cdaec8853d1df31d959a6915b8b9a`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 125.9 KB (125892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da50f7a164483d6c24dcbc7c1a374400c56482cef8b36cd5652beb9b0b910`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:b0baeef769e4ba8fab7ac8e0a78416a009de893fb3d6bf9c1dcbb75130fd004c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:610c0d832bdb7e0144b88a509c9b857bf1551ae55572450dee2e2515eba3b313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354223029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2ef0dbd9aca1cefb55ddecf92c830dda7d3d252e86f4a7511de382b757502e`
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
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_VERSION=6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:22:27 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Mon, 26 Jul 2021 22:22:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:22:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:23:10 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:23:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:23:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:23:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:23:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:23:13 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:23:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:23:14 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:23:14 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:23:14 GMT
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
	-	`sha256:c19a3ff870dc5ba081bf7d1af748df9148879de3770eedbd347b181ba4418c79`  
		Last Modified: Mon, 26 Jul 2021 22:41:05 GMT  
		Size: 2.0 KB (1959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f382ce40a4c6276945dbeef635ef708db6059159d9cd4a3425a74b617526260`  
		Last Modified: Mon, 26 Jul 2021 22:41:43 GMT  
		Size: 320.0 MB (320018160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c2b9b12ebfafd8910844e882c5402810c40d25ab0db6e3d5820fd0caf23ecd`  
		Last Modified: Mon, 26 Jul 2021 22:41:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47da75ba54f0fd4481a18770a6976b47209fae9e9cfd864555a2cc9c008f14f`  
		Last Modified: Mon, 26 Jul 2021 22:41:04 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279f16369c32576b89b9cb15e9bd6cdcae6e87c10488a78576e3aaebfbcc8a05`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc3de5a1ae1dcb40c884fe38811c4ddec5f9a69fc46ac0baa1600c5eddf1840`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af87bf9317c38c511c9e1d45f577b67286e9e32b9cf9e7f11477850fc3400c2`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103e2a72cbd3696decc19440714d165b3ba00fe9bb3b598d2f5ff90d8972a99`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 118.2 KB (118192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a84cb279ced42a19136d7a67ce9cfa512a52dd859792f4d93e2c4b605d95a`  
		Last Modified: Mon, 26 Jul 2021 22:41:02 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.0`

```console
$ docker pull couchbase@sha256:5209e8a3f6d820f51156b2d42022f1ad9ed307d06bed98200e9640104bc6903c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.0` - linux; amd64

```console
$ docker pull couchbase@sha256:1596930a8d36d5ccab44257d51e12b2af353f43b4c0578df69c0cf7a747be928
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.2 MB (422213968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb087be1f30a05c7a561653462f48398876552d038d6dfa0d8033bd565345108`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:21:17 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:21:17 GMT
ARG CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917
# Tue, 27 Jul 2021 19:21:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:21:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:22:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:22:10 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:22:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:22:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:22:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:22:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=dd70ca6e45fa40aff5b168aef89509f97eaad5dc2c74c9df7966d28bdc56d917 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:22:13 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:22:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:22:13 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:22:13 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:22:13 GMT
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
	-	`sha256:a1cf83af44430a71943715b43e7c8f87d6ce82d8bdb88192cc20b73a87b43f33`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aaeb2cc13bed178c9e5e91c6ba3ecf54abb4454f39364d358a700f69d05bac`  
		Last Modified: Tue, 27 Jul 2021 19:24:50 GMT  
		Size: 387.2 MB (387243194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde7395f0568ff1c42d851212ce76a4f9bf40ec9a71afb1952aae67fc7bed1aa`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38df88bcf23d7f037db5fc4e006badc005366761c3c1cf420c3c7774f17f030`  
		Last Modified: Tue, 27 Jul 2021 19:24:04 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d04a1e99ea14c12b42d9753fc2fdb631bdbbc9fff53fc6eab1ed040f779383`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54719ccd40bb0f33aea8d0a9c5df90325fb22efae883c578ac83f0de97750248`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a2045c058ad8acb998220d05cbf9de249e96103ed80d428da13e49913b6bf5`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ad80e471e34c27ed65fa8e3fde09a29a6cdaec8853d1df31d959a6915b8b9a`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 125.9 KB (125892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da50f7a164483d6c24dcbc7c1a374400c56482cef8b36cd5652beb9b0b910`  
		Last Modified: Tue, 27 Jul 2021 19:24:02 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:005fb3ba97c2362b9ccc9d96f0d94bf09c2fe784d889fe71c5a2ba475e4645a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:f2a81b4271f0bdec4d2e5f8f2b9e9febced79048b4cd9c144ff3b832272ba76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633083217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9022428339d4615af519685439630f4532bb43a64f4c82f29c299271e16d0e56`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 27 Jul 2021 19:19:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:19:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:20:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:20:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:20:58 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:20:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:20:59 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:21:01 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:21:01 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:21:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:21:01 GMT
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
	-	`sha256:a6cdc5f71c3710468544fa224018c4a47ccf6c406ead41085cedf89ef99d1775`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e678d3290280e91fe94b0fc2b0faff059cab446516e5fb869856421c7001f4e`  
		Last Modified: Tue, 27 Jul 2021 19:23:43 GMT  
		Size: 598.1 MB (598112447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6969abcd0ca4371e2769bc97077e2f43ced0451abd159601e138e1edf5b1e283`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa359b4f22f914a20e211ae281fe312fe947736087893320e7c6543ccae9be`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07230fb0fa2e887a74bad436262a80d194b7ffe238041586fd2b4130b1e9c0d9`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9404dfab9613ac5843b1093f86d2cbaba3da74f61f3f5afb689f34b58298c55a`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73844eba4f0814d5e3f122bcd4fe4af5b787a43cad92054aa50926896fea85`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce7876a709925e51b4b5d0cee4cf4e000bf2bda2719984b15d8977e5256d50`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 125.9 KB (125889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f13caac7cd9de24759a20e590d18b3ce3c085c8ce971e0a023b96f4ed12c4f`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:4076897f81ab96c69d27f42accb996d141dbd3a2e9023579841b2361597553c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:3a8ee070210558c8a7b4f42d1cef3d608db79a83510927b40eec0423ccbd23d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466124028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8db7615f18de1e06f508993a9d442ce0eafcea50895d938de595152a2123121`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:21:49 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 26 Jul 2021 22:23:55 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:23:56 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_VERSION=6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Mon, 26 Jul 2021 22:23:56 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Mon, 26 Jul 2021 22:23:57 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Mon, 26 Jul 2021 22:23:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 26 Jul 2021 22:23:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 26 Jul 2021 22:24:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 26 Jul 2021 22:25:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 26 Jul 2021 22:25:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Mon, 26 Jul 2021 22:25:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 26 Jul 2021 22:25:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 26 Jul 2021 22:25:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 26 Jul 2021 22:25:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Mon, 26 Jul 2021 22:25:03 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Mon, 26 Jul 2021 22:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 26 Jul 2021 22:25:04 GMT
CMD ["couchbase-server"]
# Mon, 26 Jul 2021 22:25:04 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 26 Jul 2021 22:25:04 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34675e7dacc0ce319b39b9ea2535f805fa959a52abc54f87cc0a227b97902ca`  
		Last Modified: Mon, 26 Jul 2021 22:42:05 GMT  
		Size: 15.9 MB (15922947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889c4fafca81882f6937a23d718195844112f8f700b2bbf19b2fed74fb78653f`  
		Last Modified: Mon, 26 Jul 2021 22:42:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f22272715b7ac39bdeb72247eb7c9d676e111cb87f716a6b7d9a3699677895`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 2.0 KB (1969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6272140edf88cd01360aac5bddc2d13a011276f72173b6d9ae176fe243afbcbe`  
		Last Modified: Mon, 26 Jul 2021 22:42:41 GMT  
		Size: 423.4 MB (423361988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78863e03e170d48a06840a1f3c0af08fc6a03998bd8b2cc5bd9d42146459335`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c75079115b27ecc729a3d9a6ea34ffbbf322b75074b937b0a88b311b44e09`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be88b035f8327fce982f782ee4d4f158a491292ab1a83ea9bec04510e2eeedf`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93191caa985b907966beca25f0640d7f64475b6f2662beaa3e13685df8684139`  
		Last Modified: Mon, 26 Jul 2021 22:41:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a7069e44f4669174a2e317fd06732143189d95777bc146d3897c070d52028`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d37421dd736067d67fc2e040630fd1bc247c1f2cfc75354428c93d6ace6ba3`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 125.6 KB (125559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4704f88c75024de08db79dc6908a3dc28f99ca5b88bb3d403b7410161fc66d`  
		Last Modified: Mon, 26 Jul 2021 22:41:55 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.2`

```console
$ docker pull couchbase@sha256:9e6e9947a937f0e1d692deb0276131e10f0f12a8fd469e33d30fdd6b6a658c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.2` - linux; amd64

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

## `couchbase:enterprise-7.0.0`

```console
$ docker pull couchbase@sha256:005fb3ba97c2362b9ccc9d96f0d94bf09c2fe784d889fe71c5a2ba475e4645a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.0` - linux; amd64

```console
$ docker pull couchbase@sha256:f2a81b4271f0bdec4d2e5f8f2b9e9febced79048b4cd9c144ff3b832272ba76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633083217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9022428339d4615af519685439630f4532bb43a64f4c82f29c299271e16d0e56`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 27 Jul 2021 19:19:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:19:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:20:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:20:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:20:58 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:20:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:20:59 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:21:01 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:21:01 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:21:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:21:01 GMT
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
	-	`sha256:a6cdc5f71c3710468544fa224018c4a47ccf6c406ead41085cedf89ef99d1775`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e678d3290280e91fe94b0fc2b0faff059cab446516e5fb869856421c7001f4e`  
		Last Modified: Tue, 27 Jul 2021 19:23:43 GMT  
		Size: 598.1 MB (598112447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6969abcd0ca4371e2769bc97077e2f43ced0451abd159601e138e1edf5b1e283`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa359b4f22f914a20e211ae281fe312fe947736087893320e7c6543ccae9be`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07230fb0fa2e887a74bad436262a80d194b7ffe238041586fd2b4130b1e9c0d9`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9404dfab9613ac5843b1093f86d2cbaba3da74f61f3f5afb689f34b58298c55a`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73844eba4f0814d5e3f122bcd4fe4af5b787a43cad92054aa50926896fea85`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce7876a709925e51b4b5d0cee4cf4e000bf2bda2719984b15d8977e5256d50`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 125.9 KB (125889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f13caac7cd9de24759a20e590d18b3ce3c085c8ce971e0a023b96f4ed12c4f`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:005fb3ba97c2362b9ccc9d96f0d94bf09c2fe784d889fe71c5a2ba475e4645a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:f2a81b4271f0bdec4d2e5f8f2b9e9febced79048b4cd9c144ff3b832272ba76e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **633.1 MB (633083217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9022428339d4615af519685439630f4532bb43a64f4c82f29c299271e16d0e56`
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
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_VERSION=7.0.0
# Tue, 27 Jul 2021 19:19:36 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb
# Tue, 27 Jul 2021 19:19:37 GMT
ARG CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7
# Tue, 27 Jul 2021 19:19:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 27 Jul 2021 19:19:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 27 Jul 2021 19:20:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 27 Jul 2021 19:20:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 27 Jul 2021 19:20:58 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 27 Jul 2021 19:20:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 27 Jul 2021 19:20:59 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 27 Jul 2021 19:21:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0 CB_SHA256=6ce174d5ffd22ade6abbf44619e4126c6977635f58f7e08d09553b6b9f8117b7 CB_VERSION=7.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 27 Jul 2021 19:21:01 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 27 Jul 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 19:21:01 GMT
CMD ["couchbase-server"]
# Tue, 27 Jul 2021 19:21:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 27 Jul 2021 19:21:01 GMT
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
	-	`sha256:a6cdc5f71c3710468544fa224018c4a47ccf6c406ead41085cedf89ef99d1775`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e678d3290280e91fe94b0fc2b0faff059cab446516e5fb869856421c7001f4e`  
		Last Modified: Tue, 27 Jul 2021 19:23:43 GMT  
		Size: 598.1 MB (598112447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6969abcd0ca4371e2769bc97077e2f43ced0451abd159601e138e1edf5b1e283`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aa359b4f22f914a20e211ae281fe312fe947736087893320e7c6543ccae9be`  
		Last Modified: Tue, 27 Jul 2021 19:22:41 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07230fb0fa2e887a74bad436262a80d194b7ffe238041586fd2b4130b1e9c0d9`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9404dfab9613ac5843b1093f86d2cbaba3da74f61f3f5afb689f34b58298c55a`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73844eba4f0814d5e3f122bcd4fe4af5b787a43cad92054aa50926896fea85`  
		Last Modified: Tue, 27 Jul 2021 19:22:39 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce7876a709925e51b4b5d0cee4cf4e000bf2bda2719984b15d8977e5256d50`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 125.9 KB (125889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f13caac7cd9de24759a20e590d18b3ce3c085c8ce971e0a023b96f4ed12c4f`  
		Last Modified: Tue, 27 Jul 2021 19:22:38 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
