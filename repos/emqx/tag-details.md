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
-	[`emqx:5.3.2`](#emqx532)
-	[`emqx:latest`](#emqxlatest)

## `emqx:5`

```console
$ docker pull emqx@sha256:931752bb54d45278fc5c8959887a8844437a6c5960977b65b3db952f5dab1e8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:3c82206aac1aaacb33b4dfbac7f02448a55e5f3053a585229fd2a027e44e8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101780864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2318b222abc2a4ab5841d67867fb414afb31b74c577aeecea5b093627319b141`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:53:13 GMT
ENV EMQX_VERSION=5.3.2
# Tue, 19 Dec 2023 04:53:13 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Tue, 19 Dec 2023 04:53:13 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Tue, 19 Dec 2023 04:53:13 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:53:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:53:27 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:53:27 GMT
USER emqx
# Tue, 19 Dec 2023 04:53:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:53:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:53:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:53:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:53:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8584f03abcd8dc4f4e74091c8e788a0de343e4e28e45ce61f5c8e7fa8f21f`  
		Last Modified: Tue, 19 Dec 2023 04:54:37 GMT  
		Size: 70.4 MB (70362088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad325587982cabb9a450034ff1c3634132a7dd6fe384135965a76c9761f21`  
		Last Modified: Tue, 19 Dec 2023 04:54:29 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:37c5cef07e7ca8ff5746eb0778d1172837fcee5f699853fd85cddd77484364f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92080821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17daefdba2cb8879ebdc3f1ce47bfa5f09a982bb98b4c5003261280836a7731`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Fri, 01 Dec 2023 19:39:33 GMT
ENV EMQX_VERSION=5.3.2
# Fri, 01 Dec 2023 19:39:33 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Fri, 01 Dec 2023 19:39:33 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Fri, 01 Dec 2023 19:39:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 01 Dec 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 01 Dec 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Fri, 01 Dec 2023 19:39:46 GMT
USER emqx
# Fri, 01 Dec 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 01 Dec 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 01 Dec 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 01 Dec 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 01 Dec 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11963938c71fa3540543048bfc860754b6b00f59333d233f90245bf8d8d0aa09`  
		Last Modified: Fri, 01 Dec 2023 19:40:04 GMT  
		Size: 62.0 MB (62015793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2341b045d8fa3bf2f13f2da4e89afff038c3d568d50f164b64106b4dbc0f5dc`  
		Last Modified: Fri, 01 Dec 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:22f20e35009fddf341e7c9f6d5478af61804fc0c27da3637069ccbf3a242d6c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:cdb5d0d498c9a5c4dbfeecb52ae6d6d5b0ece96d123db939b61e87c6902ddbc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101984409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2850a60f42ca2924f7de4c8d39ef1bca056fdb7a38a2f9b5032992ec181b7698`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:52:30 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:52:31 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 19 Dec 2023 04:52:31 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 19 Dec 2023 04:52:31 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 19 Dec 2023 04:52:31 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 19 Dec 2023 04:52:31 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:52:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 19 Dec 2023 04:52:39 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:52:39 GMT
USER emqx
# Tue, 19 Dec 2023 04:52:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:52:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:52:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:52:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:52:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81485be977d1d3fe94a5b66b3785b7655ef00b2f45fd07342cd68fc243ae806`  
		Last Modified: Tue, 19 Dec 2023 04:53:43 GMT  
		Size: 3.0 MB (2989650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b109779462b5f5d7c8711d702009c239196c4c3f39bc2ac0ad12eddea7610c`  
		Last Modified: Tue, 19 Dec 2023 04:53:42 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9815b8a840a0468772652a27aaf7223b2bbc5149c76827b9381f86d513e14dbb`  
		Last Modified: Tue, 19 Dec 2023 04:53:50 GMT  
		Size: 67.6 MB (67571873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4084859a820e1b6016b1ebc5279bdb729b6470574e4bafffec22daf352fd5`  
		Last Modified: Tue, 19 Dec 2023 04:53:42 GMT  
		Size: 901.0 B  
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
$ docker pull emqx@sha256:22f20e35009fddf341e7c9f6d5478af61804fc0c27da3637069ccbf3a242d6c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.26` - linux; amd64

```console
$ docker pull emqx@sha256:cdb5d0d498c9a5c4dbfeecb52ae6d6d5b0ece96d123db939b61e87c6902ddbc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101984409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2850a60f42ca2924f7de4c8d39ef1bca056fdb7a38a2f9b5032992ec181b7698`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:52:30 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:52:31 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 19 Dec 2023 04:52:31 GMT
ENV EMQX_VERSION=5.0.26
# Tue, 19 Dec 2023 04:52:31 GMT
ENV AMD64_SHA256=00f954065fe7fd2f678f2e561578234240cc2cace49fb5cbb5aa7fb450825ffa
# Tue, 19 Dec 2023 04:52:31 GMT
ENV ARM64_SHA256=0b013f0b900e687c1ef3ed73bd6fef268b5492d12a3083ffd0d75c8e3935b4ae
# Tue, 19 Dec 2023 04:52:31 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:52:38 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Tue, 19 Dec 2023 04:52:39 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:52:39 GMT
USER emqx
# Tue, 19 Dec 2023 04:52:39 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:52:39 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:52:39 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:52:39 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:52:39 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81485be977d1d3fe94a5b66b3785b7655ef00b2f45fd07342cd68fc243ae806`  
		Last Modified: Tue, 19 Dec 2023 04:53:43 GMT  
		Size: 3.0 MB (2989650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b109779462b5f5d7c8711d702009c239196c4c3f39bc2ac0ad12eddea7610c`  
		Last Modified: Tue, 19 Dec 2023 04:53:42 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9815b8a840a0468772652a27aaf7223b2bbc5149c76827b9381f86d513e14dbb`  
		Last Modified: Tue, 19 Dec 2023 04:53:50 GMT  
		Size: 67.6 MB (67571873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4084859a820e1b6016b1ebc5279bdb729b6470574e4bafffec22daf352fd5`  
		Last Modified: Tue, 19 Dec 2023 04:53:42 GMT  
		Size: 901.0 B  
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
$ docker pull emqx@sha256:896e9c5861e25e3bc317eb3c093ff099b912acf05127482b8bfba797654ad8bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1` - linux; amd64

```console
$ docker pull emqx@sha256:931c0dca953709b7c00a0d214231ff8f56128a3e346f02e7859a06725c64ea1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102393797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb9d702579271a58adf5cbd49a7259b37f9f9c9597d610b09a3d36c85b0d4a9`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:52:30 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:52:31 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 19 Dec 2023 04:52:42 GMT
ENV EMQX_VERSION=5.1.6
# Tue, 19 Dec 2023 04:52:42 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Tue, 19 Dec 2023 04:52:42 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Tue, 19 Dec 2023 04:52:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:52:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 19 Dec 2023 04:52:49 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:52:49 GMT
USER emqx
# Tue, 19 Dec 2023 04:52:49 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:52:49 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:52:49 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:52:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:52:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81485be977d1d3fe94a5b66b3785b7655ef00b2f45fd07342cd68fc243ae806`  
		Last Modified: Tue, 19 Dec 2023 04:53:43 GMT  
		Size: 3.0 MB (2989650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b109779462b5f5d7c8711d702009c239196c4c3f39bc2ac0ad12eddea7610c`  
		Last Modified: Tue, 19 Dec 2023 04:53:42 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cf5dcb5939ce87deb069609859b228c88a3d3d02ce507c670f0392b1a2327`  
		Last Modified: Tue, 19 Dec 2023 04:54:06 GMT  
		Size: 68.0 MB (67981259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44819c1978424924f86ea06aaeba5105688cf831384d43cb43c9281626d97dc9`  
		Last Modified: Tue, 19 Dec 2023 04:53:59 GMT  
		Size: 903.0 B  
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
$ docker pull emqx@sha256:896e9c5861e25e3bc317eb3c093ff099b912acf05127482b8bfba797654ad8bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.1.6` - linux; amd64

```console
$ docker pull emqx@sha256:931c0dca953709b7c00a0d214231ff8f56128a3e346f02e7859a06725c64ea1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.4 MB (102393797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb9d702579271a58adf5cbd49a7259b37f9f9c9597d610b09a3d36c85b0d4a9`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:52:30 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:52:31 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 19 Dec 2023 04:52:42 GMT
ENV EMQX_VERSION=5.1.6
# Tue, 19 Dec 2023 04:52:42 GMT
ENV AMD64_SHA256=5c65f7538141e93d71d1dd7d088589339ef6a091b90f901604a2e0e004f5f4aa
# Tue, 19 Dec 2023 04:52:42 GMT
ENV ARM64_SHA256=ae832d29d6b4e7fa43f3bf04c8c9fad4c9047f079d1587d3ed2a3564d5ea8147
# Tue, 19 Dec 2023 04:52:42 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:52:49 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg
# Tue, 19 Dec 2023 04:52:49 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:52:49 GMT
USER emqx
# Tue, 19 Dec 2023 04:52:49 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:52:49 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:52:49 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:52:50 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:52:50 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81485be977d1d3fe94a5b66b3785b7655ef00b2f45fd07342cd68fc243ae806`  
		Last Modified: Tue, 19 Dec 2023 04:53:43 GMT  
		Size: 3.0 MB (2989650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b109779462b5f5d7c8711d702009c239196c4c3f39bc2ac0ad12eddea7610c`  
		Last Modified: Tue, 19 Dec 2023 04:53:42 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037cf5dcb5939ce87deb069609859b228c88a3d3d02ce507c670f0392b1a2327`  
		Last Modified: Tue, 19 Dec 2023 04:54:06 GMT  
		Size: 68.0 MB (67981259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44819c1978424924f86ea06aaeba5105688cf831384d43cb43c9281626d97dc9`  
		Last Modified: Tue, 19 Dec 2023 04:53:59 GMT  
		Size: 903.0 B  
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
$ docker pull emqx@sha256:6cecb27b0ff6effec56df4219b9222ba0add30f22f95cdcd2c66b6342f753401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2` - linux; amd64

```console
$ docker pull emqx@sha256:e876c8101026429cab210574ac2bd117511e1d53843361a77f58030df6099ba9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101165575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818b5c7436d0b8729dbf4b26ecd136ef3b2d04b4e5930822a7abcd359f9dac7c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:52:57 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:52:58 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 19 Dec 2023 04:52:58 GMT
ENV EMQX_VERSION=5.2.1
# Tue, 19 Dec 2023 04:52:58 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Tue, 19 Dec 2023 04:52:58 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Tue, 19 Dec 2023 04:52:58 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:53:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Tue, 19 Dec 2023 04:53:09 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:53:09 GMT
USER emqx
# Tue, 19 Dec 2023 04:53:10 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:53:10 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:53:10 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:53:10 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:53:10 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b84215a53870bb5e99e78f157dbed531d5dbcab34bc7cfa9039dbb7b6e0b922`  
		Last Modified: Tue, 19 Dec 2023 04:54:14 GMT  
		Size: 1.6 MB (1631630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0882c638bbfdc7dc76a191bb343f9f4f048b8d6b9575553c138e6a64c56dab3`  
		Last Modified: Tue, 19 Dec 2023 04:54:14 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13acbcf85d62dc5c3f01551b6f05db1bf332cbdd0e3f562d65ae7a3dbd360e0d`  
		Last Modified: Tue, 19 Dec 2023 04:54:21 GMT  
		Size: 68.1 MB (68111056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7d6988b322b2c7a63a38b08de3fca5bd98ecf78c8798b32616697c6d967843`  
		Last Modified: Tue, 19 Dec 2023 04:54:14 GMT  
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
$ docker pull emqx@sha256:6cecb27b0ff6effec56df4219b9222ba0add30f22f95cdcd2c66b6342f753401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.2.1` - linux; amd64

```console
$ docker pull emqx@sha256:e876c8101026429cab210574ac2bd117511e1d53843361a77f58030df6099ba9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101165575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818b5c7436d0b8729dbf4b26ecd136ef3b2d04b4e5930822a7abcd359f9dac7c`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:52:57 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:52:58 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Tue, 19 Dec 2023 04:52:58 GMT
ENV EMQX_VERSION=5.2.1
# Tue, 19 Dec 2023 04:52:58 GMT
ENV AMD64_SHA256=359a12811e5e6725e4269d9484abd348effdde35c0f2af1f5b63cae790c73020
# Tue, 19 Dec 2023 04:52:58 GMT
ENV ARM64_SHA256=2e0a3e0b33669c9b6da488970a2f92d08d7bd0824295822b205b83461ba4728d
# Tue, 19 Dec 2023 04:52:58 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:53:09 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl;     rm -rf /var/lib/apt/lists/*;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl
# Tue, 19 Dec 2023 04:53:09 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:53:09 GMT
USER emqx
# Tue, 19 Dec 2023 04:53:10 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:53:10 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:53:10 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:53:10 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:53:10 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b84215a53870bb5e99e78f157dbed531d5dbcab34bc7cfa9039dbb7b6e0b922`  
		Last Modified: Tue, 19 Dec 2023 04:54:14 GMT  
		Size: 1.6 MB (1631630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0882c638bbfdc7dc76a191bb343f9f4f048b8d6b9575553c138e6a64c56dab3`  
		Last Modified: Tue, 19 Dec 2023 04:54:14 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13acbcf85d62dc5c3f01551b6f05db1bf332cbdd0e3f562d65ae7a3dbd360e0d`  
		Last Modified: Tue, 19 Dec 2023 04:54:21 GMT  
		Size: 68.1 MB (68111056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7d6988b322b2c7a63a38b08de3fca5bd98ecf78c8798b32616697c6d967843`  
		Last Modified: Tue, 19 Dec 2023 04:54:14 GMT  
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
$ docker pull emqx@sha256:931752bb54d45278fc5c8959887a8844437a6c5960977b65b3db952f5dab1e8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3` - linux; amd64

```console
$ docker pull emqx@sha256:3c82206aac1aaacb33b4dfbac7f02448a55e5f3053a585229fd2a027e44e8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101780864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2318b222abc2a4ab5841d67867fb414afb31b74c577aeecea5b093627319b141`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:53:13 GMT
ENV EMQX_VERSION=5.3.2
# Tue, 19 Dec 2023 04:53:13 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Tue, 19 Dec 2023 04:53:13 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Tue, 19 Dec 2023 04:53:13 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:53:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:53:27 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:53:27 GMT
USER emqx
# Tue, 19 Dec 2023 04:53:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:53:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:53:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:53:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:53:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8584f03abcd8dc4f4e74091c8e788a0de343e4e28e45ce61f5c8e7fa8f21f`  
		Last Modified: Tue, 19 Dec 2023 04:54:37 GMT  
		Size: 70.4 MB (70362088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad325587982cabb9a450034ff1c3634132a7dd6fe384135965a76c9761f21`  
		Last Modified: Tue, 19 Dec 2023 04:54:29 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:37c5cef07e7ca8ff5746eb0778d1172837fcee5f699853fd85cddd77484364f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92080821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17daefdba2cb8879ebdc3f1ce47bfa5f09a982bb98b4c5003261280836a7731`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Fri, 01 Dec 2023 19:39:33 GMT
ENV EMQX_VERSION=5.3.2
# Fri, 01 Dec 2023 19:39:33 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Fri, 01 Dec 2023 19:39:33 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Fri, 01 Dec 2023 19:39:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 01 Dec 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 01 Dec 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Fri, 01 Dec 2023 19:39:46 GMT
USER emqx
# Fri, 01 Dec 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 01 Dec 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 01 Dec 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 01 Dec 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 01 Dec 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11963938c71fa3540543048bfc860754b6b00f59333d233f90245bf8d8d0aa09`  
		Last Modified: Fri, 01 Dec 2023 19:40:04 GMT  
		Size: 62.0 MB (62015793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2341b045d8fa3bf2f13f2da4e89afff038c3d568d50f164b64106b4dbc0f5dc`  
		Last Modified: Fri, 01 Dec 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.3.2`

```console
$ docker pull emqx@sha256:931752bb54d45278fc5c8959887a8844437a6c5960977b65b3db952f5dab1e8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.3.2` - linux; amd64

```console
$ docker pull emqx@sha256:3c82206aac1aaacb33b4dfbac7f02448a55e5f3053a585229fd2a027e44e8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101780864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2318b222abc2a4ab5841d67867fb414afb31b74c577aeecea5b093627319b141`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:53:13 GMT
ENV EMQX_VERSION=5.3.2
# Tue, 19 Dec 2023 04:53:13 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Tue, 19 Dec 2023 04:53:13 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Tue, 19 Dec 2023 04:53:13 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:53:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:53:27 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:53:27 GMT
USER emqx
# Tue, 19 Dec 2023 04:53:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:53:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:53:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:53:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:53:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8584f03abcd8dc4f4e74091c8e788a0de343e4e28e45ce61f5c8e7fa8f21f`  
		Last Modified: Tue, 19 Dec 2023 04:54:37 GMT  
		Size: 70.4 MB (70362088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad325587982cabb9a450034ff1c3634132a7dd6fe384135965a76c9761f21`  
		Last Modified: Tue, 19 Dec 2023 04:54:29 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.3.2` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:37c5cef07e7ca8ff5746eb0778d1172837fcee5f699853fd85cddd77484364f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92080821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17daefdba2cb8879ebdc3f1ce47bfa5f09a982bb98b4c5003261280836a7731`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Fri, 01 Dec 2023 19:39:33 GMT
ENV EMQX_VERSION=5.3.2
# Fri, 01 Dec 2023 19:39:33 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Fri, 01 Dec 2023 19:39:33 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Fri, 01 Dec 2023 19:39:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 01 Dec 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 01 Dec 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Fri, 01 Dec 2023 19:39:46 GMT
USER emqx
# Fri, 01 Dec 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 01 Dec 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 01 Dec 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 01 Dec 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 01 Dec 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11963938c71fa3540543048bfc860754b6b00f59333d233f90245bf8d8d0aa09`  
		Last Modified: Fri, 01 Dec 2023 19:40:04 GMT  
		Size: 62.0 MB (62015793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2341b045d8fa3bf2f13f2da4e89afff038c3d568d50f164b64106b4dbc0f5dc`  
		Last Modified: Fri, 01 Dec 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:931752bb54d45278fc5c8959887a8844437a6c5960977b65b3db952f5dab1e8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:3c82206aac1aaacb33b4dfbac7f02448a55e5f3053a585229fd2a027e44e8e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101780864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2318b222abc2a4ab5841d67867fb414afb31b74c577aeecea5b093627319b141`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:53:13 GMT
ENV EMQX_VERSION=5.3.2
# Tue, 19 Dec 2023 04:53:13 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Tue, 19 Dec 2023 04:53:13 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Tue, 19 Dec 2023 04:53:13 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Tue, 19 Dec 2023 04:53:27 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:53:27 GMT
WORKDIR /opt/emqx
# Tue, 19 Dec 2023 04:53:27 GMT
USER emqx
# Tue, 19 Dec 2023 04:53:27 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Tue, 19 Dec 2023 04:53:28 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Tue, 19 Dec 2023 04:53:28 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Tue, 19 Dec 2023 04:53:28 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 04:53:28 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c8584f03abcd8dc4f4e74091c8e788a0de343e4e28e45ce61f5c8e7fa8f21f`  
		Last Modified: Tue, 19 Dec 2023 04:54:37 GMT  
		Size: 70.4 MB (70362088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ad325587982cabb9a450034ff1c3634132a7dd6fe384135965a76c9761f21`  
		Last Modified: Tue, 19 Dec 2023 04:54:29 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:37c5cef07e7ca8ff5746eb0778d1172837fcee5f699853fd85cddd77484364f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92080821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17daefdba2cb8879ebdc3f1ce47bfa5f09a982bb98b4c5003261280836a7731`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Fri, 01 Dec 2023 19:39:33 GMT
ENV EMQX_VERSION=5.3.2
# Fri, 01 Dec 2023 19:39:33 GMT
ENV AMD64_SHA256=d5948d4171f57e77756dd6c9eeb745c39e391e75aad3798fce445f44f5690be0
# Fri, 01 Dec 2023 19:39:33 GMT
ENV ARM64_SHA256=82b056bb1c1cd1f16e9d0719150fa8ac19c499d29563738bcd6984b3c395c6ac
# Fri, 01 Dec 2023 19:39:33 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Fri, 01 Dec 2023 19:39:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends ca-certificates procps curl;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c;     mkdir /opt/emqx;     tar zxf $pkg -C /opt/emqx;     find /opt/emqx -name 'swagger*.js.map' -exec rm {} +;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -f $pkg;     apt-get purge -y --auto-remove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 01 Dec 2023 19:39:46 GMT
WORKDIR /opt/emqx
# Fri, 01 Dec 2023 19:39:46 GMT
USER emqx
# Fri, 01 Dec 2023 19:39:46 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Fri, 01 Dec 2023 19:39:46 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Fri, 01 Dec 2023 19:39:46 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Fri, 01 Dec 2023 19:39:46 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Fri, 01 Dec 2023 19:39:46 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11963938c71fa3540543048bfc860754b6b00f59333d233f90245bf8d8d0aa09`  
		Last Modified: Fri, 01 Dec 2023 19:40:04 GMT  
		Size: 62.0 MB (62015793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2341b045d8fa3bf2f13f2da4e89afff038c3d568d50f164b64106b4dbc0f5dc`  
		Last Modified: Fri, 01 Dec 2023 19:39:59 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
