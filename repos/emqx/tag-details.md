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
$ docker pull emqx@sha256:5d96db88bc148d14f6bb7ee2b2573e0baad26c955d010a7f4b7e4d09cad23e0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

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

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a7dea9af9700a776fb0e77081de9d7e6222d40b144d90940c7a5588a6ad05e45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91391993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9190172420bc4dcc7109eaa90101624a40c6223df73f4455f5ab0200d4d8dd90`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:09:10 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 01 Nov 2023 08:09:10 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 01 Nov 2023 08:09:10 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 01 Nov 2023 08:09:11 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:09:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:09:26 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:09:26 GMT
USER emqx
# Wed, 01 Nov 2023 08:09:26 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:09:27 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:09:27 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:09:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:09:27 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c326eb1a34ee42fc4124b1ad69319c25f18f1f618d47d9d60735589611e37219`  
		Last Modified: Wed, 01 Nov 2023 08:10:27 GMT  
		Size: 61.3 MB (61327184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62ac87e010b58bb6cff7eda950067b09c5797cbd9b5958267fe0b9869ad6c47`  
		Last Modified: Wed, 01 Nov 2023 08:10:21 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:0a7563024098f0da4f9e7878df6631ac48d1a5e94f4c770607d61eadd12e8f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:9c5491db12ef2ca83926d7ef125b7ca5caf7dd35b459112cad5cccc494c0f84e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101984009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76351e155569a72186d600f1c58b439c1f14ad7ce971fabb3c5496ba2817108b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:58:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:58:27 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 04:58:27 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 01 Nov 2023 04:58:28 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 01 Nov 2023 04:58:28 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 01 Nov 2023 04:58:28 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:58:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Nov 2023 04:58:39 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:58:39 GMT
USER emqx
# Wed, 01 Nov 2023 04:58:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:58:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:58:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:58:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:58:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe217836c5687c572b72a280ad71deb220e59ddcecc1922c819c5f83b1f6e5`  
		Last Modified: Wed, 01 Nov 2023 04:59:57 GMT  
		Size: 3.0 MB (2989237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38063d59296b0772b4e82c2bebe3c9e90c5370fa533729ffc8ed7162ef2fb44d`  
		Last Modified: Wed, 01 Nov 2023 04:59:56 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfd36fad3723fd34b5df7332c78ae3bfa76ed3f85b7e65ac77a6b811585a4a9`  
		Last Modified: Wed, 01 Nov 2023 05:00:05 GMT  
		Size: 67.6 MB (67571850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333968be826d130d0a687abf9c69d9b0e7b3ad0120226c4ddd78d8c1dbf848ae`  
		Last Modified: Wed, 01 Nov 2023 04:59:56 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:609905fd0c401659985738e799726ee3da1eb67bcbba06bd63d07374ac79ad4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93063836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d79965e6af88bbf8b5a17183813da6e12c8e276a202c472c1ed35117ae1945`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:08:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:08:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 08:08:17 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 01 Nov 2023 08:08:17 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 01 Nov 2023 08:08:17 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 01 Nov 2023 08:08:17 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:08:26 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Nov 2023 08:08:26 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:08:26 GMT
USER emqx
# Wed, 01 Nov 2023 08:08:26 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:08:26 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:08:26 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:08:26 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:08:27 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ea9b8eee5e1c638468f88309ebc15b04efc7f5ae00ef193c61013a282ace7e`  
		Last Modified: Wed, 01 Nov 2023 08:09:41 GMT  
		Size: 3.0 MB (3005512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb03a3fd3e4fab823f779ae247f0543343d565e3fdde3d1c1056a1c6a1cd30c8`  
		Last Modified: Wed, 01 Nov 2023 08:09:40 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f658c7a2d23050e6280a6f08c3170942ebee5ab107ccb7acc9f2e06dacf97058`  
		Last Modified: Wed, 01 Nov 2023 08:09:46 GMT  
		Size: 60.0 MB (59989403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d5299224073d8fc24a95adffacd67abaf38bb84836bc67aaa60035db1de81`  
		Last Modified: Wed, 01 Nov 2023 08:09:40 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:0a7563024098f0da4f9e7878df6631ac48d1a5e94f4c770607d61eadd12e8f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:9c5491db12ef2ca83926d7ef125b7ca5caf7dd35b459112cad5cccc494c0f84e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101984009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76351e155569a72186d600f1c58b439c1f14ad7ce971fabb3c5496ba2817108b`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:58:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:58:27 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 04:58:27 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 01 Nov 2023 04:58:28 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 01 Nov 2023 04:58:28 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 01 Nov 2023 04:58:28 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:58:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Nov 2023 04:58:39 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:58:39 GMT
USER emqx
# Wed, 01 Nov 2023 04:58:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:58:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:58:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:58:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:58:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe217836c5687c572b72a280ad71deb220e59ddcecc1922c819c5f83b1f6e5`  
		Last Modified: Wed, 01 Nov 2023 04:59:57 GMT  
		Size: 3.0 MB (2989237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38063d59296b0772b4e82c2bebe3c9e90c5370fa533729ffc8ed7162ef2fb44d`  
		Last Modified: Wed, 01 Nov 2023 04:59:56 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfd36fad3723fd34b5df7332c78ae3bfa76ed3f85b7e65ac77a6b811585a4a9`  
		Last Modified: Wed, 01 Nov 2023 05:00:05 GMT  
		Size: 67.6 MB (67571850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333968be826d130d0a687abf9c69d9b0e7b3ad0120226c4ddd78d8c1dbf848ae`  
		Last Modified: Wed, 01 Nov 2023 04:59:56 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.26` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:609905fd0c401659985738e799726ee3da1eb67bcbba06bd63d07374ac79ad4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93063836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d79965e6af88bbf8b5a17183813da6e12c8e276a202c472c1ed35117ae1945`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:08:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:08:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 08:08:17 GMT
ENV EMQX_VERSION=5.0.26
# Wed, 01 Nov 2023 08:08:17 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Wed, 01 Nov 2023 08:08:17 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Wed, 01 Nov 2023 08:08:17 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:08:26 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Wed, 01 Nov 2023 08:08:26 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:08:26 GMT
USER emqx
# Wed, 01 Nov 2023 08:08:26 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:08:26 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:08:26 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:08:26 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:08:27 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ea9b8eee5e1c638468f88309ebc15b04efc7f5ae00ef193c61013a282ace7e`  
		Last Modified: Wed, 01 Nov 2023 08:09:41 GMT  
		Size: 3.0 MB (3005512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb03a3fd3e4fab823f779ae247f0543343d565e3fdde3d1c1056a1c6a1cd30c8`  
		Last Modified: Wed, 01 Nov 2023 08:09:40 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f658c7a2d23050e6280a6f08c3170942ebee5ab107ccb7acc9f2e06dacf97058`  
		Last Modified: Wed, 01 Nov 2023 08:09:46 GMT  
		Size: 60.0 MB (59989403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d5299224073d8fc24a95adffacd67abaf38bb84836bc67aaa60035db1de81`  
		Last Modified: Wed, 01 Nov 2023 08:09:40 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:8ccb54b9af23e276a7b8ab3fac8a13b37c64fd61f15fc9d216e257a023ac2cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:c2a23946e6bbf14aa7fae5586d35821e8842c67369878a2f5d82ed004b050775
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102393414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ea1ae47560586da9327a21bf7acd1b465fa79a777271d44ee31e0a6d6ecbef`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:58:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:58:27 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 04:58:45 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 01 Nov 2023 04:58:45 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 01 Nov 2023 04:58:45 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 01 Nov 2023 04:58:45 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:58:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 01 Nov 2023 04:58:56 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:58:56 GMT
USER emqx
# Wed, 01 Nov 2023 04:58:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:58:57 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:58:57 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:58:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:58:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe217836c5687c572b72a280ad71deb220e59ddcecc1922c819c5f83b1f6e5`  
		Last Modified: Wed, 01 Nov 2023 04:59:57 GMT  
		Size: 3.0 MB (2989237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38063d59296b0772b4e82c2bebe3c9e90c5370fa533729ffc8ed7162ef2fb44d`  
		Last Modified: Wed, 01 Nov 2023 04:59:56 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03b7b5c3ba5b27a3db8de9bca56ad6d403808a562845c3682e66401ccf6022f`  
		Last Modified: Wed, 01 Nov 2023 05:00:25 GMT  
		Size: 68.0 MB (67981255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e252eafc3c62198309776738ab870e37b407fe34d854678738d5898eca19`  
		Last Modified: Wed, 01 Nov 2023 05:00:18 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:c034450b05b312b1556ac9d1a58dc6efdaf224859ce56d8223578f08b25b70c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92699045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949804345f2578ca21c51b0884923da610584d0883e42e6d866aaa7df35325f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:08:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:08:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 08:08:31 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 01 Nov 2023 08:08:31 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 01 Nov 2023 08:08:31 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 01 Nov 2023 08:08:31 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:08:43 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 01 Nov 2023 08:08:43 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:08:43 GMT
USER emqx
# Wed, 01 Nov 2023 08:08:43 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:08:43 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:08:43 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:08:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:08:43 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ea9b8eee5e1c638468f88309ebc15b04efc7f5ae00ef193c61013a282ace7e`  
		Last Modified: Wed, 01 Nov 2023 08:09:41 GMT  
		Size: 3.0 MB (3005512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb03a3fd3e4fab823f779ae247f0543343d565e3fdde3d1c1056a1c6a1cd30c8`  
		Last Modified: Wed, 01 Nov 2023 08:09:40 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa5d76d2cd744f1a35389cbb3601d69ba8687a241fe7b32e123ce4a7db6032d`  
		Last Modified: Wed, 01 Nov 2023 08:09:59 GMT  
		Size: 59.6 MB (59624611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee81301e82dfa1b8f7b20b1dbec2f7be49af6a86add078479c8ea83f2658c0ce`  
		Last Modified: Wed, 01 Nov 2023 08:09:54 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.6`

```console
$ docker pull emqx@sha256:8ccb54b9af23e276a7b8ab3fac8a13b37c64fd61f15fc9d216e257a023ac2cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.6` - linux; amd64

```console
$ docker pull emqx@sha256:c2a23946e6bbf14aa7fae5586d35821e8842c67369878a2f5d82ed004b050775
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102393414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ea1ae47560586da9327a21bf7acd1b465fa79a777271d44ee31e0a6d6ecbef`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:58:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:58:27 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 04:58:45 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 01 Nov 2023 04:58:45 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 01 Nov 2023 04:58:45 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 01 Nov 2023 04:58:45 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:58:56 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 01 Nov 2023 04:58:56 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:58:56 GMT
USER emqx
# Wed, 01 Nov 2023 04:58:56 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:58:57 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:58:57 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:58:57 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:58:57 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fe217836c5687c572b72a280ad71deb220e59ddcecc1922c819c5f83b1f6e5`  
		Last Modified: Wed, 01 Nov 2023 04:59:57 GMT  
		Size: 3.0 MB (2989237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38063d59296b0772b4e82c2bebe3c9e90c5370fa533729ffc8ed7162ef2fb44d`  
		Last Modified: Wed, 01 Nov 2023 04:59:56 GMT  
		Size: 4.1 KB (4105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03b7b5c3ba5b27a3db8de9bca56ad6d403808a562845c3682e66401ccf6022f`  
		Last Modified: Wed, 01 Nov 2023 05:00:25 GMT  
		Size: 68.0 MB (67981255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e252eafc3c62198309776738ab870e37b407fe34d854678738d5898eca19`  
		Last Modified: Wed, 01 Nov 2023 05:00:18 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.1.6` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:c034450b05b312b1556ac9d1a58dc6efdaf224859ce56d8223578f08b25b70c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92699045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:949804345f2578ca21c51b0884923da610584d0883e42e6d866aaa7df35325f0`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:08:16 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:08:17 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 08:08:31 GMT
ENV EMQX_VERSION=5.1.6
# Wed, 01 Nov 2023 08:08:31 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Wed, 01 Nov 2023 08:08:31 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Wed, 01 Nov 2023 08:08:31 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:08:43 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Wed, 01 Nov 2023 08:08:43 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:08:43 GMT
USER emqx
# Wed, 01 Nov 2023 08:08:43 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:08:43 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:08:43 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:08:43 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:08:43 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ea9b8eee5e1c638468f88309ebc15b04efc7f5ae00ef193c61013a282ace7e`  
		Last Modified: Wed, 01 Nov 2023 08:09:41 GMT  
		Size: 3.0 MB (3005512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb03a3fd3e4fab823f779ae247f0543343d565e3fdde3d1c1056a1c6a1cd30c8`  
		Last Modified: Wed, 01 Nov 2023 08:09:40 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa5d76d2cd744f1a35389cbb3601d69ba8687a241fe7b32e123ce4a7db6032d`  
		Last Modified: Wed, 01 Nov 2023 08:09:59 GMT  
		Size: 59.6 MB (59624611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee81301e82dfa1b8f7b20b1dbec2f7be49af6a86add078479c8ea83f2658c0ce`  
		Last Modified: Wed, 01 Nov 2023 08:09:54 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2`

```console
$ docker pull emqx@sha256:ffc7c30bfa5599592f93399beadc1cab37350b106b490e58cc834fd719d38a0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2` - linux; amd64

```console
$ docker pull emqx@sha256:6eb3ec201bff1b88852458b87c2c644a1a8d46f99ce8b2fbb2e667f38ae8846f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101165579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1fc404ec6700153e988d82c2556c233b80aa04bb4f1c32ec844f6fadffe154`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:59:04 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:59:04 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 04:59:05 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 01 Nov 2023 04:59:05 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 01 Nov 2023 04:59:05 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 01 Nov 2023 04:59:05 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:59:18 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 01 Nov 2023 04:59:19 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:59:19 GMT
USER emqx
# Wed, 01 Nov 2023 04:59:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:59:19 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:59:19 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:59:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:59:19 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573138db7004555fa87d2527352cb1283a3618a572a284110bbddc2e76c61521`  
		Last Modified: Wed, 01 Nov 2023 05:00:34 GMT  
		Size: 1.6 MB (1631629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999d1079ec0e6dfb1224326f8e2ed602bbe4e131dd1aca6af62eb28f51349678`  
		Last Modified: Wed, 01 Nov 2023 05:00:33 GMT  
		Size: 4.1 KB (4108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d3806e327889811435ede521c3961118d6f06531c6557526f058582e579322`  
		Last Modified: Wed, 01 Nov 2023 05:00:40 GMT  
		Size: 68.1 MB (68111024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabcb7a88a5ee8f7497a999d3b7c99492b448ee627d2e5e974b6e377c348cbf3`  
		Last Modified: Wed, 01 Nov 2023 05:00:34 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.2` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:0d3349f8f9d572758f5df2d200bed018a787644668ddf6bb64ca7f591ac2aa42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91466653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6c7507910c82264aded4c662b1ffdccf95fe7536868981d8d3cc3a1dcda31`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:08:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:08:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 08:08:52 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 01 Nov 2023 08:08:52 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 01 Nov 2023 08:08:52 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 01 Nov 2023 08:08:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:09:06 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 01 Nov 2023 08:09:06 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:09:06 GMT
USER emqx
# Wed, 01 Nov 2023 08:09:06 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:09:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:09:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:09:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:09:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bdeb9842c2751f0ecd4375678d5c51e80edf4a7fbeac18afc557ef0cf04cfc`  
		Last Modified: Wed, 01 Nov 2023 08:10:08 GMT  
		Size: 1.6 MB (1645885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aebca533594cfb1f2455d3647058bef1d42e5349479ac80f246cb1490254d25`  
		Last Modified: Wed, 01 Nov 2023 08:10:07 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee61e3f907fc201683e8585c1ab26324b055e508cf653aee07576420646ea24`  
		Last Modified: Wed, 01 Nov 2023 08:10:12 GMT  
		Size: 59.8 MB (59751849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936cf03ff804dd7714799f4ceb32ebb50e2d32282bc2471e35e8c34f240cf377`  
		Last Modified: Wed, 01 Nov 2023 08:10:07 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2.1`

```console
$ docker pull emqx@sha256:ffc7c30bfa5599592f93399beadc1cab37350b106b490e58cc834fd719d38a0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2.1` - linux; amd64

```console
$ docker pull emqx@sha256:6eb3ec201bff1b88852458b87c2c644a1a8d46f99ce8b2fbb2e667f38ae8846f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101165579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1fc404ec6700153e988d82c2556c233b80aa04bb4f1c32ec844f6fadffe154`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 04:59:04 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 04:59:04 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 04:59:05 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 01 Nov 2023 04:59:05 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 01 Nov 2023 04:59:05 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 01 Nov 2023 04:59:05 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 04:59:18 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 01 Nov 2023 04:59:19 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 04:59:19 GMT
USER emqx
# Wed, 01 Nov 2023 04:59:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 04:59:19 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 04:59:19 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 04:59:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 04:59:19 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573138db7004555fa87d2527352cb1283a3618a572a284110bbddc2e76c61521`  
		Last Modified: Wed, 01 Nov 2023 05:00:34 GMT  
		Size: 1.6 MB (1631629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999d1079ec0e6dfb1224326f8e2ed602bbe4e131dd1aca6af62eb28f51349678`  
		Last Modified: Wed, 01 Nov 2023 05:00:33 GMT  
		Size: 4.1 KB (4108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d3806e327889811435ede521c3961118d6f06531c6557526f058582e579322`  
		Last Modified: Wed, 01 Nov 2023 05:00:40 GMT  
		Size: 68.1 MB (68111024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabcb7a88a5ee8f7497a999d3b7c99492b448ee627d2e5e974b6e377c348cbf3`  
		Last Modified: Wed, 01 Nov 2023 05:00:34 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.2.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:0d3349f8f9d572758f5df2d200bed018a787644668ddf6bb64ca7f591ac2aa42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91466653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6c7507910c82264aded4c662b1ffdccf95fe7536868981d8d3cc3a1dcda31`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:08:51 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:08:51 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Wed, 01 Nov 2023 08:08:52 GMT
ENV EMQX_VERSION=5.2.1
# Wed, 01 Nov 2023 08:08:52 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Wed, 01 Nov 2023 08:08:52 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Wed, 01 Nov 2023 08:08:52 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:09:06 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Wed, 01 Nov 2023 08:09:06 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:09:06 GMT
USER emqx
# Wed, 01 Nov 2023 08:09:06 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:09:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:09:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:09:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:09:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bdeb9842c2751f0ecd4375678d5c51e80edf4a7fbeac18afc557ef0cf04cfc`  
		Last Modified: Wed, 01 Nov 2023 08:10:08 GMT  
		Size: 1.6 MB (1645885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aebca533594cfb1f2455d3647058bef1d42e5349479ac80f246cb1490254d25`  
		Last Modified: Wed, 01 Nov 2023 08:10:07 GMT  
		Size: 4.1 KB (4111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee61e3f907fc201683e8585c1ab26324b055e508cf653aee07576420646ea24`  
		Last Modified: Wed, 01 Nov 2023 08:10:12 GMT  
		Size: 59.8 MB (59751849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936cf03ff804dd7714799f4ceb32ebb50e2d32282bc2471e35e8c34f240cf377`  
		Last Modified: Wed, 01 Nov 2023 08:10:07 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3`

```console
$ docker pull emqx@sha256:5d96db88bc148d14f6bb7ee2b2573e0baad26c955d010a7f4b7e4d09cad23e0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3` - linux; amd64

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

### `emqx:5.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a7dea9af9700a776fb0e77081de9d7e6222d40b144d90940c7a5588a6ad05e45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91391993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9190172420bc4dcc7109eaa90101624a40c6223df73f4455f5ab0200d4d8dd90`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:09:10 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 01 Nov 2023 08:09:10 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 01 Nov 2023 08:09:10 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 01 Nov 2023 08:09:11 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:09:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:09:26 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:09:26 GMT
USER emqx
# Wed, 01 Nov 2023 08:09:26 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:09:27 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:09:27 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:09:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:09:27 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c326eb1a34ee42fc4124b1ad69319c25f18f1f618d47d9d60735589611e37219`  
		Last Modified: Wed, 01 Nov 2023 08:10:27 GMT  
		Size: 61.3 MB (61327184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62ac87e010b58bb6cff7eda950067b09c5797cbd9b5958267fe0b9869ad6c47`  
		Last Modified: Wed, 01 Nov 2023 08:10:21 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3.0`

```console
$ docker pull emqx@sha256:5d96db88bc148d14f6bb7ee2b2573e0baad26c955d010a7f4b7e4d09cad23e0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3.0` - linux; amd64

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

### `emqx:5.3.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:a7dea9af9700a776fb0e77081de9d7e6222d40b144d90940c7a5588a6ad05e45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91391993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9190172420bc4dcc7109eaa90101624a40c6223df73f4455f5ab0200d4d8dd90`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:09:10 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 01 Nov 2023 08:09:10 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 01 Nov 2023 08:09:10 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 01 Nov 2023 08:09:11 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:09:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:09:26 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:09:26 GMT
USER emqx
# Wed, 01 Nov 2023 08:09:26 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:09:27 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:09:27 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:09:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:09:27 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c326eb1a34ee42fc4124b1ad69319c25f18f1f618d47d9d60735589611e37219`  
		Last Modified: Wed, 01 Nov 2023 08:10:27 GMT  
		Size: 61.3 MB (61327184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62ac87e010b58bb6cff7eda950067b09c5797cbd9b5958267fe0b9869ad6c47`  
		Last Modified: Wed, 01 Nov 2023 08:10:21 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:5d96db88bc148d14f6bb7ee2b2573e0baad26c955d010a7f4b7e4d09cad23e0c
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
$ docker pull emqx@sha256:a7dea9af9700a776fb0e77081de9d7e6222d40b144d90940c7a5588a6ad05e45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91391993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9190172420bc4dcc7109eaa90101624a40c6223df73f4455f5ab0200d4d8dd90`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:09:10 GMT
ENV EMQX_VERSION=5.3.0
# Wed, 01 Nov 2023 08:09:10 GMT
ENV AMD64_SHA256=c534711d2a2b278e93dea33c2019f6e3b647f372a67e7a987ed7b0ca0984394d
# Wed, 01 Nov 2023 08:09:10 GMT
ENV ARM64_SHA256=1aa299f0ff04ed08af1fe4de37adbe888616ae203b7e38e81ef1f78b6f10527b
# Wed, 01 Nov 2023 08:09:11 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Wed, 01 Nov 2023 08:09:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:09:26 GMT
WORKDIR /opt/emqx
# Wed, 01 Nov 2023 08:09:26 GMT
USER emqx
# Wed, 01 Nov 2023 08:09:26 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Wed, 01 Nov 2023 08:09:27 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Wed, 01 Nov 2023 08:09:27 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Wed, 01 Nov 2023 08:09:27 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 08:09:27 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c326eb1a34ee42fc4124b1ad69319c25f18f1f618d47d9d60735589611e37219`  
		Last Modified: Wed, 01 Nov 2023 08:10:27 GMT  
		Size: 61.3 MB (61327184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62ac87e010b58bb6cff7eda950067b09c5797cbd9b5958267fe0b9869ad6c47`  
		Last Modified: Wed, 01 Nov 2023 08:10:21 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
