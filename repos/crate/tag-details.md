<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.6`](#crate46)
-	[`crate:4.6.7`](#crate467)
-	[`crate:4.7`](#crate47)
-	[`crate:4.7.0`](#crate470)
-	[`crate:latest`](#cratelatest)

## `crate:4.6`

```console
$ docker pull crate@sha256:02a874ce907887ae1fbbc19f92203c0101e542af100153dc81c2702cf02bb66a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.6` - linux; amd64

```console
$ docker pull crate@sha256:255c3b47643e81a805755aaa64cf9360ea4b692d511d430ca93ef0e15cd8efb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333282166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a4c40d8f42111730dbac154a8daaf9b092dd4060d41ab55095a8e662502558a`
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
# Mon, 24 Jan 2022 20:58:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.7.tar.gz.asc crate-4.6.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.7.tar.gz.asc     && tar -xf crate-4.6.7.tar.gz -C /crate --strip-components=1     && rm crate-4.6.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 24 Jan 2022 20:59:31 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 24 Jan 2022 20:59:31 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jan 2022 20:59:31 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 24 Jan 2022 20:59:32 GMT
RUN mkdir -p /data/data /data/log
# Mon, 24 Jan 2022 20:59:32 GMT
VOLUME [/data]
# Mon, 24 Jan 2022 20:59:32 GMT
WORKDIR /data
# Mon, 24 Jan 2022 20:59:32 GMT
EXPOSE 4200 4300 5432
# Mon, 24 Jan 2022 20:59:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 24 Jan 2022 20:59:33 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 24 Jan 2022 20:59:33 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-19T15:25:26.265468 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.7
# Mon, 24 Jan 2022 20:59:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 24 Jan 2022 20:59:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Jan 2022 20:59:34 GMT
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
	-	`sha256:77bdfcc915e3d6b46b979bd0efbaf130a1ca62b4b7459b5389cc2a446a09c2a4`  
		Last Modified: Mon, 24 Jan 2022 21:00:15 GMT  
		Size: 255.6 MB (255598668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cf083680069f1ae344d9ce89da674fd52aad77271d0e536dbfc438bbc2eb7f`  
		Last Modified: Mon, 24 Jan 2022 20:59:47 GMT  
		Size: 1.6 MB (1582201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4da95b014bb5dde7754ea770a5a84f70e1ee3a57e7568af1b2f1cb2bf23d736`  
		Last Modified: Mon, 24 Jan 2022 20:59:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b729a7b2b19736b06daf6734a270e598df42325396100d6e97603438aacbf`  
		Last Modified: Mon, 24 Jan 2022 20:59:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cd90676ad3d4a672a8aa75cd930205f9484b05a16e6204230dc65b0fd3377a`  
		Last Modified: Mon, 24 Jan 2022 20:59:48 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aac0d94022e8be81274f75ba3ac9d477df89ecb1d8ff77fd6250629ce25935`  
		Last Modified: Mon, 24 Jan 2022 20:59:47 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.6` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f83e6eec3a9f89cccebf7e50dda42080c88bb027964130178288e0ce4ebbea0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7735b30dbb2ef4230be0a951faf26ab97eeec520eab2456d69e8e435359ad6e0`
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
# Mon, 14 Feb 2022 20:22:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.7.tar.gz.asc crate-4.6.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.7.tar.gz.asc     && tar -xf crate-4.6.7.tar.gz -C /crate --strip-components=1     && rm crate-4.6.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 14 Feb 2022 20:23:24 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Feb 2022 20:23:24 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Feb 2022 20:23:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Feb 2022 20:23:27 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Feb 2022 20:23:27 GMT
VOLUME [/data]
# Mon, 14 Feb 2022 20:23:28 GMT
WORKDIR /data
# Mon, 14 Feb 2022 20:23:29 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Feb 2022 20:23:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Feb 2022 20:23:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Feb 2022 20:23:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-19T15:25:26.265468 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.7
# Mon, 14 Feb 2022 20:23:34 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Feb 2022 20:23:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Feb 2022 20:23:35 GMT
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
	-	`sha256:6391baa5cbf6c036e8b30fb61aab1b4f9a0df072350e0848ee3be29b2d76a1ae`  
		Last Modified: Mon, 14 Feb 2022 20:25:10 GMT  
		Size: 252.4 MB (252384831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c6803e0cae7b5da845c50dcb7a3869f226922447b82d2bcb6c929e7975a62e`  
		Last Modified: Mon, 14 Feb 2022 20:24:44 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303a21d62a369deb7030b7135c5447d0b98dd5a37e206d5d142adcb3c554717`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e4314134cfbb3307cc22ba4cc350243ca604b2fc4003917a44afd73901e6df`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ec9592e405b5ea118358e50938fdbb1bc84ab06d6f35ddaddc51c6626e89b2`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392765819ba9ebaeebce3a1a9c284ddceefab454a274f0d0a4039884787b8a80`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.6.7`

```console
$ docker pull crate@sha256:02a874ce907887ae1fbbc19f92203c0101e542af100153dc81c2702cf02bb66a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.6.7` - linux; amd64

```console
$ docker pull crate@sha256:255c3b47643e81a805755aaa64cf9360ea4b692d511d430ca93ef0e15cd8efb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333282166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a4c40d8f42111730dbac154a8daaf9b092dd4060d41ab55095a8e662502558a`
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
# Mon, 24 Jan 2022 20:58:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.7.tar.gz.asc crate-4.6.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.7.tar.gz.asc     && tar -xf crate-4.6.7.tar.gz -C /crate --strip-components=1     && rm crate-4.6.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 24 Jan 2022 20:59:31 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 24 Jan 2022 20:59:31 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Jan 2022 20:59:31 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 24 Jan 2022 20:59:32 GMT
RUN mkdir -p /data/data /data/log
# Mon, 24 Jan 2022 20:59:32 GMT
VOLUME [/data]
# Mon, 24 Jan 2022 20:59:32 GMT
WORKDIR /data
# Mon, 24 Jan 2022 20:59:32 GMT
EXPOSE 4200 4300 5432
# Mon, 24 Jan 2022 20:59:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 24 Jan 2022 20:59:33 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 24 Jan 2022 20:59:33 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-19T15:25:26.265468 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.7
# Mon, 24 Jan 2022 20:59:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 24 Jan 2022 20:59:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Jan 2022 20:59:34 GMT
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
	-	`sha256:77bdfcc915e3d6b46b979bd0efbaf130a1ca62b4b7459b5389cc2a446a09c2a4`  
		Last Modified: Mon, 24 Jan 2022 21:00:15 GMT  
		Size: 255.6 MB (255598668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cf083680069f1ae344d9ce89da674fd52aad77271d0e536dbfc438bbc2eb7f`  
		Last Modified: Mon, 24 Jan 2022 20:59:47 GMT  
		Size: 1.6 MB (1582201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4da95b014bb5dde7754ea770a5a84f70e1ee3a57e7568af1b2f1cb2bf23d736`  
		Last Modified: Mon, 24 Jan 2022 20:59:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b729a7b2b19736b06daf6734a270e598df42325396100d6e97603438aacbf`  
		Last Modified: Mon, 24 Jan 2022 20:59:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cd90676ad3d4a672a8aa75cd930205f9484b05a16e6204230dc65b0fd3377a`  
		Last Modified: Mon, 24 Jan 2022 20:59:48 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aac0d94022e8be81274f75ba3ac9d477df89ecb1d8ff77fd6250629ce25935`  
		Last Modified: Mon, 24 Jan 2022 20:59:47 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.6.7` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f83e6eec3a9f89cccebf7e50dda42080c88bb027964130178288e0ce4ebbea0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7735b30dbb2ef4230be0a951faf26ab97eeec520eab2456d69e8e435359ad6e0`
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
# Mon, 14 Feb 2022 20:22:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.7.tar.gz.asc crate-4.6.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.7.tar.gz.asc     && tar -xf crate-4.6.7.tar.gz -C /crate --strip-components=1     && rm crate-4.6.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 14 Feb 2022 20:23:24 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Feb 2022 20:23:24 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Feb 2022 20:23:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Feb 2022 20:23:27 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Feb 2022 20:23:27 GMT
VOLUME [/data]
# Mon, 14 Feb 2022 20:23:28 GMT
WORKDIR /data
# Mon, 14 Feb 2022 20:23:29 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Feb 2022 20:23:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Feb 2022 20:23:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Feb 2022 20:23:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-19T15:25:26.265468 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.7
# Mon, 14 Feb 2022 20:23:34 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Feb 2022 20:23:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Feb 2022 20:23:35 GMT
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
	-	`sha256:6391baa5cbf6c036e8b30fb61aab1b4f9a0df072350e0848ee3be29b2d76a1ae`  
		Last Modified: Mon, 14 Feb 2022 20:25:10 GMT  
		Size: 252.4 MB (252384831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c6803e0cae7b5da845c50dcb7a3869f226922447b82d2bcb6c929e7975a62e`  
		Last Modified: Mon, 14 Feb 2022 20:24:44 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d303a21d62a369deb7030b7135c5447d0b98dd5a37e206d5d142adcb3c554717`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e4314134cfbb3307cc22ba4cc350243ca604b2fc4003917a44afd73901e6df`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ec9592e405b5ea118358e50938fdbb1bc84ab06d6f35ddaddc51c6626e89b2`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392765819ba9ebaeebce3a1a9c284ddceefab454a274f0d0a4039884787b8a80`  
		Last Modified: Mon, 14 Feb 2022 20:24:42 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.7`

```console
$ docker pull crate@sha256:c7984a05e15b16452458716021a4c8918ddf58a1e9b335517a23baa7f22693bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.7` - linux; amd64

```console
$ docker pull crate@sha256:bf74f9a4f17c35cf91fcf96a645d19e59344d8dc1f4fddf66baab3a811b0e5de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.7 MB (324666013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc1b69cbe7da4af4e9c515e47e59697da3045fd55e287c5f779247566c0e092`
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
# Tue, 01 Feb 2022 22:32:49 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.0.tar.gz.asc crate-4.7.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.0.tar.gz.asc     && tar -xf crate-4.7.0.tar.gz -C /crate --strip-components=1     && rm crate-4.7.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 01 Feb 2022 22:33:30 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 01 Feb 2022 22:33:30 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 22:33:30 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 01 Feb 2022 22:33:31 GMT
RUN mkdir -p /data/data /data/log
# Tue, 01 Feb 2022 22:33:31 GMT
VOLUME [/data]
# Tue, 01 Feb 2022 22:33:31 GMT
WORKDIR /data
# Tue, 01 Feb 2022 22:33:31 GMT
EXPOSE 4200 4300 5432
# Tue, 01 Feb 2022 22:33:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 01 Feb 2022 22:33:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 01 Feb 2022 22:33:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-26T09:48:10.009142 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.0
# Tue, 01 Feb 2022 22:33:32 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 01 Feb 2022 22:33:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Feb 2022 22:33:33 GMT
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
	-	`sha256:049a2b0ddeaa71e0b757326b3a4ed25408e13445463712fa859c81dd445844c8`  
		Last Modified: Tue, 01 Feb 2022 22:34:10 GMT  
		Size: 247.0 MB (246982517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a6364dd15a26c1d031ca4e60809ae602eb70bfe41d7a4ed986455deafb6e53`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 1.6 MB (1582196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c485a94c69c70f23da68d11449a17459b49c6c0fc22c90cc79738bd21911a8f1`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3348aaf6a0129e5744da1cf8861a6844f5626de7a8c6815e29a8799d1407922`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912a3928803663f10203735b32e381ffca7cc769f4eb63591bba26c70e222e31`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bf50c4d91a93a0ce2083147498112a15341fd181982ce7a035fa7ea9fb8c53`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.7` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:99667432bb8b9270599e50b21f6f76487ae303ff9f337c161786e633a018978f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352978911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b769f7f79a3cd4a80c73f7234303eb95801bf1c38979b77f8dc65e2b348349f`
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
# Mon, 14 Feb 2022 20:19:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.0.tar.gz.asc crate-4.7.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.0.tar.gz.asc     && tar -xf crate-4.7.0.tar.gz -C /crate --strip-components=1     && rm crate-4.7.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 14 Feb 2022 20:20:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Feb 2022 20:20:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Feb 2022 20:20:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Feb 2022 20:20:49 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Feb 2022 20:20:49 GMT
VOLUME [/data]
# Mon, 14 Feb 2022 20:20:50 GMT
WORKDIR /data
# Mon, 14 Feb 2022 20:20:51 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Feb 2022 20:20:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Feb 2022 20:20:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Feb 2022 20:20:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-26T09:48:10.009142 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.0
# Mon, 14 Feb 2022 20:20:56 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Feb 2022 20:20:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Feb 2022 20:20:57 GMT
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
	-	`sha256:9867e4e87a4a436261223764eba2f55f57f61515b41b29b0fe6b465021def368`  
		Last Modified: Mon, 14 Feb 2022 20:24:28 GMT  
		Size: 243.0 MB (243019329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cdf900812a41a0eac111bf2b772f7ae4169b72e420c93a543bb29f2f5d61fe`  
		Last Modified: Mon, 14 Feb 2022 20:24:01 GMT  
		Size: 1.6 MB (1580576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f913b8c084125e3225066e085751ce1730259578cbb6d4bae04ae8062b6ae88`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec8e7cc6fdb89c4dba12bb982f8c6d7af8a819e09969aa807bcae395afe90d`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdcc5e2dfdf24301bccdd521e701bccad12e76493a63415ebba0c6c49bf6992`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157ba91bbf57dfcec33e05bcb5c4292c0998f656f289e84bc13a2511792bd62a`  
		Last Modified: Mon, 14 Feb 2022 20:24:01 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.7.0`

```console
$ docker pull crate@sha256:c7984a05e15b16452458716021a4c8918ddf58a1e9b335517a23baa7f22693bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.7.0` - linux; amd64

```console
$ docker pull crate@sha256:bf74f9a4f17c35cf91fcf96a645d19e59344d8dc1f4fddf66baab3a811b0e5de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.7 MB (324666013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc1b69cbe7da4af4e9c515e47e59697da3045fd55e287c5f779247566c0e092`
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
# Tue, 01 Feb 2022 22:32:49 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.0.tar.gz.asc crate-4.7.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.0.tar.gz.asc     && tar -xf crate-4.7.0.tar.gz -C /crate --strip-components=1     && rm crate-4.7.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 01 Feb 2022 22:33:30 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 01 Feb 2022 22:33:30 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 22:33:30 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 01 Feb 2022 22:33:31 GMT
RUN mkdir -p /data/data /data/log
# Tue, 01 Feb 2022 22:33:31 GMT
VOLUME [/data]
# Tue, 01 Feb 2022 22:33:31 GMT
WORKDIR /data
# Tue, 01 Feb 2022 22:33:31 GMT
EXPOSE 4200 4300 5432
# Tue, 01 Feb 2022 22:33:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 01 Feb 2022 22:33:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 01 Feb 2022 22:33:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-26T09:48:10.009142 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.0
# Tue, 01 Feb 2022 22:33:32 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 01 Feb 2022 22:33:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Feb 2022 22:33:33 GMT
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
	-	`sha256:049a2b0ddeaa71e0b757326b3a4ed25408e13445463712fa859c81dd445844c8`  
		Last Modified: Tue, 01 Feb 2022 22:34:10 GMT  
		Size: 247.0 MB (246982517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a6364dd15a26c1d031ca4e60809ae602eb70bfe41d7a4ed986455deafb6e53`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 1.6 MB (1582196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c485a94c69c70f23da68d11449a17459b49c6c0fc22c90cc79738bd21911a8f1`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3348aaf6a0129e5744da1cf8861a6844f5626de7a8c6815e29a8799d1407922`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912a3928803663f10203735b32e381ffca7cc769f4eb63591bba26c70e222e31`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bf50c4d91a93a0ce2083147498112a15341fd181982ce7a035fa7ea9fb8c53`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.7.0` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:99667432bb8b9270599e50b21f6f76487ae303ff9f337c161786e633a018978f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352978911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b769f7f79a3cd4a80c73f7234303eb95801bf1c38979b77f8dc65e2b348349f`
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
# Mon, 14 Feb 2022 20:19:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.0.tar.gz.asc crate-4.7.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.0.tar.gz.asc     && tar -xf crate-4.7.0.tar.gz -C /crate --strip-components=1     && rm crate-4.7.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 14 Feb 2022 20:20:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Feb 2022 20:20:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Feb 2022 20:20:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Feb 2022 20:20:49 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Feb 2022 20:20:49 GMT
VOLUME [/data]
# Mon, 14 Feb 2022 20:20:50 GMT
WORKDIR /data
# Mon, 14 Feb 2022 20:20:51 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Feb 2022 20:20:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Feb 2022 20:20:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Feb 2022 20:20:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-26T09:48:10.009142 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.0
# Mon, 14 Feb 2022 20:20:56 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Feb 2022 20:20:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Feb 2022 20:20:57 GMT
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
	-	`sha256:9867e4e87a4a436261223764eba2f55f57f61515b41b29b0fe6b465021def368`  
		Last Modified: Mon, 14 Feb 2022 20:24:28 GMT  
		Size: 243.0 MB (243019329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cdf900812a41a0eac111bf2b772f7ae4169b72e420c93a543bb29f2f5d61fe`  
		Last Modified: Mon, 14 Feb 2022 20:24:01 GMT  
		Size: 1.6 MB (1580576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f913b8c084125e3225066e085751ce1730259578cbb6d4bae04ae8062b6ae88`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec8e7cc6fdb89c4dba12bb982f8c6d7af8a819e09969aa807bcae395afe90d`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdcc5e2dfdf24301bccdd521e701bccad12e76493a63415ebba0c6c49bf6992`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157ba91bbf57dfcec33e05bcb5c4292c0998f656f289e84bc13a2511792bd62a`  
		Last Modified: Mon, 14 Feb 2022 20:24:01 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:c7984a05e15b16452458716021a4c8918ddf58a1e9b335517a23baa7f22693bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:bf74f9a4f17c35cf91fcf96a645d19e59344d8dc1f4fddf66baab3a811b0e5de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.7 MB (324666013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc1b69cbe7da4af4e9c515e47e59697da3045fd55e287c5f779247566c0e092`
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
# Tue, 01 Feb 2022 22:32:49 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.0.tar.gz.asc crate-4.7.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.0.tar.gz.asc     && tar -xf crate-4.7.0.tar.gz -C /crate --strip-components=1     && rm crate-4.7.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 01 Feb 2022 22:33:30 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 01 Feb 2022 22:33:30 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 22:33:30 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 01 Feb 2022 22:33:31 GMT
RUN mkdir -p /data/data /data/log
# Tue, 01 Feb 2022 22:33:31 GMT
VOLUME [/data]
# Tue, 01 Feb 2022 22:33:31 GMT
WORKDIR /data
# Tue, 01 Feb 2022 22:33:31 GMT
EXPOSE 4200 4300 5432
# Tue, 01 Feb 2022 22:33:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 01 Feb 2022 22:33:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 01 Feb 2022 22:33:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-26T09:48:10.009142 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.0
# Tue, 01 Feb 2022 22:33:32 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 01 Feb 2022 22:33:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Feb 2022 22:33:33 GMT
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
	-	`sha256:049a2b0ddeaa71e0b757326b3a4ed25408e13445463712fa859c81dd445844c8`  
		Last Modified: Tue, 01 Feb 2022 22:34:10 GMT  
		Size: 247.0 MB (246982517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a6364dd15a26c1d031ca4e60809ae602eb70bfe41d7a4ed986455deafb6e53`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 1.6 MB (1582196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c485a94c69c70f23da68d11449a17459b49c6c0fc22c90cc79738bd21911a8f1`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3348aaf6a0129e5744da1cf8861a6844f5626de7a8c6815e29a8799d1407922`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912a3928803663f10203735b32e381ffca7cc769f4eb63591bba26c70e222e31`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bf50c4d91a93a0ce2083147498112a15341fd181982ce7a035fa7ea9fb8c53`  
		Last Modified: Tue, 01 Feb 2022 22:33:48 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:99667432bb8b9270599e50b21f6f76487ae303ff9f337c161786e633a018978f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352978911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b769f7f79a3cd4a80c73f7234303eb95801bf1c38979b77f8dc65e2b348349f`
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
# Mon, 14 Feb 2022 20:19:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.7.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.7.0.tar.gz.asc crate-4.7.0.tar.gz     && rm -rf "$GNUPGHOME" crate-4.7.0.tar.gz.asc     && tar -xf crate-4.7.0.tar.gz -C /crate --strip-components=1     && rm crate-4.7.0.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 14 Feb 2022 20:20:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Feb 2022 20:20:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Feb 2022 20:20:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Feb 2022 20:20:49 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Feb 2022 20:20:49 GMT
VOLUME [/data]
# Mon, 14 Feb 2022 20:20:50 GMT
WORKDIR /data
# Mon, 14 Feb 2022 20:20:51 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Feb 2022 20:20:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Feb 2022 20:20:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Feb 2022 20:20:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-01-26T09:48:10.009142 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.7.0
# Mon, 14 Feb 2022 20:20:56 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Feb 2022 20:20:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Feb 2022 20:20:57 GMT
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
	-	`sha256:9867e4e87a4a436261223764eba2f55f57f61515b41b29b0fe6b465021def368`  
		Last Modified: Mon, 14 Feb 2022 20:24:28 GMT  
		Size: 243.0 MB (243019329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cdf900812a41a0eac111bf2b772f7ae4169b72e420c93a543bb29f2f5d61fe`  
		Last Modified: Mon, 14 Feb 2022 20:24:01 GMT  
		Size: 1.6 MB (1580576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f913b8c084125e3225066e085751ce1730259578cbb6d4bae04ae8062b6ae88`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ec8e7cc6fdb89c4dba12bb982f8c6d7af8a819e09969aa807bcae395afe90d`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdcc5e2dfdf24301bccdd521e701bccad12e76493a63415ebba0c6c49bf6992`  
		Last Modified: Mon, 14 Feb 2022 20:24:00 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157ba91bbf57dfcec33e05bcb5c4292c0998f656f289e84bc13a2511792bd62a`  
		Last Modified: Mon, 14 Feb 2022 20:24:01 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
