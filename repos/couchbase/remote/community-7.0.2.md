## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:2c02dd364bd9364b2e1b8abe1f9964ccfbe6c172449d06d6eb088b3649411f00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:cb693c76d10b76312914e106fd08ad5bbfa6b0a1acc45193e8a3cc511c901620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429073076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3225058bc95cf03127581d0c8a8b26ffbc5372904936dc9e7e6fef56f3d98c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:31:16 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 02 Dec 2023 04:38:19 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:38:20 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_VERSION=7.0.2
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 02 Dec 2023 04:38:20 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 02 Dec 2023 04:38:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 02 Dec 2023 04:38:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 02 Dec 2023 04:39:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 02 Dec 2023 04:39:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 02 Dec 2023 04:39:14 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 02 Dec 2023 04:39:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 02 Dec 2023 04:39:14 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 02 Dec 2023 04:39:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 02 Dec 2023 04:39:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 02 Dec 2023 04:39:15 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 02 Dec 2023 04:39:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:39:16 GMT
CMD ["couchbase-server"]
# Sat, 02 Dec 2023 04:39:16 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 02 Dec 2023 04:39:16 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65927d84c24c98e842144855954f018a422bc7e00f62308c065f19ce0edf1e9e`  
		Last Modified: Sat, 02 Dec 2023 04:45:43 GMT  
		Size: 6.3 MB (6292702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612fc827a2f2cb20b9d45cf6f20bf4df15529289b1db462651dc590613d5901`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b40b79652403b877dcb2205c84dbd4ef60ef8351ec632f0787477e380f44361`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9126cbba021dd665a7466dbf63ecf40772147a5f61b215ab903fa7308613883`  
		Last Modified: Sat, 02 Dec 2023 04:46:23 GMT  
		Size: 394.1 MB (394062361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b67e25a6340abd393796f3d27833c93b91b8dd1f572c581aa3af4dfa6cb1576`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce50b39df7a855ee9e0d71b930af3b8ca6491ff8cee25ec1f242976060538843`  
		Last Modified: Sat, 02 Dec 2023 04:45:40 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f398ef2f2d335dce55c49e05380613b650449e15fa269b1d1bd245185748fc50`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c71a6e05d717a9ba3dd83ddade009d27f0404763464988dd365c88adc3a950`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa8c5c217a2ee26e891ce6ac87f0cc80cb3f310fd97da7ccb1ca150a2536ac8`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857a79c56d8629196a07236f53adc8d9705294ea30879cb95711279c481ce78d`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 129.5 KB (129508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecd8f43744f56644c9aedc42f287f21c38f2f11246a77ec01fd5fece7dd0336`  
		Last Modified: Sat, 02 Dec 2023 04:45:38 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
