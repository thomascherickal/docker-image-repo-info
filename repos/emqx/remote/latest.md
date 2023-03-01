## `emqx:latest`

```console
$ docker pull emqx@sha256:ac5b5c0abe4fca5c7021deba6626955b6f73a3d3729708a139f5cfbc70a43f33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:7b5f07c9a2de5626df4bcf9b120676522ff379c3b20d7060470fb67cbcf66d40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100382719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13c680478644672ceb0b19237bd2936f3b50df800a5b541fba5af6b777bb7a0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:03:25 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:03:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 05:03:26 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 05:03:26 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 05:03:26 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 05:03:26 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 05:03:32 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 05:03:32 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 05:03:32 GMT
USER emqx
# Wed, 01 Mar 2023 05:03:33 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 05:03:33 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 05:03:33 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 05:03:33 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:03:33 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a35a595ef04513102e76624112833df5aee4f5e7a95b61fa5eddc304211ab3`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 3.0 MB (2987679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e798ac719c7147c6c2faada408a48221abe27042dbc139527a475289fd20c98a`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90082bdef278a00e8f0f402c5d1d0d16842f414d5c26f1026e94c85a09e8c01`  
		Last Modified: Wed, 01 Mar 2023 05:04:27 GMT  
		Size: 66.0 MB (65978625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3520531f1aedaeb8f6657b0038a7910aadfbc1ac68d967315920e63f1d64e6f7`  
		Last Modified: Wed, 01 Mar 2023 05:04:19 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:d222de7e3082562495e7489361785d9afff79946b6f7cf539cdb413c925cd1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91481252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07131b1bf1a6771f2062969c0e108ec4a223c65b61d57d8f5eaccc2b04af83e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:21:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 03:21:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Mar 2023 03:21:17 GMT
ENV EMQX_VERSION=5.0.17
# Wed, 01 Mar 2023 03:21:17 GMT
ENV AMD64_SHA256=baed949959990ac18c12f35776a8ddf3b0bc4db3f7a855997e127b1fd1e7f1a7
# Wed, 01 Mar 2023 03:21:17 GMT
ENV ARM64_SHA256=1a2c40a71d55814e99207537616e4fec1c401fea77b53612c6d24dc7d55fe13d
# Wed, 01 Mar 2023 03:21:17 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Mar 2023 03:21:22 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Mar 2023 03:21:23 GMT
WORKDIR /opt/emqx
# Wed, 01 Mar 2023 03:21:23 GMT
USER emqx
# Wed, 01 Mar 2023 03:21:23 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Mar 2023 03:21:23 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Mar 2023 03:21:23 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Mar 2023 03:21:23 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 03:21:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38086ab7a191a5da95fb6158c384014d022c21f7e3615ad8b0cdd460c25f9035`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 3.0 MB (3002759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54eeac58f385f878614093545595a71c10cb909203557c85c1b5ef5defba64d`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 4.1 KB (4114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5876ed859c2399e42063251e048eb01628d191474154ee3e2692e01707e8c5`  
		Last Modified: Wed, 01 Mar 2023 03:22:10 GMT  
		Size: 58.4 MB (58410663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7ba419171d628ef2af2a2a9c4f4970ebc699c278af40d2d4fa9f8b097c7426`  
		Last Modified: Wed, 01 Mar 2023 03:22:04 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
