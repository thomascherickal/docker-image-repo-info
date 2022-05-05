<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.6`](#crate46)
-	[`crate:4.6.8`](#crate468)
-	[`crate:4.7`](#crate47)
-	[`crate:4.7.2`](#crate472)
-	[`crate:4.8`](#crate48)
-	[`crate:4.8.0`](#crate480)
-	[`crate:latest`](#cratelatest)

## `crate:4.6`

```console
$ docker pull crate@sha256:64fd5119f66e902498610152dba07a27363df1f193d22730175bb8b09ee883b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.6` - linux; amd64

```console
$ docker pull crate@sha256:93632109a3539c26ed9a5b3f8697a4c375893fb70aea87b3953d76002a7e3fe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333298491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:489ec3cd90eda191854db4fa2f2b6fcfd796bed07ef007d4ce6ce274e0325e96`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 16 Mar 2022 00:26:02 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.8.tar.gz.asc crate-4.6.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.8.tar.gz.asc     && tar -xf crate-4.6.8.tar.gz -C /crate --strip-components=1     && rm crate-4.6.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 16 Mar 2022 00:26:35 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 16 Mar 2022 00:26:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:26:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 16 Mar 2022 00:26:36 GMT
RUN mkdir -p /data/data /data/log
# Wed, 16 Mar 2022 00:26:36 GMT
VOLUME [/data]
# Wed, 16 Mar 2022 00:26:36 GMT
WORKDIR /data
# Wed, 16 Mar 2022 00:26:36 GMT
EXPOSE 4200 4300 5432
# Wed, 16 Mar 2022 00:26:36 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 16 Mar 2022 00:26:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 16 Mar 2022 00:26:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-03-10T10:39:18.218424 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.8
# Wed, 16 Mar 2022 00:26:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 16 Mar 2022 00:26:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Mar 2022 00:26:37 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4eb0e6af56c8c0900122db7a6808def673a4ceecdb95b699f9ca0078c52c074`  
		Last Modified: Wed, 16 Mar 2022 00:27:56 GMT  
		Size: 255.6 MB (255614996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86f3db1f86fd161c20ebd210b3b5324dd3ab8647233685c86b30c4bcbf25d33`  
		Last Modified: Wed, 16 Mar 2022 00:27:34 GMT  
		Size: 1.6 MB (1582197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f230a107ddd6d942339256630c7882c616d8960b4103de7b877bfbf888f07876`  
		Last Modified: Wed, 16 Mar 2022 00:27:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e6a74bfead1f8a250143d841bef006617d5313413d2cafc929cfce7d4bd7df`  
		Last Modified: Wed, 16 Mar 2022 00:27:33 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce1768c7c5213b32777c5c631168cc1f348b7dd4c81383a44e6cd8f8cdaeeb`  
		Last Modified: Wed, 16 Mar 2022 00:27:33 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac286d124317b0d806c8fa98acf5372ffd61dc6c920f9dab724e15879a207fd`  
		Last Modified: Wed, 16 Mar 2022 00:27:34 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.6` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:a1c139662f1d9a0097994f00cfa81eec166a5db241942e491d5d2539238ad521
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b09b5df3b440fa883c5fb4c85438824fe354dc0c4d903c66059a09dc06572a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 16 Mar 2022 00:49:00 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.8.tar.gz.asc crate-4.6.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.8.tar.gz.asc     && tar -xf crate-4.6.8.tar.gz -C /crate --strip-components=1     && rm crate-4.6.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 16 Mar 2022 00:49:41 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 16 Mar 2022 00:49:41 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:49:42 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 16 Mar 2022 00:49:43 GMT
RUN mkdir -p /data/data /data/log
# Wed, 16 Mar 2022 00:49:44 GMT
VOLUME [/data]
# Wed, 16 Mar 2022 00:49:45 GMT
WORKDIR /data
# Wed, 16 Mar 2022 00:49:46 GMT
EXPOSE 4200 4300 5432
# Wed, 16 Mar 2022 00:49:48 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 16 Mar 2022 00:49:49 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 16 Mar 2022 00:49:49 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-03-10T10:39:18.218424 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.8
# Wed, 16 Mar 2022 00:49:51 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 16 Mar 2022 00:49:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Mar 2022 00:49:52 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18494ee0116ddb7fc6d9a1ff0335ba763062815df80185b5a5881aa9f266f226`  
		Last Modified: Wed, 16 Mar 2022 00:51:34 GMT  
		Size: 252.4 MB (252385074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ed3a573490ccb5e418acdc43a7fbcb30905113697e37b13362f68ddbdb308`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 1.6 MB (1580569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91af8584979695159a69fea1700f6771ac062c62f31760a3e0e3d6ad9fa6b0e`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb27b132f0d22f02542f83d53b087e79125b50d5fdc16092e8d75451ad1ec93`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd025c87bb8bb650250fe19913d0a21aa214a45d5109d79391a1ab7e975792b`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3982a4830b74dae916cc3e004fe05c1b44addb345a6fa47d2705dabfadb6717`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.6.8`

```console
$ docker pull crate@sha256:64fd5119f66e902498610152dba07a27363df1f193d22730175bb8b09ee883b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.6.8` - linux; amd64

```console
$ docker pull crate@sha256:93632109a3539c26ed9a5b3f8697a4c375893fb70aea87b3953d76002a7e3fe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333298491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:489ec3cd90eda191854db4fa2f2b6fcfd796bed07ef007d4ce6ce274e0325e96`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 16 Mar 2022 00:26:02 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.8.tar.gz.asc crate-4.6.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.8.tar.gz.asc     && tar -xf crate-4.6.8.tar.gz -C /crate --strip-components=1     && rm crate-4.6.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 16 Mar 2022 00:26:35 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 16 Mar 2022 00:26:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:26:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 16 Mar 2022 00:26:36 GMT
RUN mkdir -p /data/data /data/log
# Wed, 16 Mar 2022 00:26:36 GMT
VOLUME [/data]
# Wed, 16 Mar 2022 00:26:36 GMT
WORKDIR /data
# Wed, 16 Mar 2022 00:26:36 GMT
EXPOSE 4200 4300 5432
# Wed, 16 Mar 2022 00:26:36 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 16 Mar 2022 00:26:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 16 Mar 2022 00:26:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-03-10T10:39:18.218424 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.8
# Wed, 16 Mar 2022 00:26:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 16 Mar 2022 00:26:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Mar 2022 00:26:37 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4eb0e6af56c8c0900122db7a6808def673a4ceecdb95b699f9ca0078c52c074`  
		Last Modified: Wed, 16 Mar 2022 00:27:56 GMT  
		Size: 255.6 MB (255614996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86f3db1f86fd161c20ebd210b3b5324dd3ab8647233685c86b30c4bcbf25d33`  
		Last Modified: Wed, 16 Mar 2022 00:27:34 GMT  
		Size: 1.6 MB (1582197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f230a107ddd6d942339256630c7882c616d8960b4103de7b877bfbf888f07876`  
		Last Modified: Wed, 16 Mar 2022 00:27:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e6a74bfead1f8a250143d841bef006617d5313413d2cafc929cfce7d4bd7df`  
		Last Modified: Wed, 16 Mar 2022 00:27:33 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce1768c7c5213b32777c5c631168cc1f348b7dd4c81383a44e6cd8f8cdaeeb`  
		Last Modified: Wed, 16 Mar 2022 00:27:33 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac286d124317b0d806c8fa98acf5372ffd61dc6c920f9dab724e15879a207fd`  
		Last Modified: Wed, 16 Mar 2022 00:27:34 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.6.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:a1c139662f1d9a0097994f00cfa81eec166a5db241942e491d5d2539238ad521
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b09b5df3b440fa883c5fb4c85438824fe354dc0c4d903c66059a09dc06572a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 16 Mar 2022 00:49:00 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.8.tar.gz.asc crate-4.6.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.8.tar.gz.asc     && tar -xf crate-4.6.8.tar.gz -C /crate --strip-components=1     && rm crate-4.6.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 16 Mar 2022 00:49:41 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 16 Mar 2022 00:49:41 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Mar 2022 00:49:42 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 16 Mar 2022 00:49:43 GMT
RUN mkdir -p /data/data /data/log
# Wed, 16 Mar 2022 00:49:44 GMT
VOLUME [/data]
# Wed, 16 Mar 2022 00:49:45 GMT
WORKDIR /data
# Wed, 16 Mar 2022 00:49:46 GMT
EXPOSE 4200 4300 5432
# Wed, 16 Mar 2022 00:49:48 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 16 Mar 2022 00:49:49 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 16 Mar 2022 00:49:49 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-03-10T10:39:18.218424 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.8
# Wed, 16 Mar 2022 00:49:51 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 16 Mar 2022 00:49:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Mar 2022 00:49:52 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18494ee0116ddb7fc6d9a1ff0335ba763062815df80185b5a5881aa9f266f226`  
		Last Modified: Wed, 16 Mar 2022 00:51:34 GMT  
		Size: 252.4 MB (252385074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ed3a573490ccb5e418acdc43a7fbcb30905113697e37b13362f68ddbdb308`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 1.6 MB (1580569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91af8584979695159a69fea1700f6771ac062c62f31760a3e0e3d6ad9fa6b0e`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb27b132f0d22f02542f83d53b087e79125b50d5fdc16092e8d75451ad1ec93`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd025c87bb8bb650250fe19913d0a21aa214a45d5109d79391a1ab7e975792b`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3982a4830b74dae916cc3e004fe05c1b44addb345a6fa47d2705dabfadb6717`  
		Last Modified: Wed, 16 Mar 2022 00:51:04 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.7`

```console
$ docker pull crate@sha256:81c83e381596e67eb1eebd205e5f93bd08041c466003b4931dd0f0d6bddcff7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.7` - linux; amd64

```console
$ docker pull crate@sha256:35d27d99309729016a6adff1ed535fde77174e13e27d2d05b5374ad40c615e78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.4 MB (324429897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e954b92c04c03b8b845c7a420b3335ba5d361b9388163df2f8b15a7585fb52ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 18:25:14 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.2.tar.gz.asc crate-4.7.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.2.tar.gz.asc     && tar -xf crate-4.7.2.tar.gz -C /crate --strip-components=1     && rm crate-4.7.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 18:25:17 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 18:25:17 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:25:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 18:25:18 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 18:25:18 GMT
VOLUME [/data]
# Thu, 05 May 2022 18:25:18 GMT
WORKDIR /data
# Thu, 05 May 2022 18:25:18 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 18:25:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 18:25:18 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 18:25:18 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T15:02:07.791462 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.2
# Thu, 05 May 2022 18:25:18 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 18:25:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 18:25:19 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6ca85c7cd29488e315a6d29c62fab42c4dd489189669126cfa0aef45cc75af`  
		Last Modified: Thu, 05 May 2022 18:26:32 GMT  
		Size: 246.7 MB (246746404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9192d6a458ebcfcb2adf44f842c86346428a85a614bd1b6eec93d6579505eac`  
		Last Modified: Thu, 05 May 2022 18:26:10 GMT  
		Size: 1.6 MB (1582193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c3eebddf3509627d01cbc521f8bbe95bc05d3aa453dc2e17dcb2c52dfc2aeb`  
		Last Modified: Thu, 05 May 2022 18:26:10 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad80830d8dd678f6c0f50ee9e177809a2ee9cd8543514430748753199c4ecfb`  
		Last Modified: Thu, 05 May 2022 18:26:09 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f70ea48b7ca739f795d34f193092dcf0527056501c140d0fb1159854aa8b26b`  
		Last Modified: Thu, 05 May 2022 18:26:09 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d57d2b6f3f33bd86371b559a4f8cba8803ea1a5b23e6b24fa21728ff042b22`  
		Last Modified: Thu, 05 May 2022 18:26:10 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.7` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:1f3792136d75b00bc6e2bc55c6ac319f76e6f446f42d1ba5925fbcc58e2a5834
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.6 MB (354610631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418d6cf52b07eebfade75e7b20c2e211f0ea11d719e307d3bf00e01165400ebf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 17:42:20 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.2.tar.gz.asc crate-4.7.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.2.tar.gz.asc     && tar -xf crate-4.7.2.tar.gz -C /crate --strip-components=1     && rm crate-4.7.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 17:42:22 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 17:42:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:42:24 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 17:42:26 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 17:42:26 GMT
VOLUME [/data]
# Thu, 05 May 2022 17:42:27 GMT
WORKDIR /data
# Thu, 05 May 2022 17:42:28 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 17:42:30 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 17:42:31 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 17:42:31 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T15:02:07.791462 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.2
# Thu, 05 May 2022 17:42:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 17:42:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 17:42:34 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83c3f0282326f4382421f0068284bae413d2e9a017eb6c41543dd40d7f3ca5c`  
		Last Modified: Thu, 05 May 2022 17:44:13 GMT  
		Size: 244.7 MB (244651051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3625ed13d49464247a4da30c7f8445daaf1ac1f3a2ad147c41ad1244c941072`  
		Last Modified: Thu, 05 May 2022 17:43:47 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c3dcce143896e547b3ce248733db76c4e4f7a18dad5e212675b431cf1a1402`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6ece29da35e7124ee4aea0b44d4f297143a35e64e2fd0afa9a61f3f7e85647`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809b2c7787a28aa760f2b39e58ad6793d1ea69189e8eccd7b93bfa31db405a7c`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e38abec161e7fb952f266511e7d01ec2ccab71f8debcf2c9221e3d4fbf878`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.7.2`

```console
$ docker pull crate@sha256:81c83e381596e67eb1eebd205e5f93bd08041c466003b4931dd0f0d6bddcff7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.7.2` - linux; amd64

```console
$ docker pull crate@sha256:35d27d99309729016a6adff1ed535fde77174e13e27d2d05b5374ad40c615e78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.4 MB (324429897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e954b92c04c03b8b845c7a420b3335ba5d361b9388163df2f8b15a7585fb52ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 18:25:14 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.2.tar.gz.asc crate-4.7.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.2.tar.gz.asc     && tar -xf crate-4.7.2.tar.gz -C /crate --strip-components=1     && rm crate-4.7.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 18:25:17 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 18:25:17 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:25:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 18:25:18 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 18:25:18 GMT
VOLUME [/data]
# Thu, 05 May 2022 18:25:18 GMT
WORKDIR /data
# Thu, 05 May 2022 18:25:18 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 18:25:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 18:25:18 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 18:25:18 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T15:02:07.791462 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.2
# Thu, 05 May 2022 18:25:18 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 18:25:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 18:25:19 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6ca85c7cd29488e315a6d29c62fab42c4dd489189669126cfa0aef45cc75af`  
		Last Modified: Thu, 05 May 2022 18:26:32 GMT  
		Size: 246.7 MB (246746404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9192d6a458ebcfcb2adf44f842c86346428a85a614bd1b6eec93d6579505eac`  
		Last Modified: Thu, 05 May 2022 18:26:10 GMT  
		Size: 1.6 MB (1582193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c3eebddf3509627d01cbc521f8bbe95bc05d3aa453dc2e17dcb2c52dfc2aeb`  
		Last Modified: Thu, 05 May 2022 18:26:10 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad80830d8dd678f6c0f50ee9e177809a2ee9cd8543514430748753199c4ecfb`  
		Last Modified: Thu, 05 May 2022 18:26:09 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f70ea48b7ca739f795d34f193092dcf0527056501c140d0fb1159854aa8b26b`  
		Last Modified: Thu, 05 May 2022 18:26:09 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d57d2b6f3f33bd86371b559a4f8cba8803ea1a5b23e6b24fa21728ff042b22`  
		Last Modified: Thu, 05 May 2022 18:26:10 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.7.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:1f3792136d75b00bc6e2bc55c6ac319f76e6f446f42d1ba5925fbcc58e2a5834
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.6 MB (354610631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418d6cf52b07eebfade75e7b20c2e211f0ea11d719e307d3bf00e01165400ebf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 17:42:20 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.2.tar.gz.asc crate-4.7.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.2.tar.gz.asc     && tar -xf crate-4.7.2.tar.gz -C /crate --strip-components=1     && rm crate-4.7.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 17:42:22 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 17:42:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:42:24 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 17:42:26 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 17:42:26 GMT
VOLUME [/data]
# Thu, 05 May 2022 17:42:27 GMT
WORKDIR /data
# Thu, 05 May 2022 17:42:28 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 17:42:30 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 17:42:31 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 17:42:31 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T15:02:07.791462 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.2
# Thu, 05 May 2022 17:42:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 17:42:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 17:42:34 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83c3f0282326f4382421f0068284bae413d2e9a017eb6c41543dd40d7f3ca5c`  
		Last Modified: Thu, 05 May 2022 17:44:13 GMT  
		Size: 244.7 MB (244651051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3625ed13d49464247a4da30c7f8445daaf1ac1f3a2ad147c41ad1244c941072`  
		Last Modified: Thu, 05 May 2022 17:43:47 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c3dcce143896e547b3ce248733db76c4e4f7a18dad5e212675b431cf1a1402`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6ece29da35e7124ee4aea0b44d4f297143a35e64e2fd0afa9a61f3f7e85647`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809b2c7787a28aa760f2b39e58ad6793d1ea69189e8eccd7b93bfa31db405a7c`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e38abec161e7fb952f266511e7d01ec2ccab71f8debcf2c9221e3d4fbf878`  
		Last Modified: Thu, 05 May 2022 17:43:46 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.8`

```console
$ docker pull crate@sha256:8068ff815309e875170eab0e5dd4cd2ecb2ae2fab6125582bf9b9ac98d599885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.8` - linux; amd64

```console
$ docker pull crate@sha256:170490659b05a4a2644e65721e1fcd850e2a426c32a1b1552d018533f5da3fe2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308850548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146eae73ce56c9b37407ae33a759dd917f6d86c61001138e23c2f3ff2ba5ba8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 18:24:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.0.tar.gz.asc crate-4.8.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.0.tar.gz.asc     && tar -xf crate-4.8.0.tar.gz -C /crate --strip-components=1     && rm crate-4.8.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 18:24:31 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 18:24:31 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:24:31 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 18:24:32 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 18:24:32 GMT
VOLUME [/data]
# Thu, 05 May 2022 18:24:32 GMT
WORKDIR /data
# Thu, 05 May 2022 18:24:32 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 18:24:32 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 18:24:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 18:24:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T18:53:07.088304 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.0
# Thu, 05 May 2022 18:24:32 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 18:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 18:24:33 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d56db16ee6d4147de7608f3a01a833146235055fe731994c552e646c7aa1c`  
		Last Modified: Thu, 05 May 2022 18:25:57 GMT  
		Size: 231.2 MB (231167053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fd5a45b9210437c96637fc5bce51caf92b97fa53e9789b08fc93d21469a847`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 1.6 MB (1582198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52bda7f4a7f76ef5d91bd793a6fe4ce888b0bea718b46fb8dbe7f01436c8041`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d540af118b95d19bc1a7d2003ab69c1e1fe4483d3fa55e7700ee9cf7fcf73526`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984a8693c49029808a553d36ee2c14f1ff5ba6695845364f5450c1804e4f0239`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3abb1bdb0d848ef28445d2c4bb410139569a130c1b969cfa624e40019b2543a`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:2c33ade806503ee84598cb0e40208b742455d2dbd69dec937e6d1377fe131315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.0 MB (339015283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7c57155ffd6eca0e1a8d164cef4fa628fdecef8d0a1642585b2e0997631901`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 17:40:36 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.0.tar.gz.asc crate-4.8.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.0.tar.gz.asc     && tar -xf crate-4.8.0.tar.gz -C /crate --strip-components=1     && rm crate-4.8.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 17:40:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 17:40:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:40:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 17:40:49 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 17:40:49 GMT
VOLUME [/data]
# Thu, 05 May 2022 17:40:50 GMT
WORKDIR /data
# Thu, 05 May 2022 17:40:51 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 17:40:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 17:40:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 17:40:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T18:53:07.088304 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.0
# Thu, 05 May 2022 17:40:56 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 17:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 17:40:57 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b069689e8f4539df9d183ba93bb01d6bc5f059c16382a340df755984122f3e9c`  
		Last Modified: Thu, 05 May 2022 17:43:31 GMT  
		Size: 229.1 MB (229055702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5752ad92bb2440c6e88bf0e9f3deecb00dd9641bb50392030961d3ce745586a6`  
		Last Modified: Thu, 05 May 2022 17:43:05 GMT  
		Size: 1.6 MB (1580577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364ac86f52aaf4494a4ad4a507ba38c8e97db1c6798305da617693525240b23a`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a875120c41c012fe856205361975edaafbba3b78c35e6cdd9db4f671c46c0b77`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a21d0b521341450f925825ffb57d761652203aaf7fb02a08e65d9316e49046c`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b30f4f2313e2959fb4119ad163dc007df9abed4179ab4bb0b8d34534f01f369`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.8.0`

```console
$ docker pull crate@sha256:8068ff815309e875170eab0e5dd4cd2ecb2ae2fab6125582bf9b9ac98d599885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.8.0` - linux; amd64

```console
$ docker pull crate@sha256:170490659b05a4a2644e65721e1fcd850e2a426c32a1b1552d018533f5da3fe2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308850548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146eae73ce56c9b37407ae33a759dd917f6d86c61001138e23c2f3ff2ba5ba8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 18:24:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.0.tar.gz.asc crate-4.8.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.0.tar.gz.asc     && tar -xf crate-4.8.0.tar.gz -C /crate --strip-components=1     && rm crate-4.8.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 18:24:31 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 18:24:31 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:24:31 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 18:24:32 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 18:24:32 GMT
VOLUME [/data]
# Thu, 05 May 2022 18:24:32 GMT
WORKDIR /data
# Thu, 05 May 2022 18:24:32 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 18:24:32 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 18:24:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 18:24:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T18:53:07.088304 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.0
# Thu, 05 May 2022 18:24:32 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 18:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 18:24:33 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d56db16ee6d4147de7608f3a01a833146235055fe731994c552e646c7aa1c`  
		Last Modified: Thu, 05 May 2022 18:25:57 GMT  
		Size: 231.2 MB (231167053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fd5a45b9210437c96637fc5bce51caf92b97fa53e9789b08fc93d21469a847`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 1.6 MB (1582198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52bda7f4a7f76ef5d91bd793a6fe4ce888b0bea718b46fb8dbe7f01436c8041`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d540af118b95d19bc1a7d2003ab69c1e1fe4483d3fa55e7700ee9cf7fcf73526`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984a8693c49029808a553d36ee2c14f1ff5ba6695845364f5450c1804e4f0239`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3abb1bdb0d848ef28445d2c4bb410139569a130c1b969cfa624e40019b2543a`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.8.0` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:2c33ade806503ee84598cb0e40208b742455d2dbd69dec937e6d1377fe131315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.0 MB (339015283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7c57155ffd6eca0e1a8d164cef4fa628fdecef8d0a1642585b2e0997631901`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 17:40:36 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.0.tar.gz.asc crate-4.8.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.0.tar.gz.asc     && tar -xf crate-4.8.0.tar.gz -C /crate --strip-components=1     && rm crate-4.8.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 17:40:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 17:40:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:40:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 17:40:49 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 17:40:49 GMT
VOLUME [/data]
# Thu, 05 May 2022 17:40:50 GMT
WORKDIR /data
# Thu, 05 May 2022 17:40:51 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 17:40:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 17:40:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 17:40:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T18:53:07.088304 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.0
# Thu, 05 May 2022 17:40:56 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 17:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 17:40:57 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b069689e8f4539df9d183ba93bb01d6bc5f059c16382a340df755984122f3e9c`  
		Last Modified: Thu, 05 May 2022 17:43:31 GMT  
		Size: 229.1 MB (229055702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5752ad92bb2440c6e88bf0e9f3deecb00dd9641bb50392030961d3ce745586a6`  
		Last Modified: Thu, 05 May 2022 17:43:05 GMT  
		Size: 1.6 MB (1580577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364ac86f52aaf4494a4ad4a507ba38c8e97db1c6798305da617693525240b23a`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a875120c41c012fe856205361975edaafbba3b78c35e6cdd9db4f671c46c0b77`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a21d0b521341450f925825ffb57d761652203aaf7fb02a08e65d9316e49046c`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b30f4f2313e2959fb4119ad163dc007df9abed4179ab4bb0b8d34534f01f369`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:8068ff815309e875170eab0e5dd4cd2ecb2ae2fab6125582bf9b9ac98d599885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:170490659b05a4a2644e65721e1fcd850e2a426c32a1b1552d018533f5da3fe2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308850548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146eae73ce56c9b37407ae33a759dd917f6d86c61001138e23c2f3ff2ba5ba8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:37:51 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 18:24:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.0.tar.gz.asc crate-4.8.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.0.tar.gz.asc     && tar -xf crate-4.8.0.tar.gz -C /crate --strip-components=1     && rm crate-4.8.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 18:24:31 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 18:24:31 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:24:31 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 18:24:32 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 18:24:32 GMT
VOLUME [/data]
# Thu, 05 May 2022 18:24:32 GMT
WORKDIR /data
# Thu, 05 May 2022 18:24:32 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 18:24:32 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 18:24:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 18:24:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T18:53:07.088304 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.0
# Thu, 05 May 2022 18:24:32 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 18:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 18:24:33 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64b4c75f30c9b7afb780c16245b96bddad3d255e679114717859265250a0f64`  
		Last Modified: Wed, 15 Sep 2021 18:46:27 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d56db16ee6d4147de7608f3a01a833146235055fe731994c552e646c7aa1c`  
		Last Modified: Thu, 05 May 2022 18:25:57 GMT  
		Size: 231.2 MB (231167053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fd5a45b9210437c96637fc5bce51caf92b97fa53e9789b08fc93d21469a847`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 1.6 MB (1582198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52bda7f4a7f76ef5d91bd793a6fe4ce888b0bea718b46fb8dbe7f01436c8041`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d540af118b95d19bc1a7d2003ab69c1e1fe4483d3fa55e7700ee9cf7fcf73526`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984a8693c49029808a553d36ee2c14f1ff5ba6695845364f5450c1804e4f0239`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3abb1bdb0d848ef28445d2c4bb410139569a130c1b969cfa624e40019b2543a`  
		Last Modified: Thu, 05 May 2022 18:25:35 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:2c33ade806503ee84598cb0e40208b742455d2dbd69dec937e6d1377fe131315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.0 MB (339015283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7c57155ffd6eca0e1a8d164cef4fa628fdecef8d0a1642585b2e0997631901`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 20:17:55 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 05 May 2022 17:40:36 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.0.tar.gz.asc crate-4.8.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.0.tar.gz.asc     && tar -xf crate-4.8.0.tar.gz -C /crate --strip-components=1     && rm crate-4.8.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 05 May 2022 17:40:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 05 May 2022 17:40:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:40:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 05 May 2022 17:40:49 GMT
RUN mkdir -p /data/data /data/log
# Thu, 05 May 2022 17:40:49 GMT
VOLUME [/data]
# Thu, 05 May 2022 17:40:50 GMT
WORKDIR /data
# Thu, 05 May 2022 17:40:51 GMT
EXPOSE 4200 4300 5432
# Thu, 05 May 2022 17:40:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 05 May 2022 17:40:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 05 May 2022 17:40:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-04-28T18:53:07.088304 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.0
# Thu, 05 May 2022 17:40:56 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 05 May 2022 17:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 05 May 2022 17:40:57 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c55dc24d3cbebabdd223dbc4e51f5c147fad4f356562dd4a5c4fdb5a4ed4c`  
		Last Modified: Mon, 14 Feb 2022 20:24:02 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b069689e8f4539df9d183ba93bb01d6bc5f059c16382a340df755984122f3e9c`  
		Last Modified: Thu, 05 May 2022 17:43:31 GMT  
		Size: 229.1 MB (229055702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5752ad92bb2440c6e88bf0e9f3deecb00dd9641bb50392030961d3ce745586a6`  
		Last Modified: Thu, 05 May 2022 17:43:05 GMT  
		Size: 1.6 MB (1580577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364ac86f52aaf4494a4ad4a507ba38c8e97db1c6798305da617693525240b23a`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a875120c41c012fe856205361975edaafbba3b78c35e6cdd9db4f671c46c0b77`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a21d0b521341450f925825ffb57d761652203aaf7fb02a08e65d9316e49046c`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b30f4f2313e2959fb4119ad163dc007df9abed4179ab4bb0b8d34534f01f369`  
		Last Modified: Thu, 05 May 2022 17:43:04 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
