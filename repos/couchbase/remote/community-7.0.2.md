## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:cacc48d84f6cb0d217d76ef214325b25842bd6b8fe5af87a7675754e67846d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:5eecc82a485c2c8791b9c82672ac003ade5d3608366e3979b8561307337820ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429022236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a1babbec08293d5c0187fb2092a26ce27be742ec7d9f901f15b340dbb24a73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:07:34 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:35 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_VERSION=7.0.2
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 30 Apr 2022 00:07:35 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:07:36 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 30 Apr 2022 00:07:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:07:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:08:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:08:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:08:30 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:08:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:08:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:08:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 30 Apr 2022 00:08:32 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 30 Apr 2022 00:08:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:32 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:08:32 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:08:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3557df45000fab4a156d3d854e0e4e1fa62fc6744e80dd551b0cbe51261382`  
		Last Modified: Sat, 30 Apr 2022 00:19:32 GMT  
		Size: 6.3 MB (6260259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44832538c57317a4d2d2b80f48727f4d217252e0c1bca9c91764bd3c52a311f`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d30557d2ae3752e5656d5e84ddfae00bbe5f1ee403e60214744c746db794b3`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b022756e9eff4e2e5043cb6659cab72580afe823cb389bb288654a2fc7198c`  
		Last Modified: Sat, 30 Apr 2022 00:20:16 GMT  
		Size: 394.1 MB (394061761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54953e785e715fc3f75b5da9872ef7e4cd20b3722a207b4a7f618e7b15b68c4b`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365e976ccb685fa81ab103237d8da5e28ccc337555fdd76dcd3c0460a98a103b`  
		Last Modified: Sat, 30 Apr 2022 00:19:29 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da18e09f47baa880cfade31cac7432f3c5253afe94850de0ff5f68a9d6f3206c`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ecff6559e761c4792e2329e0fde5bb97f16ea8fc06f5fc3671a5ff5417786`  
		Last Modified: Sat, 30 Apr 2022 00:19:27 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062a2e7b179327ace70e89151a9cb12948137758865a2aa292d140a8f32090b5`  
		Last Modified: Sat, 30 Apr 2022 00:19:27 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068a0ecce2ebd008f15d64aa4c009579552ba84fd613c91906bd3efca784ab5e`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 129.5 KB (129509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1ef33dbf8866706153e7fe6b13631c7678e3c90427e5a23f0cdceadba7c100`  
		Last Modified: Sat, 30 Apr 2022 00:19:26 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
