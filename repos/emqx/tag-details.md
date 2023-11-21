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
-	[`emqx:5.3.1`](#emqx531)
-	[`emqx:latest`](#emqxlatest)

## `emqx:5`

```console
$ docker pull emqx@sha256:97b70b265fe39d031b8ff1db930e745d5acf4f46b4e649e6719235683e11aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:d0b529c14679337b41b26dd1dbcb3a9b5ea5786b6f5164a661fa941712b88eec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101375323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b71f409a7c567bc44d8ba4c8d8e454b2e34346342fd7bd70c75590d150de65e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Fri, 17 Nov 2023 01:30:07 GMT
ENV EMQX_VERSION=5.3.1
# Fri, 17 Nov 2023 01:30:07 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Fri, 17 Nov 2023 01:30:07 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Fri, 17 Nov 2023 01:30:07 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 17 Nov 2023 01:30:22 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 17 Nov 2023 01:30:22 GMT
WORKDIR /opt/emqx
# Fri, 17 Nov 2023 01:30:22 GMT
USER emqx
# Fri, 17 Nov 2023 01:30:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 17 Nov 2023 01:30:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 17 Nov 2023 01:30:22 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 17 Nov 2023 01:30:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 17 Nov 2023 01:30:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5476c671b1552718f0f720744d0c22c86f379d2980d0a484eba6693d015da9`  
		Last Modified: Fri, 17 Nov 2023 01:30:46 GMT  
		Size: 70.0 MB (69956505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d635eb32810b809b7a084c85d5398b7540bef45ed6f2631acfbb519e73f7647`  
		Last Modified: Fri, 17 Nov 2023 01:30:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cc31195c6e287ea408fe373fc4965c5c1f7c4f429b4fa16527a995ff55aa6646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91670521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1bc8d0c635b3a9d73f254605b5b742d7d7660cb2654f6408dd6e0013e62b9d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:15:08 GMT
ENV EMQX_VERSION=5.3.1
# Tue, 21 Nov 2023 10:15:08 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Tue, 21 Nov 2023 10:15:08 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Tue, 21 Nov 2023 10:15:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:15:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:15:21 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:15:21 GMT
USER emqx
# Tue, 21 Nov 2023 10:15:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:15:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:15:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:15:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:15:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56845559447cc0b30e74bba4e898455dc082c47b180e241fbe5fcf29b8aad6a6`  
		Last Modified: Tue, 21 Nov 2023 10:16:19 GMT  
		Size: 61.6 MB (61605495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920711b146ec99aae5eaa1087f4683ff0084f6680c2083921990b8cf776c907c`  
		Last Modified: Tue, 21 Nov 2023 10:16:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:873eed5c3646f248684b04b956fbab43b560cc390e2daf706f217316e64cdd07
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
$ docker pull emqx@sha256:f89cb986db2e3730ed2f341e97fdf25884bbc0399d66661e71c113819b97a1f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93063957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5458df38f77c0776658310f4b43c06d9ca8799009b2a531250034ad9c35ead08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:14:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:14:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 21 Nov 2023 10:14:26 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 21 Nov 2023 10:14:27 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 21 Nov 2023 10:14:27 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 21 Nov 2023 10:14:27 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:14:33 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 21 Nov 2023 10:14:33 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:14:33 GMT
USER emqx
# Tue, 21 Nov 2023 10:14:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:14:34 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:14:34 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:14:34 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:14:34 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99616413d6a3c8f46bb1ad7c165f4270383e4f1ab373749dfdf465d4b28d3b1`  
		Last Modified: Tue, 21 Nov 2023 10:15:34 GMT  
		Size: 3.0 MB (3005422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8420832c2bddea6c0722407cc6b4af4dda88c4471574dc495c5c96172c87ee10`  
		Last Modified: Tue, 21 Nov 2023 10:15:33 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302690fb5d6c617334f8f427f64bcfa8a096ee5eb1989f9d538bc9b77a743dd`  
		Last Modified: Tue, 21 Nov 2023 10:15:38 GMT  
		Size: 60.0 MB (59989401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc44771791f703c2cbccc632e122959d6ad817cd51760ecbb1330754a534814`  
		Last Modified: Tue, 21 Nov 2023 10:15:33 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.26`

```console
$ docker pull emqx@sha256:873eed5c3646f248684b04b956fbab43b560cc390e2daf706f217316e64cdd07
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
$ docker pull emqx@sha256:f89cb986db2e3730ed2f341e97fdf25884bbc0399d66661e71c113819b97a1f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93063957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5458df38f77c0776658310f4b43c06d9ca8799009b2a531250034ad9c35ead08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:14:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:14:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 21 Nov 2023 10:14:26 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 21 Nov 2023 10:14:27 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 21 Nov 2023 10:14:27 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 21 Nov 2023 10:14:27 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:14:33 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 21 Nov 2023 10:14:33 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:14:33 GMT
USER emqx
# Tue, 21 Nov 2023 10:14:34 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:14:34 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:14:34 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:14:34 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:14:34 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99616413d6a3c8f46bb1ad7c165f4270383e4f1ab373749dfdf465d4b28d3b1`  
		Last Modified: Tue, 21 Nov 2023 10:15:34 GMT  
		Size: 3.0 MB (3005422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8420832c2bddea6c0722407cc6b4af4dda88c4471574dc495c5c96172c87ee10`  
		Last Modified: Tue, 21 Nov 2023 10:15:33 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f302690fb5d6c617334f8f427f64bcfa8a096ee5eb1989f9d538bc9b77a743dd`  
		Last Modified: Tue, 21 Nov 2023 10:15:38 GMT  
		Size: 60.0 MB (59989401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc44771791f703c2cbccc632e122959d6ad817cd51760ecbb1330754a534814`  
		Last Modified: Tue, 21 Nov 2023 10:15:33 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1`

```console
$ docker pull emqx@sha256:94d52800c5907e2fe7495c46e9c4a006992f84d7c014f429772db2fc52fbbc30
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
$ docker pull emqx@sha256:07b7a50e930af503db65e70abe86b609c8a15c4a86593445fdc56838e7baf6b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92699251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96763b8adea3608145048364450554f13f7cc6d66f31993b0311d8a3f4ae46c3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:14:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:14:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 21 Nov 2023 10:14:37 GMT
ENV EMQX_VERSION=5.1.6
# Tue, 21 Nov 2023 10:14:37 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Tue, 21 Nov 2023 10:14:37 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Tue, 21 Nov 2023 10:14:37 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:14:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 21 Nov 2023 10:14:44 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:14:45 GMT
USER emqx
# Tue, 21 Nov 2023 10:14:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:14:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:14:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:14:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:14:45 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99616413d6a3c8f46bb1ad7c165f4270383e4f1ab373749dfdf465d4b28d3b1`  
		Last Modified: Tue, 21 Nov 2023 10:15:34 GMT  
		Size: 3.0 MB (3005422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8420832c2bddea6c0722407cc6b4af4dda88c4471574dc495c5c96172c87ee10`  
		Last Modified: Tue, 21 Nov 2023 10:15:33 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6586f1107540b703740d06516743a869e77bf4834608d86df574bbd6a05c5c5`  
		Last Modified: Tue, 21 Nov 2023 10:15:51 GMT  
		Size: 59.6 MB (59624697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e41a453a4e01c0571463168487cc2f093f2dcb9c9b4a582708b8f3d09b4a884`  
		Last Modified: Tue, 21 Nov 2023 10:15:46 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.1.6`

```console
$ docker pull emqx@sha256:94d52800c5907e2fe7495c46e9c4a006992f84d7c014f429772db2fc52fbbc30
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
$ docker pull emqx@sha256:07b7a50e930af503db65e70abe86b609c8a15c4a86593445fdc56838e7baf6b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92699251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96763b8adea3608145048364450554f13f7cc6d66f31993b0311d8a3f4ae46c3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:14:26 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:14:26 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 21 Nov 2023 10:14:37 GMT
ENV EMQX_VERSION=5.1.6
# Tue, 21 Nov 2023 10:14:37 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Tue, 21 Nov 2023 10:14:37 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Tue, 21 Nov 2023 10:14:37 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:14:44 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 21 Nov 2023 10:14:44 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:14:45 GMT
USER emqx
# Tue, 21 Nov 2023 10:14:45 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:14:45 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:14:45 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:14:45 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:14:45 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99616413d6a3c8f46bb1ad7c165f4270383e4f1ab373749dfdf465d4b28d3b1`  
		Last Modified: Tue, 21 Nov 2023 10:15:34 GMT  
		Size: 3.0 MB (3005422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8420832c2bddea6c0722407cc6b4af4dda88c4471574dc495c5c96172c87ee10`  
		Last Modified: Tue, 21 Nov 2023 10:15:33 GMT  
		Size: 4.1 KB (4107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6586f1107540b703740d06516743a869e77bf4834608d86df574bbd6a05c5c5`  
		Last Modified: Tue, 21 Nov 2023 10:15:51 GMT  
		Size: 59.6 MB (59624697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e41a453a4e01c0571463168487cc2f093f2dcb9c9b4a582708b8f3d09b4a884`  
		Last Modified: Tue, 21 Nov 2023 10:15:46 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2`

```console
$ docker pull emqx@sha256:15f34d71c67328482e9295b17023e7d06d33c72455fb7e63db295fa49670c0cf
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
$ docker pull emqx@sha256:338220eed5be331fe32fecf7cbfc097dd13e8bc97cf5942bf85e76ea11cd50e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91466707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab639b8c2c012166fb7a3cf4bf203a500068d017d8e5c02e0e845526f1434168`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:14:52 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:14:52 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 21 Nov 2023 10:14:52 GMT
ENV EMQX_VERSION=5.2.1
# Tue, 21 Nov 2023 10:14:53 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Tue, 21 Nov 2023 10:14:53 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Tue, 21 Nov 2023 10:14:53 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:15:02 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Tue, 21 Nov 2023 10:15:03 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:15:03 GMT
USER emqx
# Tue, 21 Nov 2023 10:15:03 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:15:03 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:15:03 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:15:03 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:15:03 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faf19c7b902a213dee90b0aec91abaf87bb600d398f3290b8970ece4baa5d0c`  
		Last Modified: Tue, 21 Nov 2023 10:16:00 GMT  
		Size: 1.6 MB (1645840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4370357dc913804e45c84e36d32603b076cef45d22699d6af105f5e53beab8`  
		Last Modified: Tue, 21 Nov 2023 10:16:00 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366a91635bf670cf46d7ccd8b9e31152e2ca016c0db782e8e151ca685ebfbeac`  
		Last Modified: Tue, 21 Nov 2023 10:16:05 GMT  
		Size: 59.8 MB (59751733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b2dddaacaf7357386cb7ab9c5d0557409e70080e99a04fad28dde0d5538cb6`  
		Last Modified: Tue, 21 Nov 2023 10:16:00 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.2.1`

```console
$ docker pull emqx@sha256:15f34d71c67328482e9295b17023e7d06d33c72455fb7e63db295fa49670c0cf
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
$ docker pull emqx@sha256:338220eed5be331fe32fecf7cbfc097dd13e8bc97cf5942bf85e76ea11cd50e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91466707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab639b8c2c012166fb7a3cf4bf203a500068d017d8e5c02e0e845526f1434168`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:14:52 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:14:52 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 21 Nov 2023 10:14:52 GMT
ENV EMQX_VERSION=5.2.1
# Tue, 21 Nov 2023 10:14:53 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Tue, 21 Nov 2023 10:14:53 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Tue, 21 Nov 2023 10:14:53 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:15:02 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Tue, 21 Nov 2023 10:15:03 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:15:03 GMT
USER emqx
# Tue, 21 Nov 2023 10:15:03 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:15:03 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:15:03 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:15:03 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:15:03 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faf19c7b902a213dee90b0aec91abaf87bb600d398f3290b8970ece4baa5d0c`  
		Last Modified: Tue, 21 Nov 2023 10:16:00 GMT  
		Size: 1.6 MB (1645840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4370357dc913804e45c84e36d32603b076cef45d22699d6af105f5e53beab8`  
		Last Modified: Tue, 21 Nov 2023 10:16:00 GMT  
		Size: 4.1 KB (4109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366a91635bf670cf46d7ccd8b9e31152e2ca016c0db782e8e151ca685ebfbeac`  
		Last Modified: Tue, 21 Nov 2023 10:16:05 GMT  
		Size: 59.8 MB (59751733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b2dddaacaf7357386cb7ab9c5d0557409e70080e99a04fad28dde0d5538cb6`  
		Last Modified: Tue, 21 Nov 2023 10:16:00 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3`

```console
$ docker pull emqx@sha256:97b70b265fe39d031b8ff1db930e745d5acf4f46b4e649e6719235683e11aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3` - linux; amd64

```console
$ docker pull emqx@sha256:d0b529c14679337b41b26dd1dbcb3a9b5ea5786b6f5164a661fa941712b88eec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101375323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b71f409a7c567bc44d8ba4c8d8e454b2e34346342fd7bd70c75590d150de65e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Fri, 17 Nov 2023 01:30:07 GMT
ENV EMQX_VERSION=5.3.1
# Fri, 17 Nov 2023 01:30:07 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Fri, 17 Nov 2023 01:30:07 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Fri, 17 Nov 2023 01:30:07 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 17 Nov 2023 01:30:22 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 17 Nov 2023 01:30:22 GMT
WORKDIR /opt/emqx
# Fri, 17 Nov 2023 01:30:22 GMT
USER emqx
# Fri, 17 Nov 2023 01:30:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 17 Nov 2023 01:30:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 17 Nov 2023 01:30:22 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 17 Nov 2023 01:30:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 17 Nov 2023 01:30:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5476c671b1552718f0f720744d0c22c86f379d2980d0a484eba6693d015da9`  
		Last Modified: Fri, 17 Nov 2023 01:30:46 GMT  
		Size: 70.0 MB (69956505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d635eb32810b809b7a084c85d5398b7540bef45ed6f2631acfbb519e73f7647`  
		Last Modified: Fri, 17 Nov 2023 01:30:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cc31195c6e287ea408fe373fc4965c5c1f7c4f429b4fa16527a995ff55aa6646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91670521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1bc8d0c635b3a9d73f254605b5b742d7d7660cb2654f6408dd6e0013e62b9d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:15:08 GMT
ENV EMQX_VERSION=5.3.1
# Tue, 21 Nov 2023 10:15:08 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Tue, 21 Nov 2023 10:15:08 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Tue, 21 Nov 2023 10:15:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:15:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:15:21 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:15:21 GMT
USER emqx
# Tue, 21 Nov 2023 10:15:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:15:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:15:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:15:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:15:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56845559447cc0b30e74bba4e898455dc082c47b180e241fbe5fcf29b8aad6a6`  
		Last Modified: Tue, 21 Nov 2023 10:16:19 GMT  
		Size: 61.6 MB (61605495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920711b146ec99aae5eaa1087f4683ff0084f6680c2083921990b8cf776c907c`  
		Last Modified: Tue, 21 Nov 2023 10:16:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3.1`

```console
$ docker pull emqx@sha256:97b70b265fe39d031b8ff1db930e745d5acf4f46b4e649e6719235683e11aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3.1` - linux; amd64

```console
$ docker pull emqx@sha256:d0b529c14679337b41b26dd1dbcb3a9b5ea5786b6f5164a661fa941712b88eec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101375323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b71f409a7c567bc44d8ba4c8d8e454b2e34346342fd7bd70c75590d150de65e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Fri, 17 Nov 2023 01:30:07 GMT
ENV EMQX_VERSION=5.3.1
# Fri, 17 Nov 2023 01:30:07 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Fri, 17 Nov 2023 01:30:07 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Fri, 17 Nov 2023 01:30:07 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 17 Nov 2023 01:30:22 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 17 Nov 2023 01:30:22 GMT
WORKDIR /opt/emqx
# Fri, 17 Nov 2023 01:30:22 GMT
USER emqx
# Fri, 17 Nov 2023 01:30:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 17 Nov 2023 01:30:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 17 Nov 2023 01:30:22 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 17 Nov 2023 01:30:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 17 Nov 2023 01:30:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5476c671b1552718f0f720744d0c22c86f379d2980d0a484eba6693d015da9`  
		Last Modified: Fri, 17 Nov 2023 01:30:46 GMT  
		Size: 70.0 MB (69956505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d635eb32810b809b7a084c85d5398b7540bef45ed6f2631acfbb519e73f7647`  
		Last Modified: Fri, 17 Nov 2023 01:30:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.3.1` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cc31195c6e287ea408fe373fc4965c5c1f7c4f429b4fa16527a995ff55aa6646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91670521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1bc8d0c635b3a9d73f254605b5b742d7d7660cb2654f6408dd6e0013e62b9d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:15:08 GMT
ENV EMQX_VERSION=5.3.1
# Tue, 21 Nov 2023 10:15:08 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Tue, 21 Nov 2023 10:15:08 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Tue, 21 Nov 2023 10:15:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:15:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:15:21 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:15:21 GMT
USER emqx
# Tue, 21 Nov 2023 10:15:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:15:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:15:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:15:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:15:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56845559447cc0b30e74bba4e898455dc082c47b180e241fbe5fcf29b8aad6a6`  
		Last Modified: Tue, 21 Nov 2023 10:16:19 GMT  
		Size: 61.6 MB (61605495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920711b146ec99aae5eaa1087f4683ff0084f6680c2083921990b8cf776c907c`  
		Last Modified: Tue, 21 Nov 2023 10:16:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:97b70b265fe39d031b8ff1db930e745d5acf4f46b4e649e6719235683e11aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:d0b529c14679337b41b26dd1dbcb3a9b5ea5786b6f5164a661fa941712b88eec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101375323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b71f409a7c567bc44d8ba4c8d8e454b2e34346342fd7bd70c75590d150de65e`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Fri, 17 Nov 2023 01:30:07 GMT
ENV EMQX_VERSION=5.3.1
# Fri, 17 Nov 2023 01:30:07 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Fri, 17 Nov 2023 01:30:07 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Fri, 17 Nov 2023 01:30:07 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 17 Nov 2023 01:30:22 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 17 Nov 2023 01:30:22 GMT
WORKDIR /opt/emqx
# Fri, 17 Nov 2023 01:30:22 GMT
USER emqx
# Fri, 17 Nov 2023 01:30:22 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 17 Nov 2023 01:30:22 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 17 Nov 2023 01:30:22 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 17 Nov 2023 01:30:22 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 17 Nov 2023 01:30:23 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5476c671b1552718f0f720744d0c22c86f379d2980d0a484eba6693d015da9`  
		Last Modified: Fri, 17 Nov 2023 01:30:46 GMT  
		Size: 70.0 MB (69956505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d635eb32810b809b7a084c85d5398b7540bef45ed6f2631acfbb519e73f7647`  
		Last Modified: Fri, 17 Nov 2023 01:30:39 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:cc31195c6e287ea408fe373fc4965c5c1f7c4f429b4fa16527a995ff55aa6646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91670521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1bc8d0c635b3a9d73f254605b5b742d7d7660cb2654f6408dd6e0013e62b9d`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:15:08 GMT
ENV EMQX_VERSION=5.3.1
# Tue, 21 Nov 2023 10:15:08 GMT
ENV AMD64_SHA256=1d13906b397e86e7822133d27d124bd06d714002293480047d5ac0e22d193fe2
# Tue, 21 Nov 2023 10:15:08 GMT
ENV ARM64_SHA256=e8aae039125194e9edb5dfbe8cf5c3eaf0e4bd2b9610fa97118d344115e31d2c
# Tue, 21 Nov 2023 10:15:08 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 21 Nov 2023 10:15:20 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:15:21 GMT
WORKDIR /opt/emqx
# Tue, 21 Nov 2023 10:15:21 GMT
USER emqx
# Tue, 21 Nov 2023 10:15:21 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 21 Nov 2023 10:15:21 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 21 Nov 2023 10:15:21 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 21 Nov 2023 10:15:21 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:15:21 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56845559447cc0b30e74bba4e898455dc082c47b180e241fbe5fcf29b8aad6a6`  
		Last Modified: Tue, 21 Nov 2023 10:16:19 GMT  
		Size: 61.6 MB (61605495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920711b146ec99aae5eaa1087f4683ff0084f6680c2083921990b8cf776c907c`  
		Last Modified: Tue, 21 Nov 2023 10:16:14 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
