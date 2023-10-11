<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.26`](#emqx5026)
-	[`emqx:5.1`](#emqx51)
-	[`emqx:5.1.6`](#emqx516)
-	[`emqx:5.2`](#emqx52)
-	[`emqx:5.2.1`](#emqx521)
-	[`emqx:5.3`](#emqx53)
-	[`emqx:5.3.0`](#emqx530)
-	[`emqx:latest`](#emqxlatest)

## `emqx:5`

```console
$ docker pull emqx@sha256:b843614f4bd265f1bfc23456b36ec1680d9d2aa03e5a86a383cd513ea5a4f6af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:c15d3934cd5cc345a6de83e453187d7ac6048af2f7f48e5ee49778d3b44e43b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101097396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a530f25f4dc528e09bace9b17b6df83c9e6bfbd43ad1fa373e3f392543d587`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:46:42 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 21:46:42 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 21:46:42 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 21:46:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:57 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:46:57 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:57 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5022e31a6d4bd5f2e83b40a764b67efbff299d421465036e9aef04ededfc7c`  
		Last Modified: Wed, 11 Oct 2023 21:48:09 GMT  
		Size: 69.7 MB (69678633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d238e62b505ccb65d9f0a31d9f9c6d0109804d85120e13a314daf108f33cf15c`  
		Last Modified: Wed, 11 Oct 2023 21:48:00 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:434f538a77274155c3c36e769cf85061587ea13646b228007f9341d65a18b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91392162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33af0ed47222a6b07b7c37173a8804b2453adcc7fdfe9a4802e3c39f3994d6b4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:23 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 22:33:23 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 22:33:23 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 22:33:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:33:36 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:33:36 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:33:36 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:37 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c22a6b8bf4a0abd905adc5e5daf5df01b957d842cb3823a1d641434cf4afd4`  
		Last Modified: Wed, 11 Oct 2023 22:34:39 GMT  
		Size: 61.3 MB (61327172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d2956a29ac7156af4516b9eacab5be3a3a666f4a7b52aa57c15d4b768f3b4`  
		Last Modified: Wed, 11 Oct 2023 22:34:33 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:c5c965ae6eb66413638eb157cd372c385053b963918687e7a321324b4aee1b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:ecb2c3e19f891b5774a294f6f1777af8332f2bcdf096202756910c80f0b3600c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101983976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461e8f6fd57db1bc2c41e5da03cd0aa8c7dd1e6504bacebac387954481e48bb1`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:45:54 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:45:55 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 21:45:55 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 11 Oct 2023 21:45:55 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 11 Oct 2023 21:45:55 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 11 Oct 2023 21:45:55 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:03 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 11 Oct 2023 21:46:03 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:03 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:03 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:03 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:04 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:04 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa209cd30504d311a91bfefa773a6d235554ec0567920051188b9a5e14c72f`  
		Last Modified: Wed, 11 Oct 2023 21:47:13 GMT  
		Size: 3.0 MB (2989228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34c06ea6473194b32659f73afab7dc11e00c8588e28f324e5d8c397cde1c78`  
		Last Modified: Wed, 11 Oct 2023 21:47:12 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292897b8bd7d47f5909ca7d076d8d0f8d6480ac70168d40bb19c270209da0ce`  
		Last Modified: Wed, 11 Oct 2023 21:47:21 GMT  
		Size: 67.6 MB (67571871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da6e42f61d0b37187a2855cd3024889d689d2f3a769e6559a2f550edf40827`  
		Last Modified: Wed, 11 Oct 2023 21:47:12 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:48b2874e7042acd5a05c6177871b2958a3849b6dee2b5d7ead8773ff034944d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93064035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f992584d5bbda0a07c75ac49519545f10340b8d8a50c9c1f1d2a6a43c939b9ce`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:32:41 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 22:32:41 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 11 Oct 2023 22:32:41 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 11 Oct 2023 22:32:41 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 11 Oct 2023 22:32:41 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:32:48 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 11 Oct 2023 22:32:48 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:32:48 GMT
USER emqx
# Wed, 11 Oct 2023 22:32:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:32:48 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:32:48 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:32:49 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:32:49 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35268b46a5017b4ab4a19d82fdbce7cf5eebc19812e0371aa196060b28b83e4`  
		Last Modified: Wed, 11 Oct 2023 22:33:51 GMT  
		Size: 3.0 MB (3005523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7a4a4168e436f382bad41939f1b1f7e26a5fd9993b98e3f9c771f53b0544b`  
		Last Modified: Wed, 11 Oct 2023 22:33:50 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0669ace7d5cb617ec98e323ee2f9c127a9ab7e10d0712ea5193e27259d51d78`  
		Last Modified: Wed, 11 Oct 2023 22:33:56 GMT  
		Size: 60.0 MB (59989406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116d4a2cec76fb4f9635c6667466156b75b3a3366ccf768a8da18c02e27c42b7`  
		Last Modified: Wed, 11 Oct 2023 22:33:50 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:c5c965ae6eb66413638eb157cd372c385053b963918687e7a321324b4aee1b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:ecb2c3e19f891b5774a294f6f1777af8332f2bcdf096202756910c80f0b3600c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101983976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461e8f6fd57db1bc2c41e5da03cd0aa8c7dd1e6504bacebac387954481e48bb1`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:45:54 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:45:55 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 21:45:55 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 11 Oct 2023 21:45:55 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 11 Oct 2023 21:45:55 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 11 Oct 2023 21:45:55 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:03 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 11 Oct 2023 21:46:03 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:03 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:03 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:03 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:04 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:04 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:04 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa209cd30504d311a91bfefa773a6d235554ec0567920051188b9a5e14c72f`  
		Last Modified: Wed, 11 Oct 2023 21:47:13 GMT  
		Size: 3.0 MB (2989228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34c06ea6473194b32659f73afab7dc11e00c8588e28f324e5d8c397cde1c78`  
		Last Modified: Wed, 11 Oct 2023 21:47:12 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292897b8bd7d47f5909ca7d076d8d0f8d6480ac70168d40bb19c270209da0ce`  
		Last Modified: Wed, 11 Oct 2023 21:47:21 GMT  
		Size: 67.6 MB (67571871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da6e42f61d0b37187a2855cd3024889d689d2f3a769e6559a2f550edf40827`  
		Last Modified: Wed, 11 Oct 2023 21:47:12 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:48b2874e7042acd5a05c6177871b2958a3849b6dee2b5d7ead8773ff034944d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93064035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f992584d5bbda0a07c75ac49519545f10340b8d8a50c9c1f1d2a6a43c939b9ce`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:32:41 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 22:32:41 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 11 Oct 2023 22:32:41 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 11 Oct 2023 22:32:41 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 11 Oct 2023 22:32:41 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:32:48 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 11 Oct 2023 22:32:48 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:32:48 GMT
USER emqx
# Wed, 11 Oct 2023 22:32:48 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:32:48 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:32:48 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:32:49 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:32:49 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35268b46a5017b4ab4a19d82fdbce7cf5eebc19812e0371aa196060b28b83e4`  
		Last Modified: Wed, 11 Oct 2023 22:33:51 GMT  
		Size: 3.0 MB (3005523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7a4a4168e436f382bad41939f1b1f7e26a5fd9993b98e3f9c771f53b0544b`  
		Last Modified: Wed, 11 Oct 2023 22:33:50 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0669ace7d5cb617ec98e323ee2f9c127a9ab7e10d0712ea5193e27259d51d78`  
		Last Modified: Wed, 11 Oct 2023 22:33:56 GMT  
		Size: 60.0 MB (59989406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116d4a2cec76fb4f9635c6667466156b75b3a3366ccf768a8da18c02e27c42b7`  
		Last Modified: Wed, 11 Oct 2023 22:33:50 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:3f072d66765dbd8dfc5de99d82e3ff153ef62bd887a2d77ad95033c3b0098f3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:ec2663779d2c3e34693e771c928b34d60d3f8c7e03daa2e700ca79b1e61aac91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102393337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c899881376de7ece78eb2e097ba270933f1b8d463467cb181ba0394a21799dae`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:45:54 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:45:55 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 21:46:09 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 11 Oct 2023 21:46:09 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 11 Oct 2023 21:46:10 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 11 Oct 2023 21:46:10 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:18 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 11 Oct 2023 21:46:18 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:18 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:18 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:18 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:19 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:19 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa209cd30504d311a91bfefa773a6d235554ec0567920051188b9a5e14c72f`  
		Last Modified: Wed, 11 Oct 2023 21:47:13 GMT  
		Size: 3.0 MB (2989228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34c06ea6473194b32659f73afab7dc11e00c8588e28f324e5d8c397cde1c78`  
		Last Modified: Wed, 11 Oct 2023 21:47:12 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f7763ae254d2450a79e0d32c74aeb5ccc5bcda12877291dcfcb5c5d5f27fcc`  
		Last Modified: Wed, 11 Oct 2023 21:47:37 GMT  
		Size: 68.0 MB (67981232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ccd7d9527e6953efd6283253dbd8fd0666159bdd75850eb89a7ba656aa4647`  
		Last Modified: Wed, 11 Oct 2023 21:47:30 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:42ac54b2e3905656b356eb477be029e60465993616415e6bfd5b81d449891f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92699258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97c3cdab9ccb2f24ae341fe0422496ae37a057969e30a5a9515c91195add17d8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:32:41 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 22:32:52 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 11 Oct 2023 22:32:52 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 11 Oct 2023 22:32:52 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 11 Oct 2023 22:32:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:32:59 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 11 Oct 2023 22:32:59 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:32:59 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:00 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:00 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:00 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:00 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:00 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35268b46a5017b4ab4a19d82fdbce7cf5eebc19812e0371aa196060b28b83e4`  
		Last Modified: Wed, 11 Oct 2023 22:33:51 GMT  
		Size: 3.0 MB (3005523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7a4a4168e436f382bad41939f1b1f7e26a5fd9993b98e3f9c771f53b0544b`  
		Last Modified: Wed, 11 Oct 2023 22:33:50 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7560261d159ae5d277deb73dceb52f1981eebf07f1b9e82c2c8a46aad317a4`  
		Last Modified: Wed, 11 Oct 2023 22:34:10 GMT  
		Size: 59.6 MB (59624630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68b9c410de16d5181c03b376c69fee5185e244bc067cba6ff3f80e17383ac54`  
		Last Modified: Wed, 11 Oct 2023 22:34:05 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.6`

```console
$ docker pull emqx@sha256:3f072d66765dbd8dfc5de99d82e3ff153ef62bd887a2d77ad95033c3b0098f3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.6` - linux; amd64

```console
$ docker pull emqx@sha256:ec2663779d2c3e34693e771c928b34d60d3f8c7e03daa2e700ca79b1e61aac91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102393337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c899881376de7ece78eb2e097ba270933f1b8d463467cb181ba0394a21799dae`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:45:54 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:45:55 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 21:46:09 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 11 Oct 2023 21:46:09 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 11 Oct 2023 21:46:10 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 11 Oct 2023 21:46:10 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:18 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 11 Oct 2023 21:46:18 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:18 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:18 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:18 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:19 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:19 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa209cd30504d311a91bfefa773a6d235554ec0567920051188b9a5e14c72f`  
		Last Modified: Wed, 11 Oct 2023 21:47:13 GMT  
		Size: 3.0 MB (2989228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34c06ea6473194b32659f73afab7dc11e00c8588e28f324e5d8c397cde1c78`  
		Last Modified: Wed, 11 Oct 2023 21:47:12 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f7763ae254d2450a79e0d32c74aeb5ccc5bcda12877291dcfcb5c5d5f27fcc`  
		Last Modified: Wed, 11 Oct 2023 21:47:37 GMT  
		Size: 68.0 MB (67981232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ccd7d9527e6953efd6283253dbd8fd0666159bdd75850eb89a7ba656aa4647`  
		Last Modified: Wed, 11 Oct 2023 21:47:30 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1.6` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:42ac54b2e3905656b356eb477be029e60465993616415e6bfd5b81d449891f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92699258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97c3cdab9ccb2f24ae341fe0422496ae37a057969e30a5a9515c91195add17d8`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:40 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:32:41 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 22:32:52 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 11 Oct 2023 22:32:52 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 11 Oct 2023 22:32:52 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 11 Oct 2023 22:32:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:32:59 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 11 Oct 2023 22:32:59 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:32:59 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:00 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:00 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:00 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:00 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:00 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35268b46a5017b4ab4a19d82fdbce7cf5eebc19812e0371aa196060b28b83e4`  
		Last Modified: Wed, 11 Oct 2023 22:33:51 GMT  
		Size: 3.0 MB (3005523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7a4a4168e436f382bad41939f1b1f7e26a5fd9993b98e3f9c771f53b0544b`  
		Last Modified: Wed, 11 Oct 2023 22:33:50 GMT  
		Size: 4.1 KB (4118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7560261d159ae5d277deb73dceb52f1981eebf07f1b9e82c2c8a46aad317a4`  
		Last Modified: Wed, 11 Oct 2023 22:34:10 GMT  
		Size: 59.6 MB (59624630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68b9c410de16d5181c03b376c69fee5185e244bc067cba6ff3f80e17383ac54`  
		Last Modified: Wed, 11 Oct 2023 22:34:05 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2`

```console
$ docker pull emqx@sha256:95c660ccf1fd1d525a944c9bf6144f2d9b7113f18b6fe5b2293a23b800625315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2` - linux; amd64

```console
$ docker pull emqx@sha256:579037fc7a0b1ca6a2f20b77453c2100482879cc3e361ec68c3c9236ee4e2341
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101165525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2d51481f16d14a6e56ca7e4697086e1bb5612a81d98334010f2ddc39834e01`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:46:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:46:27 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 21:46:27 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 11 Oct 2023 21:46:27 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 11 Oct 2023 21:46:27 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 11 Oct 2023 21:46:27 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:39 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 11 Oct 2023 21:46:39 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:39 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:40 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e605d7342835e8b1937390366e8e0e6062ce5658585db78973ac5c9c4d00da`  
		Last Modified: Wed, 11 Oct 2023 21:47:45 GMT  
		Size: 1.6 MB (1631620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630774fe6b0f258370f809f00f663d8c27782d024bb5df41e5ee7e8ca313e08`  
		Last Modified: Wed, 11 Oct 2023 21:47:45 GMT  
		Size: 4.1 KB (4108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4b11056ab93ae57d3788f9567bdacc281ebd2a3e2b0cfdda8c26f84901a42`  
		Last Modified: Wed, 11 Oct 2023 21:47:52 GMT  
		Size: 68.1 MB (68111032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a19122283ab80c14cb137e49488eb589320bc11d86d8560eaf36bd73cc12967`  
		Last Modified: Wed, 11 Oct 2023 21:47:45 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.2` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fa56287144f52e9706770276a5d46fd504205d55f2ecfe13c35d8a5a56c054e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91466856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e4991302a34a702d8ccb84000284e1e397d01a423d78774cf23d646011767b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:07 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:33:08 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 22:33:08 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 11 Oct 2023 22:33:08 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 11 Oct 2023 22:33:08 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 11 Oct 2023 22:33:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:33:18 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 11 Oct 2023 22:33:19 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:33:19 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:19 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:19 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:19 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a2025c21d9db013c6c95e5faa344643ed0394567adf59154265c2c8d4b6e2c`  
		Last Modified: Wed, 11 Oct 2023 22:34:19 GMT  
		Size: 1.6 MB (1645882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad368c43a6f78e25d2dfd4138c309fc07bc80af2177013c6f0490e1bcef3074a`  
		Last Modified: Wed, 11 Oct 2023 22:34:18 GMT  
		Size: 4.1 KB (4122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decf55894f79f74740bf727a8c43931d07169e08a0460adb4bf32542a6218a79`  
		Last Modified: Wed, 11 Oct 2023 22:34:23 GMT  
		Size: 59.8 MB (59751864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a684a60f05707fd564ba059ffcc57d9b1763a7cae76f957ef10cae1fb8c42`  
		Last Modified: Wed, 11 Oct 2023 22:34:18 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2.1`

```console
$ docker pull emqx@sha256:95c660ccf1fd1d525a944c9bf6144f2d9b7113f18b6fe5b2293a23b800625315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2.1` - linux; amd64

```console
$ docker pull emqx@sha256:579037fc7a0b1ca6a2f20b77453c2100482879cc3e361ec68c3c9236ee4e2341
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101165525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2d51481f16d14a6e56ca7e4697086e1bb5612a81d98334010f2ddc39834e01`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:46:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:46:27 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 21:46:27 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 11 Oct 2023 21:46:27 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 11 Oct 2023 21:46:27 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 11 Oct 2023 21:46:27 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:39 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 11 Oct 2023 21:46:39 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:39 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:40 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e605d7342835e8b1937390366e8e0e6062ce5658585db78973ac5c9c4d00da`  
		Last Modified: Wed, 11 Oct 2023 21:47:45 GMT  
		Size: 1.6 MB (1631620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630774fe6b0f258370f809f00f663d8c27782d024bb5df41e5ee7e8ca313e08`  
		Last Modified: Wed, 11 Oct 2023 21:47:45 GMT  
		Size: 4.1 KB (4108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4b11056ab93ae57d3788f9567bdacc281ebd2a3e2b0cfdda8c26f84901a42`  
		Last Modified: Wed, 11 Oct 2023 21:47:52 GMT  
		Size: 68.1 MB (68111032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a19122283ab80c14cb137e49488eb589320bc11d86d8560eaf36bd73cc12967`  
		Last Modified: Wed, 11 Oct 2023 21:47:45 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.2.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:fa56287144f52e9706770276a5d46fd504205d55f2ecfe13c35d8a5a56c054e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91466856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e4991302a34a702d8ccb84000284e1e397d01a423d78774cf23d646011767b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:07 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:33:08 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 11 Oct 2023 22:33:08 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 11 Oct 2023 22:33:08 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 11 Oct 2023 22:33:08 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 11 Oct 2023 22:33:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:33:18 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 11 Oct 2023 22:33:19 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:33:19 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:19 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:19 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:19 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a2025c21d9db013c6c95e5faa344643ed0394567adf59154265c2c8d4b6e2c`  
		Last Modified: Wed, 11 Oct 2023 22:34:19 GMT  
		Size: 1.6 MB (1645882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad368c43a6f78e25d2dfd4138c309fc07bc80af2177013c6f0490e1bcef3074a`  
		Last Modified: Wed, 11 Oct 2023 22:34:18 GMT  
		Size: 4.1 KB (4122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decf55894f79f74740bf727a8c43931d07169e08a0460adb4bf32542a6218a79`  
		Last Modified: Wed, 11 Oct 2023 22:34:23 GMT  
		Size: 59.8 MB (59751864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a684a60f05707fd564ba059ffcc57d9b1763a7cae76f957ef10cae1fb8c42`  
		Last Modified: Wed, 11 Oct 2023 22:34:18 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3`

```console
$ docker pull emqx@sha256:b843614f4bd265f1bfc23456b36ec1680d9d2aa03e5a86a383cd513ea5a4f6af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3` - linux; amd64

```console
$ docker pull emqx@sha256:c15d3934cd5cc345a6de83e453187d7ac6048af2f7f48e5ee49778d3b44e43b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101097396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a530f25f4dc528e09bace9b17b6df83c9e6bfbd43ad1fa373e3f392543d587`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:46:42 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 21:46:42 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 21:46:42 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 21:46:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:57 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:46:57 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:57 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5022e31a6d4bd5f2e83b40a764b67efbff299d421465036e9aef04ededfc7c`  
		Last Modified: Wed, 11 Oct 2023 21:48:09 GMT  
		Size: 69.7 MB (69678633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d238e62b505ccb65d9f0a31d9f9c6d0109804d85120e13a314daf108f33cf15c`  
		Last Modified: Wed, 11 Oct 2023 21:48:00 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:434f538a77274155c3c36e769cf85061587ea13646b228007f9341d65a18b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91392162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33af0ed47222a6b07b7c37173a8804b2453adcc7fdfe9a4802e3c39f3994d6b4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:23 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 22:33:23 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 22:33:23 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 22:33:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:33:36 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:33:36 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:33:36 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:37 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c22a6b8bf4a0abd905adc5e5daf5df01b957d842cb3823a1d641434cf4afd4`  
		Last Modified: Wed, 11 Oct 2023 22:34:39 GMT  
		Size: 61.3 MB (61327172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d2956a29ac7156af4516b9eacab5be3a3a666f4a7b52aa57c15d4b768f3b4`  
		Last Modified: Wed, 11 Oct 2023 22:34:33 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3.0`

```console
$ docker pull emqx@sha256:b843614f4bd265f1bfc23456b36ec1680d9d2aa03e5a86a383cd513ea5a4f6af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3.0` - linux; amd64

```console
$ docker pull emqx@sha256:c15d3934cd5cc345a6de83e453187d7ac6048af2f7f48e5ee49778d3b44e43b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101097396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a530f25f4dc528e09bace9b17b6df83c9e6bfbd43ad1fa373e3f392543d587`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:46:42 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 21:46:42 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 21:46:42 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 21:46:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:57 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:46:57 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:57 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5022e31a6d4bd5f2e83b40a764b67efbff299d421465036e9aef04ededfc7c`  
		Last Modified: Wed, 11 Oct 2023 21:48:09 GMT  
		Size: 69.7 MB (69678633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d238e62b505ccb65d9f0a31d9f9c6d0109804d85120e13a314daf108f33cf15c`  
		Last Modified: Wed, 11 Oct 2023 21:48:00 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.3.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:434f538a77274155c3c36e769cf85061587ea13646b228007f9341d65a18b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91392162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33af0ed47222a6b07b7c37173a8804b2453adcc7fdfe9a4802e3c39f3994d6b4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:23 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 22:33:23 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 22:33:23 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 22:33:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:33:36 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:33:36 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:33:36 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:37 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c22a6b8bf4a0abd905adc5e5daf5df01b957d842cb3823a1d641434cf4afd4`  
		Last Modified: Wed, 11 Oct 2023 22:34:39 GMT  
		Size: 61.3 MB (61327172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d2956a29ac7156af4516b9eacab5be3a3a666f4a7b52aa57c15d4b768f3b4`  
		Last Modified: Wed, 11 Oct 2023 22:34:33 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:b843614f4bd265f1bfc23456b36ec1680d9d2aa03e5a86a383cd513ea5a4f6af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:c15d3934cd5cc345a6de83e453187d7ac6048af2f7f48e5ee49778d3b44e43b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101097396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a530f25f4dc528e09bace9b17b6df83c9e6bfbd43ad1fa373e3f392543d587`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:46:42 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 21:46:42 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 21:46:42 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 21:46:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 21:46:57 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:46:57 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 21:46:57 GMT
USER emqx
# Wed, 11 Oct 2023 21:46:57 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 21:46:58 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 21:46:58 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 21:46:58 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 21:46:58 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5022e31a6d4bd5f2e83b40a764b67efbff299d421465036e9aef04ededfc7c`  
		Last Modified: Wed, 11 Oct 2023 21:48:09 GMT  
		Size: 69.7 MB (69678633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d238e62b505ccb65d9f0a31d9f9c6d0109804d85120e13a314daf108f33cf15c`  
		Last Modified: Wed, 11 Oct 2023 21:48:00 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:434f538a77274155c3c36e769cf85061587ea13646b228007f9341d65a18b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91392162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33af0ed47222a6b07b7c37173a8804b2453adcc7fdfe9a4802e3c39f3994d6b4`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:23 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 11 Oct 2023 22:33:23 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 11 Oct 2023 22:33:23 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 11 Oct 2023 22:33:23 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 11 Oct 2023 22:33:36 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:33:36 GMT
WORKDIR /opt/emqx
# Wed, 11 Oct 2023 22:33:36 GMT
USER emqx
# Wed, 11 Oct 2023 22:33:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 11 Oct 2023 22:33:37 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 11 Oct 2023 22:33:37 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 11 Oct 2023 22:33:37 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:33:37 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c22a6b8bf4a0abd905adc5e5daf5df01b957d842cb3823a1d641434cf4afd4`  
		Last Modified: Wed, 11 Oct 2023 22:34:39 GMT  
		Size: 61.3 MB (61327172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d2956a29ac7156af4516b9eacab5be3a3a666f4a7b52aa57c15d4b768f3b4`  
		Last Modified: Wed, 11 Oct 2023 22:34:33 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
