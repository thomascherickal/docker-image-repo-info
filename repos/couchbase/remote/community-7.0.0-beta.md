## `couchbase:community-7.0.0-beta`

```console
$ docker pull couchbase@sha256:5d0008523237a9302b6484725bdf8e14857a9ce15545317d88e49862b578da6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:3b9810afe75f424a49322720be3a18d0b26b20cb8103ec8da32765bb99ae42e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.0 MB (434032981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb5a98d6d2a0c5a4af192f658a49de5c09c55c0e6e6d1df643a0ad4cdcf650f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:50:49 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 13 Jul 2021 23:51:15 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata man     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:51:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Tue, 13 Jul 2021 23:51:16 GMT
ARG CB_VERSION=7.0.0-beta
# Tue, 13 Jul 2021 23:51:17 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Tue, 13 Jul 2021 23:53:16 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb
# Tue, 13 Jul 2021 23:53:16 GMT
ARG CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9
# Tue, 13 Jul 2021 23:53:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 13 Jul 2021 23:53:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 13 Jul 2021 23:54:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 13 Jul 2021 23:54:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 13 Jul 2021 23:54:23 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Tue, 13 Jul 2021 23:54:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 13 Jul 2021 23:54:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:54:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 13 Jul 2021 23:54:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=51e843e9d2b5ef746353d79c044f17e4f9be0866673bd6fda01da27a0edf9fc9 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Tue, 13 Jul 2021 23:54:26 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Tue, 13 Jul 2021 23:54:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jul 2021 23:54:27 GMT
CMD ["couchbase-server"]
# Tue, 13 Jul 2021 23:54:27 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 13 Jul 2021 23:54:27 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d820bb660a9b14c611213779ee0deee8781268242fd7d51bd43a6e638f6722`  
		Last Modified: Wed, 14 Jul 2021 00:14:56 GMT  
		Size: 8.3 MB (8286840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db40d5a53531bbb33b0d3feb0be6f6fd03a142fba87ac62d5487adf1928a6673`  
		Last Modified: Wed, 14 Jul 2021 00:14:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3896078d2dbca6a7536e29984383c46920bf7cd3141ea6cac17ba8e4299977c`  
		Last Modified: Wed, 14 Jul 2021 00:16:12 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97842510154b16a7c5dbf2edac08fdc41c1e0c2d8e7ac46439fd9f47ef9f8256`  
		Last Modified: Wed, 14 Jul 2021 00:17:01 GMT  
		Size: 397.1 MB (397050034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7f231548a787819c593246d5329e54c2ad5668fdd4f614129d3ff3f8b3eb2c`  
		Last Modified: Wed, 14 Jul 2021 00:16:12 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8ed4e7f75eaa7ac8762e88f9b40be057826f25ee8060e5252874de967ce267`  
		Last Modified: Wed, 14 Jul 2021 00:16:12 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4378de9caaedf7a35ab05134cd9b174422ed1096c37b87b1018cfa0eea2b0994`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bca8b4c46801d47f5dfae3f3408f245f6b64d2da9c71dbadfb66a2eb8200704`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c26a2366d66674c927eaa6f700b9781176042547dcd91b0a0aca9baae54684`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f56fadf88bc02d02c5d7361306d960fd3a49320bff1a645af18ae5bd0c0d70`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 125.9 KB (125892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c819ee4ae2da728f31bf6f58740f18fe23ac33976bc62eb5d3ff41ea20d69ab`  
		Last Modified: Wed, 14 Jul 2021 00:16:10 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
