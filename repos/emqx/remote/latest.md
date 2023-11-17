## `emqx:latest`

```console
$ docker pull emqx@sha256:74171cb02a9a1966acc1030a1dd7bf64763f6b1dab9859a1ca3676fa0abac964
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:21ef166de954fa3d5e484d246397f566f81925dd6e342b0cbe3cb37c752de903
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101097450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a27e33fd542808bbc5aa2f3a9215a0d59cb745b3c04ac921b4e21b75b7132a8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:59:24 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 01 Nov 2023 04:59:24 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 01 Nov 2023 04:59:24 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 01 Nov 2023 04:59:24 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:59:42 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:59:42 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:59:42 GMT
USER emqx
# Wed, 01 Nov 2023 04:59:42 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:59:42 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:59:42 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:59:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:59:43 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa951f191d90609bdcffbad9dcbb57fb7bdd9f33c68aefc212df6f1d4cf58cc`  
		Last Modified: Wed, 01 Nov 2023 05:00:56 GMT  
		Size: 69.7 MB (69678633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c035ed70287908defdf38f8b1389b5f19a20fc3a23c6f778a1fd96f023e8cad`  
		Last Modified: Wed, 01 Nov 2023 05:00:48 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:044d25402ec1fbb0ac794169040f9ccef7cfa2834dc9481f690d700b2d007197
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91670415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe39a65837e11b60c614a427a6289e64882405f99b35458509ef480d3356f389`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Fri, 17 Nov 2023 00:43:30 GMT
ENV EMQX_VERSION=5.3.1
# Fri, 17 Nov 2023 00:43:30 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Fri, 17 Nov 2023 00:43:30 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Fri, 17 Nov 2023 00:43:30 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 17 Nov 2023 00:43:42 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 17 Nov 2023 00:43:43 GMT
WORKDIR /opt/emqx
# Fri, 17 Nov 2023 00:43:43 GMT
USER emqx
# Fri, 17 Nov 2023 00:43:43 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 17 Nov 2023 00:43:43 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 17 Nov 2023 00:43:43 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 17 Nov 2023 00:43:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 17 Nov 2023 00:43:43 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d41bcf8b9f5bb21a786ef390030a0b34974ca85493e38a5aaad0fe6432cb7e`  
		Last Modified: Fri, 17 Nov 2023 00:44:04 GMT  
		Size: 61.6 MB (61605607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe103fc99a0dd3bc752b5207b4884f92f7733c939f54774e4a8b060abf5784a9`  
		Last Modified: Fri, 17 Nov 2023 00:43:59 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
