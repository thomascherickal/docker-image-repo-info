## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:3353b2761c8ac27fadf97e732d8904b550810035472f1f45b6670fcd461ef7f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:a6f8a9279f2f62eaeec322e4bcf28552d00f3ba03b05d71e054eacce13133056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.1 MB (466123926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:def0c6c83222fed57640799409223d497156d61940529a6e1c422c3259d55441`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:42:52 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 19 Mar 2022 22:45:37 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 19 Mar 2022 22:45:38 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 19 Mar 2022 22:45:38 GMT
ARG CB_VERSION=6.0.5
# Sat, 19 Mar 2022 22:45:38 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Sat, 19 Mar 2022 22:45:38 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb
# Sat, 19 Mar 2022 22:45:38 GMT
ARG CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d
# Sat, 19 Mar 2022 22:45:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 19 Mar 2022 22:45:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 19 Mar 2022 22:46:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 19 Mar 2022 22:46:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 19 Mar 2022 22:46:36 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Sat, 19 Mar 2022 22:46:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 19 Mar 2022 22:46:37 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 19 Mar 2022 22:46:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 19 Mar 2022 22:46:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu18.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=6b152590867a58d771cffc22774d3cd66c916defcbeeeb339aca8d0a8e6d7f8d CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 19 Mar 2022 22:46:38 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 19 Mar 2022 22:46:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 22:46:38 GMT
CMD ["couchbase-server"]
# Sat, 19 Mar 2022 22:46:38 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 19 Mar 2022 22:46:38 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ef97d3b57baa12bf99cd3b939effb5659b3acd642fda6ae682d737c7c6f95a`  
		Last Modified: Sat, 19 Mar 2022 22:49:23 GMT  
		Size: 15.9 MB (15923032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd422578cde0d2abcc199efecc39b549f2726c88ca751cd9fd72503ea81decb`  
		Last Modified: Sat, 19 Mar 2022 22:49:17 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501af03c65c5525712dcd1cabd09fbd5d8f0f1c5d1fd50ac3f236bdf0bfffad`  
		Last Modified: Sat, 19 Mar 2022 22:49:17 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8387bd31bb25b3aa0ffe18b24fac7967176f32ea686710fd23f5dda55116c2f1`  
		Last Modified: Sat, 19 Mar 2022 22:49:55 GMT  
		Size: 423.4 MB (423362210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32790f8f7b4effcb587c3f9eb948bed2962b70fc95c740ff31166f528adf5dd5`  
		Last Modified: Sat, 19 Mar 2022 22:49:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f80be78ac52591e4d57757e4872aa313e5c92b78d6df33f450f66b1144776e3`  
		Last Modified: Sat, 19 Mar 2022 22:49:17 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cfd96c12768f9f02091b2df4233d1bf5423e22f8e76e7d9f131f8e134a609c`  
		Last Modified: Sat, 19 Mar 2022 22:49:15 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6c6a836f14faff73492333f7f423bcfe7a83525abb4e6d25fc193f13a39b30`  
		Last Modified: Sat, 19 Mar 2022 22:49:15 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9b5b150b59f9b4049e903ccbef7b14165a2e281eb6ad3a93f3658c392271b8`  
		Last Modified: Sat, 19 Mar 2022 22:49:15 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5919a088007955e867f23d069900de6372b1c1c6330fbbd7437d14364c44bc49`  
		Last Modified: Sat, 19 Mar 2022 22:49:15 GMT  
		Size: 125.6 KB (125562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e841459951187c730fe705c11a26dab3bb7c856af5524956857b08eafadaf0f4`  
		Last Modified: Sat, 19 Mar 2022 22:49:15 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
