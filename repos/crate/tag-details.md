<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.8`](#crate48)
-	[`crate:4.8.4`](#crate484)
-	[`crate:5.2`](#crate52)
-	[`crate:5.2.11`](#crate5211)
-	[`crate:5.3`](#crate53)
-	[`crate:5.3.8`](#crate538)
-	[`crate:5.4`](#crate54)
-	[`crate:5.4.7`](#crate547)
-	[`crate:5.5`](#crate55)
-	[`crate:5.5.2`](#crate552)
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
$ docker pull crate@sha256:fa88219443f9b3b4a07c6b990bf8da3cebaafce74ab18430c2567eb1c8be2965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2` - linux; amd64

```console
$ docker pull crate@sha256:dcd0b77639efc8bda4c180d156cafca573bff7c6a44077a578fe7d5ada4938b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.9 MB (304918286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8022b1f51efe59386add96fe0bfc66fb9d01f34f1a136882d96be289f8a6241d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:50:24 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:41:33 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.11.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.11.tar.gz.asc crate-5.2.11.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.11.tar.gz.asc     && tar -xf crate-5.2.11.tar.gz -C /crate --strip-components=1     && rm crate-5.2.11.tar.gz
# Fri, 22 Dec 2023 17:41:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:41:36 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:41:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:41:36 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:41:37 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:41:37 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:41:37 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:41:37 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:41:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:41:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T22:23:59.881502 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.11
# Fri, 22 Dec 2023 17:41:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:41:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:41:37 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e88b37c36ac28be31a7117edcd4f546a476c12a070fc3589cc37db76ba889f4`  
		Last Modified: Tue, 28 Nov 2023 23:52:33 GMT  
		Size: 7.6 MB (7631993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73998c67972394f920e394236c9b6e646b47915c9835233fb40a7d60b606ea17`  
		Last Modified: Fri, 22 Dec 2023 17:43:30 GMT  
		Size: 227.1 MB (227118338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed06fd9479549db9babc3bd5defd2c4cd929404ba7f00564842f3e0331829e89`  
		Last Modified: Fri, 22 Dec 2023 17:43:13 GMT  
		Size: 2.0 MB (1954459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2d48901b62d452ebfdf1181fd2f3e5929c3d42fe64812e16e2ff0afc0c3f`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71369e426eb744876fb67e6575ffd40a46f9c61b54a7b8aab4b24c8d3df6ce7c`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bbf37580501f74d7d667b58a903c1118c94b1b5a4eb59d9e3acc503f4b4160`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493fd7210360356b806e897499106d909fd707bca5e7be77de17de883fbb8b2`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:bb2cc3511fc0db954f3633003f999cd13ad856b1d718d598a7f730422b8a0d25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302386287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f24a8752e7a8a6483216aabc514a711d6c87c3d6a907929a42b75b42147ba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:18:09 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:42:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.11.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.11.tar.gz.asc crate-5.2.11.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.11.tar.gz.asc     && tar -xf crate-5.2.11.tar.gz -C /crate --strip-components=1     && rm crate-5.2.11.tar.gz
# Fri, 22 Dec 2023 16:42:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:42:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:42:27 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:42:27 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:42:27 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:42:27 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:42:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:42:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:42:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T22:23:59.881502 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.11
# Fri, 22 Dec 2023 16:42:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:42:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:42:27 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f804096b6187f46a18908e90329b82a2f8cafca25ef269a42d22649e1fefc5`  
		Last Modified: Wed, 29 Nov 2023 00:20:12 GMT  
		Size: 7.5 MB (7476469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076fbd85ac340b0ce200b8a8d8e3f96994f244e6befdad5f45640f68e8388b12`  
		Last Modified: Fri, 22 Dec 2023 16:44:12 GMT  
		Size: 225.9 MB (225862476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8248ae993931cc052ef49a06139081896f10ab57e30f8f04b4b716c1853c9b8c`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 2.0 MB (1954468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb53d8c3574a537d8ed8374bd27619066a0f2378ed505693916c45dccd21130`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a9e523c7020d1d30f760dd234f14a9feedc6341569d0a1a386bbc2056cd582`  
		Last Modified: Fri, 22 Dec 2023 16:43:56 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66466fcbd874375b213152887c029161d6b961455e397bc5fa7b4abe090251`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3552d95f911a73741d911a7c58a437bc8b5b4a07784bd95323ae649418c426c`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2.11`

```console
$ docker pull crate@sha256:fa88219443f9b3b4a07c6b990bf8da3cebaafce74ab18430c2567eb1c8be2965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2.11` - linux; amd64

```console
$ docker pull crate@sha256:dcd0b77639efc8bda4c180d156cafca573bff7c6a44077a578fe7d5ada4938b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.9 MB (304918286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8022b1f51efe59386add96fe0bfc66fb9d01f34f1a136882d96be289f8a6241d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:50:24 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:41:33 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.11.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.11.tar.gz.asc crate-5.2.11.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.11.tar.gz.asc     && tar -xf crate-5.2.11.tar.gz -C /crate --strip-components=1     && rm crate-5.2.11.tar.gz
# Fri, 22 Dec 2023 17:41:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:41:36 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:41:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:41:36 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:41:37 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:41:37 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:41:37 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:41:37 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:41:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:41:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T22:23:59.881502 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.11
# Fri, 22 Dec 2023 17:41:37 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:41:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:41:37 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e88b37c36ac28be31a7117edcd4f546a476c12a070fc3589cc37db76ba889f4`  
		Last Modified: Tue, 28 Nov 2023 23:52:33 GMT  
		Size: 7.6 MB (7631993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73998c67972394f920e394236c9b6e646b47915c9835233fb40a7d60b606ea17`  
		Last Modified: Fri, 22 Dec 2023 17:43:30 GMT  
		Size: 227.1 MB (227118338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed06fd9479549db9babc3bd5defd2c4cd929404ba7f00564842f3e0331829e89`  
		Last Modified: Fri, 22 Dec 2023 17:43:13 GMT  
		Size: 2.0 MB (1954459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad2d48901b62d452ebfdf1181fd2f3e5929c3d42fe64812e16e2ff0afc0c3f`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71369e426eb744876fb67e6575ffd40a46f9c61b54a7b8aab4b24c8d3df6ce7c`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bbf37580501f74d7d667b58a903c1118c94b1b5a4eb59d9e3acc503f4b4160`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493fd7210360356b806e897499106d909fd707bca5e7be77de17de883fbb8b2`  
		Last Modified: Fri, 22 Dec 2023 17:43:12 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2.11` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:bb2cc3511fc0db954f3633003f999cd13ad856b1d718d598a7f730422b8a0d25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302386287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288f24a8752e7a8a6483216aabc514a711d6c87c3d6a907929a42b75b42147ba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:18:09 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:42:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.11.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.11.tar.gz.asc crate-5.2.11.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.11.tar.gz.asc     && tar -xf crate-5.2.11.tar.gz -C /crate --strip-components=1     && rm crate-5.2.11.tar.gz
# Fri, 22 Dec 2023 16:42:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:42:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:42:27 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:42:27 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:42:27 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:42:27 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:42:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:42:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:42:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T22:23:59.881502 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.11
# Fri, 22 Dec 2023 16:42:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:42:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:42:27 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f804096b6187f46a18908e90329b82a2f8cafca25ef269a42d22649e1fefc5`  
		Last Modified: Wed, 29 Nov 2023 00:20:12 GMT  
		Size: 7.5 MB (7476469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076fbd85ac340b0ce200b8a8d8e3f96994f244e6befdad5f45640f68e8388b12`  
		Last Modified: Fri, 22 Dec 2023 16:44:12 GMT  
		Size: 225.9 MB (225862476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8248ae993931cc052ef49a06139081896f10ab57e30f8f04b4b716c1853c9b8c`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 2.0 MB (1954468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb53d8c3574a537d8ed8374bd27619066a0f2378ed505693916c45dccd21130`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a9e523c7020d1d30f760dd234f14a9feedc6341569d0a1a386bbc2056cd582`  
		Last Modified: Fri, 22 Dec 2023 16:43:56 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66466fcbd874375b213152887c029161d6b961455e397bc5fa7b4abe090251`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3552d95f911a73741d911a7c58a437bc8b5b4a07784bd95323ae649418c426c`  
		Last Modified: Fri, 22 Dec 2023 16:43:57 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3`

```console
$ docker pull crate@sha256:d188481e9a593b678a7cb3dacffe41c3b6ace3cabec94bdce860d3f431ad9fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3` - linux; amd64

```console
$ docker pull crate@sha256:72e1762efa5499cfa2f443e223f6f007fae992959c8a196701f3537f847ea32a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297930729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe2ec8f908d3c36d86b9e00ed4945da77f2b2c26a799b4e9e84d26dd9055e43d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:41:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.8.tar.gz.asc crate-5.3.8.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.8.tar.gz.asc     && tar -xf crate-5.3.8.tar.gz -C /crate --strip-components=1     && rm crate-5.3.8.tar.gz
# Fri, 22 Dec 2023 17:41:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:41:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:41:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:41:08 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:41:08 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:41:08 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:41:08 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:41:08 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:41:08 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:41:08 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:59:09.428079 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.8
# Fri, 22 Dec 2023 17:41:08 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:41:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:41:09 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed71ed73d6d1e26b4598b27b6922a6dabb37dd18424875e3d4f9396abc851496`  
		Last Modified: Fri, 22 Dec 2023 17:43:03 GMT  
		Size: 227.3 MB (227337865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efcce8b61ca8721ce1b2d5e24b2984385a945b1833478feb64b1d472f858a2`  
		Last Modified: Fri, 22 Dec 2023 17:42:45 GMT  
		Size: 2.0 MB (1954468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560afeeb50a963e328a353e75774e126d19b86475bdc6170cd6621d085711ab8`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a9600ce990081a75d9ecc807b9e48bac0bf83f7c894a1290e13b60801071be`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c529bd8d4f7f31fbe1aa5a635b231ad311bb88d524d300e46c39374b63ecbf39`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa368687e761bb921f314720c3f369725dd4acd812eaf49b02369217424e63`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:69075ab59476b844b8b0459c8f4412c3b62e2533ca39143c25ca99c5c1ab1d66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295553796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25eb2553ac1ad75975e602a830d077f0eb0c7d6ad0c4ccf88741097ef142062a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:41:49 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.8.tar.gz.asc crate-5.3.8.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.8.tar.gz.asc     && tar -xf crate-5.3.8.tar.gz -C /crate --strip-components=1     && rm crate-5.3.8.tar.gz
# Fri, 22 Dec 2023 16:41:53 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:41:53 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:41:53 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:41:53 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:41:53 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:41:53 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:41:53 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:41:54 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:41:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:41:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:59:09.428079 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.8
# Fri, 22 Dec 2023 16:41:54 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:41:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:41:54 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0024f343dffa598175d76f0549f208f634dcc2b8133051fc8577ffdb615b6f5`  
		Last Modified: Fri, 22 Dec 2023 16:43:46 GMT  
		Size: 226.1 MB (226082058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f8e82c2b861d4ae3ed2272a2bb3a08b10feddf7ae85d23b6be9884fe59978`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 2.0 MB (1954462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5ad0c7670ba360e57925928d2c0cbeb903c262e17ef0c2c0ac2dc7b7d9f413`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574ef3deec2305c7045abfd80999d42af27d360ea44ec7f1fe9a6c9bb7c85e8`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fe1f2cec555b74603fcb59e3eeb491196e59398289d2a0b43ba6036400cbdd`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ed1a90023ad113da4500116d4bd5ba68e9953594817e1017ffd325dfa8bfb1`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3.8`

```console
$ docker pull crate@sha256:d188481e9a593b678a7cb3dacffe41c3b6ace3cabec94bdce860d3f431ad9fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3.8` - linux; amd64

```console
$ docker pull crate@sha256:72e1762efa5499cfa2f443e223f6f007fae992959c8a196701f3537f847ea32a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297930729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe2ec8f908d3c36d86b9e00ed4945da77f2b2c26a799b4e9e84d26dd9055e43d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:41:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.8.tar.gz.asc crate-5.3.8.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.8.tar.gz.asc     && tar -xf crate-5.3.8.tar.gz -C /crate --strip-components=1     && rm crate-5.3.8.tar.gz
# Fri, 22 Dec 2023 17:41:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:41:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:41:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:41:08 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:41:08 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:41:08 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:41:08 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:41:08 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:41:08 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:41:08 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:59:09.428079 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.8
# Fri, 22 Dec 2023 17:41:08 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:41:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:41:09 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed71ed73d6d1e26b4598b27b6922a6dabb37dd18424875e3d4f9396abc851496`  
		Last Modified: Fri, 22 Dec 2023 17:43:03 GMT  
		Size: 227.3 MB (227337865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efcce8b61ca8721ce1b2d5e24b2984385a945b1833478feb64b1d472f858a2`  
		Last Modified: Fri, 22 Dec 2023 17:42:45 GMT  
		Size: 2.0 MB (1954468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560afeeb50a963e328a353e75774e126d19b86475bdc6170cd6621d085711ab8`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a9600ce990081a75d9ecc807b9e48bac0bf83f7c894a1290e13b60801071be`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c529bd8d4f7f31fbe1aa5a635b231ad311bb88d524d300e46c39374b63ecbf39`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa368687e761bb921f314720c3f369725dd4acd812eaf49b02369217424e63`  
		Last Modified: Fri, 22 Dec 2023 17:42:44 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:69075ab59476b844b8b0459c8f4412c3b62e2533ca39143c25ca99c5c1ab1d66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295553796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25eb2553ac1ad75975e602a830d077f0eb0c7d6ad0c4ccf88741097ef142062a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:41:49 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.8.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.8.tar.gz.asc crate-5.3.8.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.8.tar.gz.asc     && tar -xf crate-5.3.8.tar.gz -C /crate --strip-components=1     && rm crate-5.3.8.tar.gz
# Fri, 22 Dec 2023 16:41:53 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:41:53 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:41:53 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:41:53 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:41:53 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:41:53 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:41:53 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:41:54 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:41:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:41:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:59:09.428079 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.8
# Fri, 22 Dec 2023 16:41:54 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:41:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:41:54 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0024f343dffa598175d76f0549f208f634dcc2b8133051fc8577ffdb615b6f5`  
		Last Modified: Fri, 22 Dec 2023 16:43:46 GMT  
		Size: 226.1 MB (226082058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f8e82c2b861d4ae3ed2272a2bb3a08b10feddf7ae85d23b6be9884fe59978`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 2.0 MB (1954462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5ad0c7670ba360e57925928d2c0cbeb903c262e17ef0c2c0ac2dc7b7d9f413`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b574ef3deec2305c7045abfd80999d42af27d360ea44ec7f1fe9a6c9bb7c85e8`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fe1f2cec555b74603fcb59e3eeb491196e59398289d2a0b43ba6036400cbdd`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ed1a90023ad113da4500116d4bd5ba68e9953594817e1017ffd325dfa8bfb1`  
		Last Modified: Fri, 22 Dec 2023 16:43:31 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.4`

```console
$ docker pull crate@sha256:fc08aadc210d303e160fbe8ea85e21eb6561ae9b5251bc2868efb30474a2a60c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.4` - linux; amd64

```console
$ docker pull crate@sha256:a8b52e1622cd8f696501beda0f0b0407c2de2204fc7981aa6982e63ae71d1ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300153147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b935eaf0589e861bfdf0e1376f93ff4e691ac40f3105e34d3ff32c7b1969db2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:40:31 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.7.tar.gz.asc crate-5.4.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.7.tar.gz.asc     && tar -xf crate-5.4.7.tar.gz -C /crate --strip-components=1     && rm crate-5.4.7.tar.gz
# Fri, 22 Dec 2023 17:40:33 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:40:33 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:40:33 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:40:34 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:40:34 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:40:34 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:40:34 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:40:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:40:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:40:35 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T20:14:00.920830 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.7
# Fri, 22 Dec 2023 17:40:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:40:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:40:35 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a11d5a208146a1413c9312b8b3ae9f0f743a8b8bf0b37860e7a1739061195`  
		Last Modified: Fri, 22 Dec 2023 17:42:33 GMT  
		Size: 229.6 MB (229560285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fdc87f9d3fedec199722b8607a5d9cde2f0ab32c23ecc03b96836be6e96dc0`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 2.0 MB (1954464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ef12cc24ad2ec045f074030e945d692bcb1263feed8007276d1e4d1644bbfa`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3063c57af558a333b596b3435a5e77c6bc5781cd806f2a51aa4db7e6617f81b5`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5181a3aab72f48b38612daa5c8e5886690dff2fea350666861f2acd445c3c2`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdacf193b85cff32dca85888845f02652365f9cd33bec411d217105cb1ae80ae`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:10543a8ba8f97177f791909ae97213fd45b27b902d828d90897f05e33a4b2b2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297359971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1117bca883d14b9254b5eb31e922b79c047654f06023e0e7f36b20182a8c02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:41:16 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.7.tar.gz.asc crate-5.4.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.7.tar.gz.asc     && tar -xf crate-5.4.7.tar.gz -C /crate --strip-components=1     && rm crate-5.4.7.tar.gz
# Fri, 22 Dec 2023 16:41:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:41:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:41:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:41:20 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:41:20 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:41:20 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:41:21 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:41:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:41:21 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T20:14:00.920830 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.7
# Fri, 22 Dec 2023 16:41:21 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:41:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:41:21 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264f2076ae84790542bf986c2ca4b712358a88517625d30c65581141fa572da2`  
		Last Modified: Fri, 22 Dec 2023 16:43:22 GMT  
		Size: 227.9 MB (227888229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe526431e743ea42f7697bd9fce6c0f10c14d0ff91583b9e3421e240679c1df`  
		Last Modified: Fri, 22 Dec 2023 16:43:07 GMT  
		Size: 2.0 MB (1954470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b19afb154affb0351eca9bde3e272502669febddd89eb8ebab47a6c2b7a5358`  
		Last Modified: Fri, 22 Dec 2023 16:43:07 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2e4467b510dbaf87e76ced298f9a1cb815464282f695614e55347a2f0eccba`  
		Last Modified: Fri, 22 Dec 2023 16:43:06 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6328215dbb68ad52cc68f052da7ea42d3b95b557b82c01b2b0485460510158`  
		Last Modified: Fri, 22 Dec 2023 16:43:06 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03fb530a0361bbbfae24c3f325e25a6b9d8a05984648187d2d773ae25116b34`  
		Last Modified: Fri, 22 Dec 2023 16:43:06 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.4.7`

```console
$ docker pull crate@sha256:fc08aadc210d303e160fbe8ea85e21eb6561ae9b5251bc2868efb30474a2a60c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.4.7` - linux; amd64

```console
$ docker pull crate@sha256:a8b52e1622cd8f696501beda0f0b0407c2de2204fc7981aa6982e63ae71d1ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300153147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b935eaf0589e861bfdf0e1376f93ff4e691ac40f3105e34d3ff32c7b1969db2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:40:31 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.7.tar.gz.asc crate-5.4.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.7.tar.gz.asc     && tar -xf crate-5.4.7.tar.gz -C /crate --strip-components=1     && rm crate-5.4.7.tar.gz
# Fri, 22 Dec 2023 17:40:33 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:40:33 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:40:33 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:40:34 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:40:34 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:40:34 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:40:34 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:40:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:40:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:40:35 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T20:14:00.920830 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.7
# Fri, 22 Dec 2023 17:40:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:40:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:40:35 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4a11d5a208146a1413c9312b8b3ae9f0f743a8b8bf0b37860e7a1739061195`  
		Last Modified: Fri, 22 Dec 2023 17:42:33 GMT  
		Size: 229.6 MB (229560285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fdc87f9d3fedec199722b8607a5d9cde2f0ab32c23ecc03b96836be6e96dc0`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 2.0 MB (1954464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ef12cc24ad2ec045f074030e945d692bcb1263feed8007276d1e4d1644bbfa`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3063c57af558a333b596b3435a5e77c6bc5781cd806f2a51aa4db7e6617f81b5`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5181a3aab72f48b38612daa5c8e5886690dff2fea350666861f2acd445c3c2`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdacf193b85cff32dca85888845f02652365f9cd33bec411d217105cb1ae80ae`  
		Last Modified: Fri, 22 Dec 2023 17:42:14 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.4.7` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:10543a8ba8f97177f791909ae97213fd45b27b902d828d90897f05e33a4b2b2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297359971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1117bca883d14b9254b5eb31e922b79c047654f06023e0e7f36b20182a8c02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:41:16 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.7.tar.gz.asc crate-5.4.7.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.7.tar.gz.asc     && tar -xf crate-5.4.7.tar.gz -C /crate --strip-components=1     && rm crate-5.4.7.tar.gz
# Fri, 22 Dec 2023 16:41:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:41:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:41:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:41:20 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:41:20 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:41:20 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:41:21 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:41:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:41:21 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T20:14:00.920830 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.7
# Fri, 22 Dec 2023 16:41:21 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:41:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:41:21 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264f2076ae84790542bf986c2ca4b712358a88517625d30c65581141fa572da2`  
		Last Modified: Fri, 22 Dec 2023 16:43:22 GMT  
		Size: 227.9 MB (227888229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe526431e743ea42f7697bd9fce6c0f10c14d0ff91583b9e3421e240679c1df`  
		Last Modified: Fri, 22 Dec 2023 16:43:07 GMT  
		Size: 2.0 MB (1954470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b19afb154affb0351eca9bde3e272502669febddd89eb8ebab47a6c2b7a5358`  
		Last Modified: Fri, 22 Dec 2023 16:43:07 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2e4467b510dbaf87e76ced298f9a1cb815464282f695614e55347a2f0eccba`  
		Last Modified: Fri, 22 Dec 2023 16:43:06 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6328215dbb68ad52cc68f052da7ea42d3b95b557b82c01b2b0485460510158`  
		Last Modified: Fri, 22 Dec 2023 16:43:06 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03fb530a0361bbbfae24c3f325e25a6b9d8a05984648187d2d773ae25116b34`  
		Last Modified: Fri, 22 Dec 2023 16:43:06 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.5`

```console
$ docker pull crate@sha256:451e22f8481a0313f195daa6e743939d4da1a93a592eb41d527978010449ee0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.5` - linux; amd64

```console
$ docker pull crate@sha256:eb7847697e1b9ec586a6f3ec8b2a3f103bb21a6fcf8acd74e019a7e3d3c5290b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.9 MB (186868864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265dc46fe158b01f5d18f659ed332368a558c71faa6e5f2c6581d7248d601762`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:39:58 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.2.tar.gz.asc crate-5.5.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.2.tar.gz.asc     && tar -xf crate-5.5.2.tar.gz -C /crate --strip-components=1     && rm crate-5.5.2.tar.gz
# Fri, 22 Dec 2023 17:40:00 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:40:00 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:40:01 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:40:01 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:40:01 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:40:01 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:40:01 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:40:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:40:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:40:02 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:11:54.972232 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.2
# Fri, 22 Dec 2023 17:40:02 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:40:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:40:02 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05a660053a74e0a9edb52edc7aafb8031c6b5dd2847ed86f1ecd0c094d8b7f`  
		Last Modified: Fri, 22 Dec 2023 17:42:03 GMT  
		Size: 116.3 MB (116276004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c622710106c69699c31fb030d1bf829d4e8f4aaa50f55ac3b28b54773b0807`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 2.0 MB (1954466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1513baeaf9f9576f8b93d8219de7261ba83d0b5cfa5dd1dcedb5be9655a061d9`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1458128d1e555db75f3e321d2567c3161ea13b21cf58a284c6aa30f7407c0ec`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5430e327bbe2a789cdcba9db631882a4b314bbf4ab7889d26edb759b84690846`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c87e01f2d95ccca0541a87bc8aa35d5c415f1adf0b63bb233e27302265ff3`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:ef3eeaa76efe3728df041a3564633fed4d33fcfe1119249c78713839953517e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185316256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7765681c0f03f57b6e2564b1b8f81405f0b677caac6624a462d7648d5ca3f747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:40:44 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.2.tar.gz.asc crate-5.5.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.2.tar.gz.asc     && tar -xf crate-5.5.2.tar.gz -C /crate --strip-components=1     && rm crate-5.5.2.tar.gz
# Fri, 22 Dec 2023 16:40:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:40:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:40:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:40:49 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:40:49 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:40:50 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:40:50 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:40:50 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:40:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:40:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:11:54.972232 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.2
# Fri, 22 Dec 2023 16:40:50 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:40:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:40:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566aa147c52fb34ae9c2cd58aa1580dc133ad08f5c1819d5fbcdf5458e15223f`  
		Last Modified: Fri, 22 Dec 2023 16:42:55 GMT  
		Size: 115.8 MB (115844512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eaade3584c0c68726c92dbf49e07acdbb278631931d0507afb413ea71e8bb`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 2.0 MB (1954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540d6d74d87b635dadb13114e9e606371a750e5bc2a59acb2e1c1c5ee58ecec0`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d619ab5c9ed042702e77b303f7a2eb4fcfabb0cfa66882234cecc45add74c3b3`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d26d214b8b17bf6941ce9ac961838a1edabd9eb1047c3d650cf5957be21bfad`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779f71414f45a627b954e5644e2d6250fc7e588c571c0287216b619da6058e5e`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.5.2`

```console
$ docker pull crate@sha256:451e22f8481a0313f195daa6e743939d4da1a93a592eb41d527978010449ee0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.5.2` - linux; amd64

```console
$ docker pull crate@sha256:eb7847697e1b9ec586a6f3ec8b2a3f103bb21a6fcf8acd74e019a7e3d3c5290b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.9 MB (186868864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265dc46fe158b01f5d18f659ed332368a558c71faa6e5f2c6581d7248d601762`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:39:58 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.2.tar.gz.asc crate-5.5.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.2.tar.gz.asc     && tar -xf crate-5.5.2.tar.gz -C /crate --strip-components=1     && rm crate-5.5.2.tar.gz
# Fri, 22 Dec 2023 17:40:00 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:40:00 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:40:01 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:40:01 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:40:01 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:40:01 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:40:01 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:40:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:40:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:40:02 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:11:54.972232 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.2
# Fri, 22 Dec 2023 17:40:02 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:40:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:40:02 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05a660053a74e0a9edb52edc7aafb8031c6b5dd2847ed86f1ecd0c094d8b7f`  
		Last Modified: Fri, 22 Dec 2023 17:42:03 GMT  
		Size: 116.3 MB (116276004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c622710106c69699c31fb030d1bf829d4e8f4aaa50f55ac3b28b54773b0807`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 2.0 MB (1954466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1513baeaf9f9576f8b93d8219de7261ba83d0b5cfa5dd1dcedb5be9655a061d9`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1458128d1e555db75f3e321d2567c3161ea13b21cf58a284c6aa30f7407c0ec`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5430e327bbe2a789cdcba9db631882a4b314bbf4ab7889d26edb759b84690846`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c87e01f2d95ccca0541a87bc8aa35d5c415f1adf0b63bb233e27302265ff3`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.5.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:ef3eeaa76efe3728df041a3564633fed4d33fcfe1119249c78713839953517e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185316256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7765681c0f03f57b6e2564b1b8f81405f0b677caac6624a462d7648d5ca3f747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:40:44 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.2.tar.gz.asc crate-5.5.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.2.tar.gz.asc     && tar -xf crate-5.5.2.tar.gz -C /crate --strip-components=1     && rm crate-5.5.2.tar.gz
# Fri, 22 Dec 2023 16:40:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:40:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:40:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:40:49 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:40:49 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:40:50 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:40:50 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:40:50 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:40:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:40:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:11:54.972232 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.2
# Fri, 22 Dec 2023 16:40:50 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:40:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:40:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566aa147c52fb34ae9c2cd58aa1580dc133ad08f5c1819d5fbcdf5458e15223f`  
		Last Modified: Fri, 22 Dec 2023 16:42:55 GMT  
		Size: 115.8 MB (115844512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eaade3584c0c68726c92dbf49e07acdbb278631931d0507afb413ea71e8bb`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 2.0 MB (1954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540d6d74d87b635dadb13114e9e606371a750e5bc2a59acb2e1c1c5ee58ecec0`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d619ab5c9ed042702e77b303f7a2eb4fcfabb0cfa66882234cecc45add74c3b3`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d26d214b8b17bf6941ce9ac961838a1edabd9eb1047c3d650cf5957be21bfad`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779f71414f45a627b954e5644e2d6250fc7e588c571c0287216b619da6058e5e`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:451e22f8481a0313f195daa6e743939d4da1a93a592eb41d527978010449ee0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:eb7847697e1b9ec586a6f3ec8b2a3f103bb21a6fcf8acd74e019a7e3d3c5290b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.9 MB (186868864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265dc46fe158b01f5d18f659ed332368a558c71faa6e5f2c6581d7248d601762`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:28:25 GMT
ADD file:9788b2efafa75575650a53daa65abb265da8eb6383be54f969f94c96c19ad82f in / 
# Tue, 28 Nov 2023 23:28:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Nov 2023 23:48:54 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 17:39:58 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.2.tar.gz.asc crate-5.5.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.2.tar.gz.asc     && tar -xf crate-5.5.2.tar.gz -C /crate --strip-components=1     && rm crate-5.5.2.tar.gz
# Fri, 22 Dec 2023 17:40:00 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 17:40:00 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 17:40:01 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 17:40:01 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 17:40:01 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 17:40:01 GMT
WORKDIR /data
# Fri, 22 Dec 2023 17:40:01 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 17:40:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 17:40:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 17:40:02 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:11:54.972232 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.2
# Fri, 22 Dec 2023 17:40:02 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 17:40:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 17:40:02 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:28130cb29ede9c7eb632516608f6be44c01d736736eb9f03846fb16c819426ae`  
		Last Modified: Tue, 28 Nov 2023 23:29:38 GMT  
		Size: 68.2 MB (68211613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474dd2aa9d062ecbc8a0eb11a10b354dea867214e1deec1655700136f902458e`  
		Last Modified: Tue, 28 Nov 2023 23:51:14 GMT  
		Size: 424.9 KB (424899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe05a660053a74e0a9edb52edc7aafb8031c6b5dd2847ed86f1ecd0c094d8b7f`  
		Last Modified: Fri, 22 Dec 2023 17:42:03 GMT  
		Size: 116.3 MB (116276004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c622710106c69699c31fb030d1bf829d4e8f4aaa50f55ac3b28b54773b0807`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 2.0 MB (1954466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1513baeaf9f9576f8b93d8219de7261ba83d0b5cfa5dd1dcedb5be9655a061d9`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1458128d1e555db75f3e321d2567c3161ea13b21cf58a284c6aa30f7407c0ec`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5430e327bbe2a789cdcba9db631882a4b314bbf4ab7889d26edb759b84690846`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c87e01f2d95ccca0541a87bc8aa35d5c415f1adf0b63bb233e27302265ff3`  
		Last Modified: Fri, 22 Dec 2023 17:41:52 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:ef3eeaa76efe3728df041a3564633fed4d33fcfe1119249c78713839953517e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185316256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7765681c0f03f57b6e2564b1b8f81405f0b677caac6624a462d7648d5ca3f747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 28 Nov 2023 23:42:55 GMT
ADD file:441d5753e358643a6d34ba14749df2f53865a75394abf02aaaf8f8cb75bd98eb in / 
# Tue, 28 Nov 2023 23:42:57 GMT
CMD ["/bin/bash"]
# Wed, 29 Nov 2023 00:16:49 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Fri, 22 Dec 2023 16:40:44 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.2.tar.gz.asc crate-5.5.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.2.tar.gz.asc     && tar -xf crate-5.5.2.tar.gz -C /crate --strip-components=1     && rm crate-5.5.2.tar.gz
# Fri, 22 Dec 2023 16:40:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.1.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.1.asc crash_standalone_0.30.1     && rm -rf "$GNUPGHOME" crash_standalone_0.30.1.asc     && mv crash_standalone_0.30.1 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 22 Dec 2023 16:40:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Dec 2023 16:40:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 22 Dec 2023 16:40:49 GMT
RUN mkdir -p /data/data /data/log
# Fri, 22 Dec 2023 16:40:49 GMT
VOLUME [/data]
# Fri, 22 Dec 2023 16:40:50 GMT
WORKDIR /data
# Fri, 22 Dec 2023 16:40:50 GMT
EXPOSE 4200 4300 5432
# Fri, 22 Dec 2023 16:40:50 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 22 Dec 2023 16:40:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 22 Dec 2023 16:40:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-12-21T21:11:54.972232 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.2
# Fri, 22 Dec 2023 16:40:50 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 22 Dec 2023 16:40:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 22 Dec 2023 16:40:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:c1500036e99b2f702d6379d090f3a4275a6e20d574bd82310d582cb60b2d1cf5`  
		Last Modified: Tue, 28 Nov 2023 23:43:55 GMT  
		Size: 67.1 MB (67090991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c229dddf1130365642b2edf5bbcf90362be62d41571e89dd36c74ef5831ba73f`  
		Last Modified: Wed, 29 Nov 2023 00:19:03 GMT  
		Size: 424.4 KB (424401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566aa147c52fb34ae9c2cd58aa1580dc133ad08f5c1819d5fbcdf5458e15223f`  
		Last Modified: Fri, 22 Dec 2023 16:42:55 GMT  
		Size: 115.8 MB (115844512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eaade3584c0c68726c92dbf49e07acdbb278631931d0507afb413ea71e8bb`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 2.0 MB (1954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540d6d74d87b635dadb13114e9e606371a750e5bc2a59acb2e1c1c5ee58ecec0`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d619ab5c9ed042702e77b303f7a2eb4fcfabb0cfa66882234cecc45add74c3b3`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d26d214b8b17bf6941ce9ac961838a1edabd9eb1047c3d650cf5957be21bfad`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779f71414f45a627b954e5644e2d6250fc7e588c571c0287216b619da6058e5e`  
		Last Modified: Fri, 22 Dec 2023 16:42:46 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
