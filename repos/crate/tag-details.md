<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.8`](#crate48)
-	[`crate:4.8.4`](#crate484)
-	[`crate:5.2`](#crate52)
-	[`crate:5.2.10`](#crate5210)
-	[`crate:5.3`](#crate53)
-	[`crate:5.3.7`](#crate537)
-	[`crate:5.4`](#crate54)
-	[`crate:5.4.5`](#crate545)
-	[`crate:5.5`](#crate55)
-	[`crate:5.5.0`](#crate550)
-	[`crate:latest`](#cratelatest)

## `crate:4.8`

```console
$ docker pull crate@sha256:fcfb1e26e4b6b84cf23bbb0de51a9671655d1e843b01cffea5984643727e021e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.8` - linux; amd64

```console
$ docker pull crate@sha256:ab33e064e23959eed997f0e9317a8ccb942974f7d3159ac464a5a3cb221e25c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.6 MB (366609762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849c866b7319b231f9f5482aef88650ec60dd6d7059a29de576cbd4b789bd3d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Mon, 12 Sep 2022 19:20:47 GMT
RUN yum install -y yum-utils deltarpm     && yum makecache     && yum upgrade -y     && yum install -y python3 openssl     && pip3 install --upgrade pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 20 Sep 2022 20:24:28 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.4.tar.gz.asc crate-4.8.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.4.tar.gz.asc     && tar -xf crate-4.8.4.tar.gz -C /crate --strip-components=1     && rm crate-4.8.4.tar.gz
# Tue, 20 Sep 2022 20:24:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 20 Sep 2022 20:24:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Sep 2022 20:24:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 20 Sep 2022 20:24:33 GMT
RUN mkdir -p /data/data /data/log
# Tue, 20 Sep 2022 20:24:33 GMT
VOLUME [/data]
# Tue, 20 Sep 2022 20:24:33 GMT
WORKDIR /data
# Tue, 20 Sep 2022 20:24:33 GMT
EXPOSE 4200 4300 5432
# Tue, 20 Sep 2022 20:24:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 20 Sep 2022 20:24:33 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 20 Sep 2022 20:24:33 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-09-15T10:52:50.199012 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.4
# Tue, 20 Sep 2022 20:24:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 20 Sep 2022 20:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 20 Sep 2022 20:24:34 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816162095613648af0045121a146a6ab058718d006d17f2ea25e169f0961b298`  
		Last Modified: Mon, 12 Sep 2022 19:22:25 GMT  
		Size: 77.1 MB (77149352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3bdb3f3876f51c5600bc5d5576e6c84959f5433fb375eb3a1b2798d93abc31`  
		Last Modified: Tue, 20 Sep 2022 20:25:15 GMT  
		Size: 211.7 MB (211650590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d385fe2b73321323b7b11085d41441495146f7a18dbf421502225a9ff8656`  
		Last Modified: Tue, 20 Sep 2022 20:24:54 GMT  
		Size: 1.7 MB (1710779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c312f86d93dded0d735bc9b7234f64c5a8ff5bc82ffe1ce9ad869ed3a7b68c68`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eeaec4222433c7af8e5220f511915ab8fb4049a7136fc371b5d2679811e34c4`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed829b350fc610813c498009ca8aecf3b3e6184dfe54943a7d490e583e207f4`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2994a6708f131a2fa358dbb8885094c2d552f7880f924a3b84048082560032f3`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:54bb068652a7f229af18cc10ae7e5d94d19cbbf4952635694dc2e34df3502b56
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **666.5 MB (666503011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac29f1818d2fdc8991ad2484f8adac7e43311743dae8b71f35d1eda47c45be02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 24 Oct 2022 21:41:05 GMT
RUN yum install -y yum-utils deltarpm     && yum makecache     && yum upgrade -y     && yum install -y python3 openssl     && pip3 install --upgrade pip     && yum clean all     && rm -rf /var/cache/yum
# Mon, 24 Oct 2022 21:42:19 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.4.tar.gz.asc crate-4.8.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.4.tar.gz.asc     && tar -xf crate-4.8.4.tar.gz -C /crate --strip-components=1     && rm crate-4.8.4.tar.gz
# Mon, 24 Oct 2022 21:42:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 24 Oct 2022 21:42:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2022 21:42:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 24 Oct 2022 21:42:24 GMT
RUN mkdir -p /data/data /data/log
# Mon, 24 Oct 2022 21:42:24 GMT
VOLUME [/data]
# Mon, 24 Oct 2022 21:42:24 GMT
WORKDIR /data
# Mon, 24 Oct 2022 21:42:24 GMT
EXPOSE 4200 4300 5432
# Mon, 24 Oct 2022 21:42:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 24 Oct 2022 21:42:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 24 Oct 2022 21:42:24 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-09-15T10:52:50.199012 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.4
# Mon, 24 Oct 2022 21:42:24 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 24 Oct 2022 21:42:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Oct 2022 21:42:24 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bd2dd4fe2ac3696c00e2e33054e11971bf81acb6591869e1d525feb18cceb3`  
		Last Modified: Mon, 24 Oct 2022 21:45:28 GMT  
		Size: 346.0 MB (345996846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5e7c58b367faadd294e7b188398fc564edf19271fac04a26b51637c28e43e6`  
		Last Modified: Mon, 24 Oct 2022 21:45:57 GMT  
		Size: 210.4 MB (210418568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b966a9d970d836ffb3ccc8dcca4ffd79e2f6334cb230e0617b25457394750b`  
		Last Modified: Mon, 24 Oct 2022 21:45:42 GMT  
		Size: 1.7 MB (1710769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286650217f63a621366b0d7e1115fa37df60654f36c5b556c3b2a5cf41e7f6cd`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d1e66c86b54db4e4dc22fce8f33097dcad2745154e050210dacb713db2c232`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a335f20bda4ea63d2b38a9c41ea60713b51e8b3816061c4067b7f69604ecf5f`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293324d5cf1d0be9fc09670f9ab9249b7775dfb2a0c350042d4909228b55011f`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.8.4`

```console
$ docker pull crate@sha256:fcfb1e26e4b6b84cf23bbb0de51a9671655d1e843b01cffea5984643727e021e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.8.4` - linux; amd64

```console
$ docker pull crate@sha256:ab33e064e23959eed997f0e9317a8ccb942974f7d3159ac464a5a3cb221e25c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.6 MB (366609762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849c866b7319b231f9f5482aef88650ec60dd6d7059a29de576cbd4b789bd3d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Mon, 12 Sep 2022 19:20:47 GMT
RUN yum install -y yum-utils deltarpm     && yum makecache     && yum upgrade -y     && yum install -y python3 openssl     && pip3 install --upgrade pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 20 Sep 2022 20:24:28 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.4.tar.gz.asc crate-4.8.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.4.tar.gz.asc     && tar -xf crate-4.8.4.tar.gz -C /crate --strip-components=1     && rm crate-4.8.4.tar.gz
# Tue, 20 Sep 2022 20:24:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 20 Sep 2022 20:24:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Sep 2022 20:24:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 20 Sep 2022 20:24:33 GMT
RUN mkdir -p /data/data /data/log
# Tue, 20 Sep 2022 20:24:33 GMT
VOLUME [/data]
# Tue, 20 Sep 2022 20:24:33 GMT
WORKDIR /data
# Tue, 20 Sep 2022 20:24:33 GMT
EXPOSE 4200 4300 5432
# Tue, 20 Sep 2022 20:24:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 20 Sep 2022 20:24:33 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 20 Sep 2022 20:24:33 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-09-15T10:52:50.199012 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.4
# Tue, 20 Sep 2022 20:24:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 20 Sep 2022 20:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 20 Sep 2022 20:24:34 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816162095613648af0045121a146a6ab058718d006d17f2ea25e169f0961b298`  
		Last Modified: Mon, 12 Sep 2022 19:22:25 GMT  
		Size: 77.1 MB (77149352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3bdb3f3876f51c5600bc5d5576e6c84959f5433fb375eb3a1b2798d93abc31`  
		Last Modified: Tue, 20 Sep 2022 20:25:15 GMT  
		Size: 211.7 MB (211650590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d385fe2b73321323b7b11085d41441495146f7a18dbf421502225a9ff8656`  
		Last Modified: Tue, 20 Sep 2022 20:24:54 GMT  
		Size: 1.7 MB (1710779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c312f86d93dded0d735bc9b7234f64c5a8ff5bc82ffe1ce9ad869ed3a7b68c68`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eeaec4222433c7af8e5220f511915ab8fb4049a7136fc371b5d2679811e34c4`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed829b350fc610813c498009ca8aecf3b3e6184dfe54943a7d490e583e207f4`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2994a6708f131a2fa358dbb8885094c2d552f7880f924a3b84048082560032f3`  
		Last Modified: Tue, 20 Sep 2022 20:24:53 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.8.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:54bb068652a7f229af18cc10ae7e5d94d19cbbf4952635694dc2e34df3502b56
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **666.5 MB (666503011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac29f1818d2fdc8991ad2484f8adac7e43311743dae8b71f35d1eda47c45be02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 24 Oct 2022 21:41:05 GMT
RUN yum install -y yum-utils deltarpm     && yum makecache     && yum upgrade -y     && yum install -y python3 openssl     && pip3 install --upgrade pip     && yum clean all     && rm -rf /var/cache/yum
# Mon, 24 Oct 2022 21:42:19 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.8.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.8.4.tar.gz.asc crate-4.8.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.8.4.tar.gz.asc     && tar -xf crate-4.8.4.tar.gz -C /crate --strip-components=1     && rm crate-4.8.4.tar.gz
# Mon, 24 Oct 2022 21:42:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 24 Oct 2022 21:42:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2022 21:42:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 24 Oct 2022 21:42:24 GMT
RUN mkdir -p /data/data /data/log
# Mon, 24 Oct 2022 21:42:24 GMT
VOLUME [/data]
# Mon, 24 Oct 2022 21:42:24 GMT
WORKDIR /data
# Mon, 24 Oct 2022 21:42:24 GMT
EXPOSE 4200 4300 5432
# Mon, 24 Oct 2022 21:42:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 24 Oct 2022 21:42:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 24 Oct 2022 21:42:24 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-09-15T10:52:50.199012 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.8.4
# Mon, 24 Oct 2022 21:42:24 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 24 Oct 2022 21:42:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 24 Oct 2022 21:42:24 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bd2dd4fe2ac3696c00e2e33054e11971bf81acb6591869e1d525feb18cceb3`  
		Last Modified: Mon, 24 Oct 2022 21:45:28 GMT  
		Size: 346.0 MB (345996846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5e7c58b367faadd294e7b188398fc564edf19271fac04a26b51637c28e43e6`  
		Last Modified: Mon, 24 Oct 2022 21:45:57 GMT  
		Size: 210.4 MB (210418568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b966a9d970d836ffb3ccc8dcca4ffd79e2f6334cb230e0617b25457394750b`  
		Last Modified: Mon, 24 Oct 2022 21:45:42 GMT  
		Size: 1.7 MB (1710769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286650217f63a621366b0d7e1115fa37df60654f36c5b556c3b2a5cf41e7f6cd`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d1e66c86b54db4e4dc22fce8f33097dcad2745154e050210dacb713db2c232`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a335f20bda4ea63d2b38a9c41ea60713b51e8b3816061c4067b7f69604ecf5f`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293324d5cf1d0be9fc09670f9ab9249b7775dfb2a0c350042d4909228b55011f`  
		Last Modified: Mon, 24 Oct 2022 21:45:41 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2`

```console
$ docker pull crate@sha256:eabdd2056b02d5ee747b9ff2a2e3c73e609ebe2fbc47f2103bbdf4f0789ffae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2` - linux; amd64

```console
$ docker pull crate@sha256:d262583aaf9bb02aaa0379f2d6f0c72dae3344e0ef3dd55f64d7d130135de13e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.9 MB (304934403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70002ccba5726c7c0cc90d0710170514f16b2c8850e086acd9786e006464a0ab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:19:42 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 01:20:59 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.10.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.10.tar.gz.asc crate-5.2.10.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.10.tar.gz.asc     && tar -xf crate-5.2.10.tar.gz -C /crate --strip-components=1     && rm crate-5.2.10.tar.gz
# Tue, 17 Oct 2023 01:21:02 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 01:21:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 01:21:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 01:21:02 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 01:21:02 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 01:21:02 GMT
WORKDIR /data
# Tue, 17 Oct 2023 01:21:03 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 01:21:03 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 01:21:03 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 01:21:03 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T15:07:59.910862 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.10
# Tue, 17 Oct 2023 01:21:03 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 01:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 01:21:03 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e2445eddd520acc99c0726888b224865c2a40b1f13168bed9a799f272e7e12`  
		Last Modified: Tue, 26 Sep 2023 18:20:18 GMT  
		Size: 7.7 MB (7669639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a2151075c010ad6d54d0de1286f72a2909c2adb250b25f9fb400a0e04eac0`  
		Last Modified: Tue, 17 Oct 2023 01:22:43 GMT  
		Size: 227.1 MB (227118914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151d7b12e398dedd5a77f271fa6820938915d579580f3456fe00dd6f06406801`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e2a4a736bcb63eb1e4c0c3b18aefea77f95c9891709425036d44cc9bbd3d90`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e725a68ad78e232bc0902292bcafdddd35d216922a6117aea77d00a0618e0e2`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ba1db1f2f0f34c2e83ca0bc2bf86d9c0d434cf3ad507282f1745e8b94875ef`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e23c456e9a2e3ab59b11b0393c040ba4e141020ca10ec2424a0f7c6804b5ebb`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:84b974e87b1b9b148e0f9b53c610131d97e34107db35d50ff158dca6c08f04f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302429188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2b51d99b4f26d601cdc5f14e2512aeb882c73d27013275b3fc1f20270506e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:39:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 00:41:59 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.10.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.10.tar.gz.asc crate-5.2.10.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.10.tar.gz.asc     && tar -xf crate-5.2.10.tar.gz -C /crate --strip-components=1     && rm crate-5.2.10.tar.gz
# Tue, 17 Oct 2023 00:42:03 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 00:42:03 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 00:42:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 00:42:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 00:42:04 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 00:42:04 GMT
WORKDIR /data
# Tue, 17 Oct 2023 00:42:04 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 00:42:04 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 00:42:04 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 00:42:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T15:07:59.910862 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.10
# Tue, 17 Oct 2023 00:42:04 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 00:42:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 00:42:04 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed142c0b1a887b57068b49d7c01694330116d5e4223aa1ec3f5d266d37add262`  
		Last Modified: Tue, 26 Sep 2023 18:40:17 GMT  
		Size: 7.5 MB (7510200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a97b356aa78dea3947ee72ea6a4d8d69f6a1864337ecec709be87c1141ff07`  
		Last Modified: Tue, 17 Oct 2023 00:43:33 GMT  
		Size: 225.9 MB (225861924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631719eff1c8e13820f8a3a86a5f67f796731971b9c346544b39cf12924985db`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 1.9 MB (1931737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee3cad283afe4bf0c54fde1d0f244ca5d33a7c1e64d11131d2f18efa7fa264`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6ff39bfa60dc5097d745cc385e007dc038db158d5a35d2338bcc2b08edf47e`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7315a2755765ae42620461d3f11de8bedbd40888391d2cfd5ed179fccd05482f`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e40db3b84ff3a56d1e5d7eed970aeec3bc9df1abef5e2809349146cff582934`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2.10`

```console
$ docker pull crate@sha256:eabdd2056b02d5ee747b9ff2a2e3c73e609ebe2fbc47f2103bbdf4f0789ffae1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2.10` - linux; amd64

```console
$ docker pull crate@sha256:d262583aaf9bb02aaa0379f2d6f0c72dae3344e0ef3dd55f64d7d130135de13e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.9 MB (304934403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70002ccba5726c7c0cc90d0710170514f16b2c8850e086acd9786e006464a0ab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:19:42 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 01:20:59 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.10.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.10.tar.gz.asc crate-5.2.10.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.10.tar.gz.asc     && tar -xf crate-5.2.10.tar.gz -C /crate --strip-components=1     && rm crate-5.2.10.tar.gz
# Tue, 17 Oct 2023 01:21:02 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 01:21:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 01:21:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 01:21:02 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 01:21:02 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 01:21:02 GMT
WORKDIR /data
# Tue, 17 Oct 2023 01:21:03 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 01:21:03 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 01:21:03 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 01:21:03 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T15:07:59.910862 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.10
# Tue, 17 Oct 2023 01:21:03 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 01:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 01:21:03 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e2445eddd520acc99c0726888b224865c2a40b1f13168bed9a799f272e7e12`  
		Last Modified: Tue, 26 Sep 2023 18:20:18 GMT  
		Size: 7.7 MB (7669639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01a2151075c010ad6d54d0de1286f72a2909c2adb250b25f9fb400a0e04eac0`  
		Last Modified: Tue, 17 Oct 2023 01:22:43 GMT  
		Size: 227.1 MB (227118914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151d7b12e398dedd5a77f271fa6820938915d579580f3456fe00dd6f06406801`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e2a4a736bcb63eb1e4c0c3b18aefea77f95c9891709425036d44cc9bbd3d90`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e725a68ad78e232bc0902292bcafdddd35d216922a6117aea77d00a0618e0e2`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ba1db1f2f0f34c2e83ca0bc2bf86d9c0d434cf3ad507282f1745e8b94875ef`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e23c456e9a2e3ab59b11b0393c040ba4e141020ca10ec2424a0f7c6804b5ebb`  
		Last Modified: Tue, 17 Oct 2023 01:22:25 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2.10` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:84b974e87b1b9b148e0f9b53c610131d97e34107db35d50ff158dca6c08f04f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302429188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2b51d99b4f26d601cdc5f14e2512aeb882c73d27013275b3fc1f20270506e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:39:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 00:41:59 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.10.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.10.tar.gz.asc crate-5.2.10.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.10.tar.gz.asc     && tar -xf crate-5.2.10.tar.gz -C /crate --strip-components=1     && rm crate-5.2.10.tar.gz
# Tue, 17 Oct 2023 00:42:03 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 00:42:03 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 00:42:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 00:42:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 00:42:04 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 00:42:04 GMT
WORKDIR /data
# Tue, 17 Oct 2023 00:42:04 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 00:42:04 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 00:42:04 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 00:42:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T15:07:59.910862 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.10
# Tue, 17 Oct 2023 00:42:04 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 00:42:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 00:42:04 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed142c0b1a887b57068b49d7c01694330116d5e4223aa1ec3f5d266d37add262`  
		Last Modified: Tue, 26 Sep 2023 18:40:17 GMT  
		Size: 7.5 MB (7510200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a97b356aa78dea3947ee72ea6a4d8d69f6a1864337ecec709be87c1141ff07`  
		Last Modified: Tue, 17 Oct 2023 00:43:33 GMT  
		Size: 225.9 MB (225861924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631719eff1c8e13820f8a3a86a5f67f796731971b9c346544b39cf12924985db`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 1.9 MB (1931737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee3cad283afe4bf0c54fde1d0f244ca5d33a7c1e64d11131d2f18efa7fa264`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6ff39bfa60dc5097d745cc385e007dc038db158d5a35d2338bcc2b08edf47e`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7315a2755765ae42620461d3f11de8bedbd40888391d2cfd5ed179fccd05482f`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e40db3b84ff3a56d1e5d7eed970aeec3bc9df1abef5e2809349146cff582934`  
		Last Modified: Tue, 17 Oct 2023 00:43:17 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3`

```console
$ docker pull crate@sha256:b9a9789814efdff94830c6620eb9a582f99af11bac501d20e03504b06e68da90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3` - linux; amd64

```console
$ docker pull crate@sha256:af7c0874200b140b8dd548095673f59fe74d7a556dd63e694b649a4bec4992b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297909615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794acb93f246a38d9098f1007041c3c72f7a03aa6c02cf1824edc28e75a5b119`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 01:20:29 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.7.tar.gz.asc crate-5.3.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.7.tar.gz.asc     && tar -xf crate-5.3.7.tar.gz -C /crate --strip-components=1     && rm crate-5.3.7.tar.gz
# Tue, 17 Oct 2023 01:20:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 01:20:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 01:20:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 01:20:32 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 01:20:32 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 01:20:33 GMT
WORKDIR /data
# Tue, 17 Oct 2023 01:20:33 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 01:20:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 01:20:33 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 01:20:33 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T16:00:23.375147 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.7
# Tue, 17 Oct 2023 01:20:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 01:20:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 01:20:33 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d128efc14189e19b8aa9c4f5a0eec8968c3b24e069b006640e98dc8f3169d81`  
		Last Modified: Tue, 18 Jul 2023 19:27:39 GMT  
		Size: 427.7 KB (427659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8d6fa025c4ff4bdf1a7c13a43cee6dd94f6b1b8801e5a487164b7b830646f6`  
		Last Modified: Tue, 17 Oct 2023 01:22:14 GMT  
		Size: 227.3 MB (227336117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62129f197f5a160885365d625bf779ca29d8aa284bb25f3d24295f07c4edf7e1`  
		Last Modified: Tue, 17 Oct 2023 01:21:55 GMT  
		Size: 1.9 MB (1931721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3642f5b3c7402183ef52780ffbdb5ef84e08086df6f265426f580e35423fd932`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea54b1babc6928f5cb43a432c62126edf385f20dc9eae51605f9acc183aa07`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e426145a6c06b60fa3bb9b629b4ca45595849e3af292f411da2bc0e5a2fd4`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6f9e4b0367b79c265b11975250bcc2c907ade5856edbf1fe398aba5aa3cb6`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:3e1bc33c4e940f1539b7dbf8207b306c81bf5d64977877a32564048d70d05f74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295564520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac3b646da4ea50063b819a84481bdad68d0505f954f778423beb035b9e2ef94`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 00:41:25 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.7.tar.gz.asc crate-5.3.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.7.tar.gz.asc     && tar -xf crate-5.3.7.tar.gz -C /crate --strip-components=1     && rm crate-5.3.7.tar.gz
# Tue, 17 Oct 2023 00:41:29 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 00:41:29 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 00:41:29 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 00:41:29 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 00:41:29 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 00:41:29 GMT
WORKDIR /data
# Tue, 17 Oct 2023 00:41:30 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 00:41:30 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 00:41:30 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 00:41:30 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T16:00:23.375147 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.7
# Tue, 17 Oct 2023 00:41:30 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 00:41:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 00:41:30 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5c408286eb8cf39dd4a503a1dcfd5cd1231b678372fbf9ea9ffb1baa10f028`  
		Last Modified: Tue, 18 Jul 2023 19:45:22 GMT  
		Size: 427.0 KB (426966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9f19740a158cf73a323966f2944a57fa3206315a14c7bc41f2b486e6cbe66`  
		Last Modified: Tue, 17 Oct 2023 00:43:08 GMT  
		Size: 226.1 MB (226080492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4927bb961d222303d8641be0fd304b0ab9d14f0bf0fdb7c4b1181367b9938559`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1125d1dbec9fe284b7e3a17261e3351448872b7e98eb642c3e4ddd165ecad418`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338cb355632f9cff47b8e9557e2e66fe139e07b46aaf8d8470c73e5e1ee2919a`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac2c3b3fc842b0664bafbdb63dbf4db6e5343032b34c0e2863699e2bd7e13ce`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7c3e98b0d45ec19a30917dd6b5d65fb64346ec379d0829cebdeb4ddaf5bc84`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3.7`

```console
$ docker pull crate@sha256:b9a9789814efdff94830c6620eb9a582f99af11bac501d20e03504b06e68da90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3.7` - linux; amd64

```console
$ docker pull crate@sha256:af7c0874200b140b8dd548095673f59fe74d7a556dd63e694b649a4bec4992b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297909615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794acb93f246a38d9098f1007041c3c72f7a03aa6c02cf1824edc28e75a5b119`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 01:20:29 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.7.tar.gz.asc crate-5.3.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.7.tar.gz.asc     && tar -xf crate-5.3.7.tar.gz -C /crate --strip-components=1     && rm crate-5.3.7.tar.gz
# Tue, 17 Oct 2023 01:20:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 01:20:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 01:20:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 01:20:32 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 01:20:32 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 01:20:33 GMT
WORKDIR /data
# Tue, 17 Oct 2023 01:20:33 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 01:20:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 01:20:33 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 01:20:33 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T16:00:23.375147 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.7
# Tue, 17 Oct 2023 01:20:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 01:20:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 01:20:33 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d128efc14189e19b8aa9c4f5a0eec8968c3b24e069b006640e98dc8f3169d81`  
		Last Modified: Tue, 18 Jul 2023 19:27:39 GMT  
		Size: 427.7 KB (427659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8d6fa025c4ff4bdf1a7c13a43cee6dd94f6b1b8801e5a487164b7b830646f6`  
		Last Modified: Tue, 17 Oct 2023 01:22:14 GMT  
		Size: 227.3 MB (227336117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62129f197f5a160885365d625bf779ca29d8aa284bb25f3d24295f07c4edf7e1`  
		Last Modified: Tue, 17 Oct 2023 01:21:55 GMT  
		Size: 1.9 MB (1931721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3642f5b3c7402183ef52780ffbdb5ef84e08086df6f265426f580e35423fd932`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea54b1babc6928f5cb43a432c62126edf385f20dc9eae51605f9acc183aa07`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345e426145a6c06b60fa3bb9b629b4ca45595849e3af292f411da2bc0e5a2fd4`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6f9e4b0367b79c265b11975250bcc2c907ade5856edbf1fe398aba5aa3cb6`  
		Last Modified: Tue, 17 Oct 2023 01:21:54 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3.7` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:3e1bc33c4e940f1539b7dbf8207b306c81bf5d64977877a32564048d70d05f74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295564520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac3b646da4ea50063b819a84481bdad68d0505f954f778423beb035b9e2ef94`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Tue, 17 Oct 2023 00:41:25 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.7.tar.gz.asc crate-5.3.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.7.tar.gz.asc     && tar -xf crate-5.3.7.tar.gz -C /crate --strip-components=1     && rm crate-5.3.7.tar.gz
# Tue, 17 Oct 2023 00:41:29 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 17 Oct 2023 00:41:29 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Oct 2023 00:41:29 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 17 Oct 2023 00:41:29 GMT
RUN mkdir -p /data/data /data/log
# Tue, 17 Oct 2023 00:41:29 GMT
VOLUME [/data]
# Tue, 17 Oct 2023 00:41:29 GMT
WORKDIR /data
# Tue, 17 Oct 2023 00:41:30 GMT
EXPOSE 4200 4300 5432
# Tue, 17 Oct 2023 00:41:30 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 17 Oct 2023 00:41:30 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 17 Oct 2023 00:41:30 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-12T16:00:23.375147 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.7
# Tue, 17 Oct 2023 00:41:30 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 17 Oct 2023 00:41:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Oct 2023 00:41:30 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5c408286eb8cf39dd4a503a1dcfd5cd1231b678372fbf9ea9ffb1baa10f028`  
		Last Modified: Tue, 18 Jul 2023 19:45:22 GMT  
		Size: 427.0 KB (426966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9f19740a158cf73a323966f2944a57fa3206315a14c7bc41f2b486e6cbe66`  
		Last Modified: Tue, 17 Oct 2023 00:43:08 GMT  
		Size: 226.1 MB (226080492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4927bb961d222303d8641be0fd304b0ab9d14f0bf0fdb7c4b1181367b9938559`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1125d1dbec9fe284b7e3a17261e3351448872b7e98eb642c3e4ddd165ecad418`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338cb355632f9cff47b8e9557e2e66fe139e07b46aaf8d8470c73e5e1ee2919a`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac2c3b3fc842b0664bafbdb63dbf4db6e5343032b34c0e2863699e2bd7e13ce`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7c3e98b0d45ec19a30917dd6b5d65fb64346ec379d0829cebdeb4ddaf5bc84`  
		Last Modified: Tue, 17 Oct 2023 00:42:52 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.4`

```console
$ docker pull crate@sha256:fc703b01f9de9914df2fbaea4d3f71200f2ed62c8d66dbe66d44620dfc52671d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.4` - linux; amd64

```console
$ docker pull crate@sha256:332bf58f06b4a980bad1aaed312b2c1a09e7577305df344b210264e3708edc0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300131288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d8e540332488e8db46bcb48d4eeb656ac680fdf7c3d5f6dd678151ed84a1a4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 06 Nov 2023 23:25:57 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.5.tar.gz.asc crate-5.4.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.5.tar.gz.asc     && tar -xf crate-5.4.5.tar.gz -C /crate --strip-components=1     && rm crate-5.4.5.tar.gz
# Mon, 06 Nov 2023 23:25:59 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 06 Nov 2023 23:25:59 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Nov 2023 23:25:59 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 06 Nov 2023 23:26:00 GMT
RUN mkdir -p /data/data /data/log
# Mon, 06 Nov 2023 23:26:00 GMT
VOLUME [/data]
# Mon, 06 Nov 2023 23:26:00 GMT
WORKDIR /data
# Mon, 06 Nov 2023 23:26:00 GMT
EXPOSE 4200 4300 5432
# Mon, 06 Nov 2023 23:26:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 06 Nov 2023 23:26:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 06 Nov 2023 23:26:00 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-26T14:14:55.560128 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.5
# Mon, 06 Nov 2023 23:26:00 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 06 Nov 2023 23:26:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Nov 2023 23:26:00 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d128efc14189e19b8aa9c4f5a0eec8968c3b24e069b006640e98dc8f3169d81`  
		Last Modified: Tue, 18 Jul 2023 19:27:39 GMT  
		Size: 427.7 KB (427659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea608d740d616c6cbaf6178bf2acb820ab7c7e9aecfee37f7d7b3ffb460176f0`  
		Last Modified: Mon, 06 Nov 2023 23:26:39 GMT  
		Size: 229.6 MB (229557773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2cb243788ba586f22e2fce53a283811939ea6b08df6636852296c4e4ea9fcf`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b13dd3896776fd771930e688bc50e6d010a0bf1a3a94d8a3ff248f7876a69`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de18cdec9be8bf72f0c5eb21aa8f5305e6d636d1c4437d3a1be4b2784c93e32`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464305d591838e61305e868e47868ccb969dd016a8d0ac3e8607c4e95b02ffab`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e53ddc845879098a33a481ab65b3773b236ff6a9f3e1abd4d857c0798d031`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f7ec1a9978cb5ea5d59c52fa3da31b6aa15842377617f4638c13d88adcea029d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297372671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ab75683e3efb84c350b42c07f06505e41d5411045c9b1360ec043a7dc3f7ae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 06 Nov 2023 23:39:32 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.5.tar.gz.asc crate-5.4.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.5.tar.gz.asc     && tar -xf crate-5.4.5.tar.gz -C /crate --strip-components=1     && rm crate-5.4.5.tar.gz
# Mon, 06 Nov 2023 23:39:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 06 Nov 2023 23:39:36 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Nov 2023 23:39:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 06 Nov 2023 23:39:37 GMT
RUN mkdir -p /data/data /data/log
# Mon, 06 Nov 2023 23:39:37 GMT
VOLUME [/data]
# Mon, 06 Nov 2023 23:39:37 GMT
WORKDIR /data
# Mon, 06 Nov 2023 23:39:37 GMT
EXPOSE 4200 4300 5432
# Mon, 06 Nov 2023 23:39:37 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 06 Nov 2023 23:39:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 06 Nov 2023 23:39:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-26T14:14:55.560128 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.5
# Mon, 06 Nov 2023 23:39:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 06 Nov 2023 23:39:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Nov 2023 23:39:38 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5c408286eb8cf39dd4a503a1dcfd5cd1231b678372fbf9ea9ffb1baa10f028`  
		Last Modified: Tue, 18 Jul 2023 19:45:22 GMT  
		Size: 427.0 KB (426966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09009b9dd8267b7308dac8188c35aeef0458783a427c45b144e14ef03badb4ed`  
		Last Modified: Mon, 06 Nov 2023 23:40:12 GMT  
		Size: 227.9 MB (227888642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a709f474325f2decdda5be986c691650ef0d0eb80ac1d31e74614f7c2c110e7`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 1.9 MB (1931736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b643f2cd3611b232259a8c7c73a095c18b7c16045b95d60d78f2eb8d2d4b537`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49bb8a27ed22a2503e6fba3e5e9c6117bee4e6b903abb66a9415fb5adb37dd2`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ead4cc371879fb87d40110287d6ad84a7aa6ee87b95447a8823b6d04f6db9`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3772c96f93fef38dc43e15907f3658bd7db2e9405498ab329e62791cb1ce22`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.4.5`

```console
$ docker pull crate@sha256:fc703b01f9de9914df2fbaea4d3f71200f2ed62c8d66dbe66d44620dfc52671d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.4.5` - linux; amd64

```console
$ docker pull crate@sha256:332bf58f06b4a980bad1aaed312b2c1a09e7577305df344b210264e3708edc0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300131288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d8e540332488e8db46bcb48d4eeb656ac680fdf7c3d5f6dd678151ed84a1a4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 06 Nov 2023 23:25:57 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.5.tar.gz.asc crate-5.4.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.5.tar.gz.asc     && tar -xf crate-5.4.5.tar.gz -C /crate --strip-components=1     && rm crate-5.4.5.tar.gz
# Mon, 06 Nov 2023 23:25:59 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 06 Nov 2023 23:25:59 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Nov 2023 23:25:59 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 06 Nov 2023 23:26:00 GMT
RUN mkdir -p /data/data /data/log
# Mon, 06 Nov 2023 23:26:00 GMT
VOLUME [/data]
# Mon, 06 Nov 2023 23:26:00 GMT
WORKDIR /data
# Mon, 06 Nov 2023 23:26:00 GMT
EXPOSE 4200 4300 5432
# Mon, 06 Nov 2023 23:26:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 06 Nov 2023 23:26:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 06 Nov 2023 23:26:00 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-26T14:14:55.560128 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.5
# Mon, 06 Nov 2023 23:26:00 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 06 Nov 2023 23:26:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Nov 2023 23:26:00 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d128efc14189e19b8aa9c4f5a0eec8968c3b24e069b006640e98dc8f3169d81`  
		Last Modified: Tue, 18 Jul 2023 19:27:39 GMT  
		Size: 427.7 KB (427659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea608d740d616c6cbaf6178bf2acb820ab7c7e9aecfee37f7d7b3ffb460176f0`  
		Last Modified: Mon, 06 Nov 2023 23:26:39 GMT  
		Size: 229.6 MB (229557773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2cb243788ba586f22e2fce53a283811939ea6b08df6636852296c4e4ea9fcf`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b13dd3896776fd771930e688bc50e6d010a0bf1a3a94d8a3ff248f7876a69`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de18cdec9be8bf72f0c5eb21aa8f5305e6d636d1c4437d3a1be4b2784c93e32`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464305d591838e61305e868e47868ccb969dd016a8d0ac3e8607c4e95b02ffab`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e53ddc845879098a33a481ab65b3773b236ff6a9f3e1abd4d857c0798d031`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.4.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f7ec1a9978cb5ea5d59c52fa3da31b6aa15842377617f4638c13d88adcea029d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297372671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ab75683e3efb84c350b42c07f06505e41d5411045c9b1360ec043a7dc3f7ae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 06 Nov 2023 23:39:32 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.5.tar.gz.asc crate-5.4.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.5.tar.gz.asc     && tar -xf crate-5.4.5.tar.gz -C /crate --strip-components=1     && rm crate-5.4.5.tar.gz
# Mon, 06 Nov 2023 23:39:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 06 Nov 2023 23:39:36 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Nov 2023 23:39:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 06 Nov 2023 23:39:37 GMT
RUN mkdir -p /data/data /data/log
# Mon, 06 Nov 2023 23:39:37 GMT
VOLUME [/data]
# Mon, 06 Nov 2023 23:39:37 GMT
WORKDIR /data
# Mon, 06 Nov 2023 23:39:37 GMT
EXPOSE 4200 4300 5432
# Mon, 06 Nov 2023 23:39:37 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 06 Nov 2023 23:39:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 06 Nov 2023 23:39:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-26T14:14:55.560128 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.5
# Mon, 06 Nov 2023 23:39:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 06 Nov 2023 23:39:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Nov 2023 23:39:38 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5c408286eb8cf39dd4a503a1dcfd5cd1231b678372fbf9ea9ffb1baa10f028`  
		Last Modified: Tue, 18 Jul 2023 19:45:22 GMT  
		Size: 427.0 KB (426966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09009b9dd8267b7308dac8188c35aeef0458783a427c45b144e14ef03badb4ed`  
		Last Modified: Mon, 06 Nov 2023 23:40:12 GMT  
		Size: 227.9 MB (227888642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a709f474325f2decdda5be986c691650ef0d0eb80ac1d31e74614f7c2c110e7`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 1.9 MB (1931736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b643f2cd3611b232259a8c7c73a095c18b7c16045b95d60d78f2eb8d2d4b537`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49bb8a27ed22a2503e6fba3e5e9c6117bee4e6b903abb66a9415fb5adb37dd2`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ead4cc371879fb87d40110287d6ad84a7aa6ee87b95447a8823b6d04f6db9`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3772c96f93fef38dc43e15907f3658bd7db2e9405498ab329e62791cb1ce22`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.5`

**does not exist** (yet?)

## `crate:5.5.0`

**does not exist** (yet?)

## `crate:latest`

```console
$ docker pull crate@sha256:fc703b01f9de9914df2fbaea4d3f71200f2ed62c8d66dbe66d44620dfc52671d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:332bf58f06b4a980bad1aaed312b2c1a09e7577305df344b210264e3708edc0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300131288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d8e540332488e8db46bcb48d4eeb656ac680fdf7c3d5f6dd678151ed84a1a4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 06 Nov 2023 23:25:57 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.5.tar.gz.asc crate-5.4.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.5.tar.gz.asc     && tar -xf crate-5.4.5.tar.gz -C /crate --strip-components=1     && rm crate-5.4.5.tar.gz
# Mon, 06 Nov 2023 23:25:59 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 06 Nov 2023 23:25:59 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Nov 2023 23:25:59 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 06 Nov 2023 23:26:00 GMT
RUN mkdir -p /data/data /data/log
# Mon, 06 Nov 2023 23:26:00 GMT
VOLUME [/data]
# Mon, 06 Nov 2023 23:26:00 GMT
WORKDIR /data
# Mon, 06 Nov 2023 23:26:00 GMT
EXPOSE 4200 4300 5432
# Mon, 06 Nov 2023 23:26:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 06 Nov 2023 23:26:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 06 Nov 2023 23:26:00 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-26T14:14:55.560128 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.5
# Mon, 06 Nov 2023 23:26:00 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 06 Nov 2023 23:26:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Nov 2023 23:26:00 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:92cbf8f6375271a4008121ff3ad96dbd0c10df3c4bc4a8951ba206dd0ffa17e2`  
		Last Modified: Tue, 18 Jul 2023 19:21:32 GMT  
		Size: 68.2 MB (68212236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d128efc14189e19b8aa9c4f5a0eec8968c3b24e069b006640e98dc8f3169d81`  
		Last Modified: Tue, 18 Jul 2023 19:27:39 GMT  
		Size: 427.7 KB (427659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea608d740d616c6cbaf6178bf2acb820ab7c7e9aecfee37f7d7b3ffb460176f0`  
		Last Modified: Mon, 06 Nov 2023 23:26:39 GMT  
		Size: 229.6 MB (229557773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2cb243788ba586f22e2fce53a283811939ea6b08df6636852296c4e4ea9fcf`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b13dd3896776fd771930e688bc50e6d010a0bf1a3a94d8a3ff248f7876a69`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de18cdec9be8bf72f0c5eb21aa8f5305e6d636d1c4437d3a1be4b2784c93e32`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464305d591838e61305e868e47868ccb969dd016a8d0ac3e8607c4e95b02ffab`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e53ddc845879098a33a481ab65b3773b236ff6a9f3e1abd4d857c0798d031`  
		Last Modified: Mon, 06 Nov 2023 23:26:21 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f7ec1a9978cb5ea5d59c52fa3da31b6aa15842377617f4638c13d88adcea029d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297372671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ab75683e3efb84c350b42c07f06505e41d5411045c9b1360ec043a7dc3f7ae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 06 Nov 2023 23:39:32 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.5.tar.gz.asc crate-5.4.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.5.tar.gz.asc     && tar -xf crate-5.4.5.tar.gz -C /crate --strip-components=1     && rm crate-5.4.5.tar.gz
# Mon, 06 Nov 2023 23:39:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 06 Nov 2023 23:39:36 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Nov 2023 23:39:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 06 Nov 2023 23:39:37 GMT
RUN mkdir -p /data/data /data/log
# Mon, 06 Nov 2023 23:39:37 GMT
VOLUME [/data]
# Mon, 06 Nov 2023 23:39:37 GMT
WORKDIR /data
# Mon, 06 Nov 2023 23:39:37 GMT
EXPOSE 4200 4300 5432
# Mon, 06 Nov 2023 23:39:37 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 06 Nov 2023 23:39:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 06 Nov 2023 23:39:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-26T14:14:55.560128 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.5
# Mon, 06 Nov 2023 23:39:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 06 Nov 2023 23:39:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Nov 2023 23:39:38 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:835f37e6c17066f8e99a562de9c491c11a1562baae1f6d2476852c9c30f298e2`  
		Last Modified: Tue, 18 Jul 2023 19:40:41 GMT  
		Size: 67.1 MB (67123448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5c408286eb8cf39dd4a503a1dcfd5cd1231b678372fbf9ea9ffb1baa10f028`  
		Last Modified: Tue, 18 Jul 2023 19:45:22 GMT  
		Size: 427.0 KB (426966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09009b9dd8267b7308dac8188c35aeef0458783a427c45b144e14ef03badb4ed`  
		Last Modified: Mon, 06 Nov 2023 23:40:12 GMT  
		Size: 227.9 MB (227888642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a709f474325f2decdda5be986c691650ef0d0eb80ac1d31e74614f7c2c110e7`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 1.9 MB (1931736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b643f2cd3611b232259a8c7c73a095c18b7c16045b95d60d78f2eb8d2d4b537`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49bb8a27ed22a2503e6fba3e5e9c6117bee4e6b903abb66a9415fb5adb37dd2`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ead4cc371879fb87d40110287d6ad84a7aa6ee87b95447a8823b6d04f6db9`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3772c96f93fef38dc43e15907f3658bd7db2e9405498ab329e62791cb1ce22`  
		Last Modified: Mon, 06 Nov 2023 23:39:55 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
