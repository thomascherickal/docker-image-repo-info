## `couchbase:community`

```console
$ docker pull couchbase@sha256:ec52fa5b6c2ca9f21be48dc1c602b3a26c7d1d9b3c2f9ddbe37de18eee53876a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:cf2449931237e2d6eaf8efaf1368a996f5dfe6f4578f8c007ecbb099dda2c18e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429021949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb6b91c09609f50f5d5e8d98d0672ac8971c7acef492091d9d8cef2e71a9140`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 22:36:59 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 19 Mar 2022 22:39:00 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 19 Mar 2022 22:39:01 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Sat, 19 Mar 2022 22:39:01 GMT
ARG CB_VERSION=7.0.2
# Sat, 19 Mar 2022 22:39:01 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Sat, 19 Mar 2022 22:39:01 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Sat, 19 Mar 2022 22:39:01 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Sat, 19 Mar 2022 22:39:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 19 Mar 2022 22:39:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 19 Mar 2022 22:39:47 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 19 Mar 2022 22:39:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 19 Mar 2022 22:39:51 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Sat, 19 Mar 2022 22:39:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 19 Mar 2022 22:39:52 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 19 Mar 2022 22:39:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 19 Mar 2022 22:39:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Sat, 19 Mar 2022 22:39:53 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Sat, 19 Mar 2022 22:39:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 22:39:53 GMT
CMD ["couchbase-server"]
# Sat, 19 Mar 2022 22:39:53 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 19 Mar 2022 22:39:53 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646eb5ba07200e13b24f8842d10c852791cb95401e4f13a4918f5419b2cdbc36`  
		Last Modified: Sat, 19 Mar 2022 22:48:22 GMT  
		Size: 6.3 MB (6260726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f51b2ea8e6e2b1feb1c510e232c5cb4d1c11c4060999269993b809abaef069c`  
		Last Modified: Sat, 19 Mar 2022 22:48:19 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5860bb4feaf2acde5329b94c98aad09ea42c16ddf952c795678241de4fe72cf`  
		Last Modified: Sat, 19 Mar 2022 22:48:19 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493b0468b20fbd495bf942473a4e5b85768cff71895de07953cd86b23a93bfa`  
		Last Modified: Sat, 19 Mar 2022 22:49:05 GMT  
		Size: 394.1 MB (394061338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc9d1641b44db9400f2d6a591a40d053907da7c2560ebf4a3fd1297d512e0b3`  
		Last Modified: Sat, 19 Mar 2022 22:48:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e45de65f9fbd4687ef01ec87a2b06cb8d601f26c86268317463df8a3a46410a`  
		Last Modified: Sat, 19 Mar 2022 22:48:19 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bcd38fe0f668688aaddda1650e77b185834abc9964c0e9fb2aeb1af97e603e`  
		Last Modified: Sat, 19 Mar 2022 22:48:16 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555f00e9e0903b82bc7cabaa062a66f3b3df1a42ea4a731220608cc0a300b217`  
		Last Modified: Sat, 19 Mar 2022 22:48:16 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b1751a61784b39f12432e59b94ce238bb675696bf87e72faa333752974e713`  
		Last Modified: Sat, 19 Mar 2022 22:48:16 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506214df5d9d61cdd3f3aa6b087dbe2f1fffa52b77e2256a64f6ebdcc6928d80`  
		Last Modified: Sat, 19 Mar 2022 22:48:16 GMT  
		Size: 129.5 KB (129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c73fbf4b55f3e6f2ca2ea71e1bb5f9fef0cd51e4efe919c6d239f148a13dda1`  
		Last Modified: Sat, 19 Mar 2022 22:48:17 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
