<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.8`](#crate48)
-	[`crate:4.8.4`](#crate484)
-	[`crate:5.1`](#crate51)
-	[`crate:5.1.4`](#crate514)
-	[`crate:5.2`](#crate52)
-	[`crate:5.2.5`](#crate525)
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

## `crate:5.1`

```console
$ docker pull crate@sha256:4e886a0e751e606b26f54584a37719b9a68fcb28cc847d1c890d6595b4ef2b78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.1` - linux; amd64

```console
$ docker pull crate@sha256:a6fbf5c3362a2382407a66038062774ce5a801fb877f08830b675c40ef146c0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374137395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e7de268aa412ee75cd4a38650f7dd9cf080500cf54a54b4a1ff3af6705d8ba`
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
# Tue, 07 Feb 2023 02:30:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.1.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.1.4.tar.gz.asc crate-5.1.4.tar.gz     && rm -rf "$GNUPGHOME" crate-5.1.4.tar.gz.asc     && tar -xf crate-5.1.4.tar.gz -C /crate --strip-components=1     && rm crate-5.1.4.tar.gz
# Tue, 07 Feb 2023 02:30:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 07 Feb 2023 02:30:25 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 02:30:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 07 Feb 2023 02:30:26 GMT
RUN mkdir -p /data/data /data/log
# Tue, 07 Feb 2023 02:30:26 GMT
VOLUME [/data]
# Tue, 07 Feb 2023 02:30:26 GMT
WORKDIR /data
# Tue, 07 Feb 2023 02:30:26 GMT
EXPOSE 4200 4300 5432
# Tue, 07 Feb 2023 02:30:26 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 07 Feb 2023 02:30:26 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 07 Feb 2023 02:30:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-01T11:51:38.179251 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.1.4
# Tue, 07 Feb 2023 02:30:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 07 Feb 2023 02:30:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:30:27 GMT
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
	-	`sha256:058d69f0b9f069da294c8c8fa7d2f042723e5e3548932cd7f56e0b3300b52d69`  
		Last Modified: Tue, 07 Feb 2023 02:31:03 GMT  
		Size: 219.2 MB (219178229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208da7a8dc8bd96bbc524f06e5a4e8d1563995381d18fa5c175330d33ccc00e`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 1.7 MB (1710774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499754ae1fbf828294712397babe49c2ffb3671a90ef0e7011ec7a38c886c4d4`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701e5b0271c83b7daa100db79d3112c4b763a49dc52bd12ecf3df1289868e72`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f33d26a8afba44a242aef0966df625ad34a1cc88e71e46052ec441c9ada3da`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855ef2f7003b260cb8f7c7c19110870792e2216ef7675eaf6b813633ee9aea2`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.1` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:07ba8158c535cfdc29c57bf5937590ef91212fc4b5431546a12c10d2b164588e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **674.1 MB (674121243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a916cd857b861cb1ddecf5154790180055db6e4d792b198e90fb0adb59f0637a`
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
# Tue, 07 Feb 2023 01:39:47 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.1.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.1.4.tar.gz.asc crate-5.1.4.tar.gz     && rm -rf "$GNUPGHOME" crate-5.1.4.tar.gz.asc     && tar -xf crate-5.1.4.tar.gz -C /crate --strip-components=1     && rm crate-5.1.4.tar.gz
# Tue, 07 Feb 2023 01:39:52 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 07 Feb 2023 01:39:52 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 01:39:52 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 07 Feb 2023 01:39:52 GMT
RUN mkdir -p /data/data /data/log
# Tue, 07 Feb 2023 01:39:52 GMT
VOLUME [/data]
# Tue, 07 Feb 2023 01:39:52 GMT
WORKDIR /data
# Tue, 07 Feb 2023 01:39:53 GMT
EXPOSE 4200 4300 5432
# Tue, 07 Feb 2023 01:39:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 07 Feb 2023 01:39:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 07 Feb 2023 01:39:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-01T11:51:38.179251 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.1.4
# Tue, 07 Feb 2023 01:39:53 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 07 Feb 2023 01:39:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:39:53 GMT
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
	-	`sha256:446682f7e3dd9f925dc4da1b4c9263ce7b153028c1044e327f3063fa3687aac0`  
		Last Modified: Tue, 07 Feb 2023 01:40:31 GMT  
		Size: 218.0 MB (218036808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599cca18e205a5fa36b3392ae26c6e3c403da7d8b5c4534bbd74ff1aa03d5a50`  
		Last Modified: Tue, 07 Feb 2023 01:40:16 GMT  
		Size: 1.7 MB (1710764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fd2c737a55f68c3930ec035c69f3fbd3473bb03e48f7fbb39ccf98f23a5a1c`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d00c39e8815c827746e059be3468eaf450c676f04778d7b7c6014f84d851206`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cee2de362be09a8976cd0782120a39fe4f0f3e248f0b33a7cf9cecadef7743`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900be12b4b1ca0fc4fc115931cd5ab4c332bd3207bfb2356292280a71edacd14`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.1.4`

```console
$ docker pull crate@sha256:4e886a0e751e606b26f54584a37719b9a68fcb28cc847d1c890d6595b4ef2b78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.1.4` - linux; amd64

```console
$ docker pull crate@sha256:a6fbf5c3362a2382407a66038062774ce5a801fb877f08830b675c40ef146c0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374137395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e7de268aa412ee75cd4a38650f7dd9cf080500cf54a54b4a1ff3af6705d8ba`
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
# Tue, 07 Feb 2023 02:30:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.1.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.1.4.tar.gz.asc crate-5.1.4.tar.gz     && rm -rf "$GNUPGHOME" crate-5.1.4.tar.gz.asc     && tar -xf crate-5.1.4.tar.gz -C /crate --strip-components=1     && rm crate-5.1.4.tar.gz
# Tue, 07 Feb 2023 02:30:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 07 Feb 2023 02:30:25 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 02:30:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 07 Feb 2023 02:30:26 GMT
RUN mkdir -p /data/data /data/log
# Tue, 07 Feb 2023 02:30:26 GMT
VOLUME [/data]
# Tue, 07 Feb 2023 02:30:26 GMT
WORKDIR /data
# Tue, 07 Feb 2023 02:30:26 GMT
EXPOSE 4200 4300 5432
# Tue, 07 Feb 2023 02:30:26 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 07 Feb 2023 02:30:26 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 07 Feb 2023 02:30:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-01T11:51:38.179251 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.1.4
# Tue, 07 Feb 2023 02:30:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 07 Feb 2023 02:30:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:30:27 GMT
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
	-	`sha256:058d69f0b9f069da294c8c8fa7d2f042723e5e3548932cd7f56e0b3300b52d69`  
		Last Modified: Tue, 07 Feb 2023 02:31:03 GMT  
		Size: 219.2 MB (219178229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208da7a8dc8bd96bbc524f06e5a4e8d1563995381d18fa5c175330d33ccc00e`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 1.7 MB (1710774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499754ae1fbf828294712397babe49c2ffb3671a90ef0e7011ec7a38c886c4d4`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701e5b0271c83b7daa100db79d3112c4b763a49dc52bd12ecf3df1289868e72`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f33d26a8afba44a242aef0966df625ad34a1cc88e71e46052ec441c9ada3da`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855ef2f7003b260cb8f7c7c19110870792e2216ef7675eaf6b813633ee9aea2`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.1.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:07ba8158c535cfdc29c57bf5937590ef91212fc4b5431546a12c10d2b164588e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **674.1 MB (674121243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a916cd857b861cb1ddecf5154790180055db6e4d792b198e90fb0adb59f0637a`
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
# Tue, 07 Feb 2023 01:39:47 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.1.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.1.4.tar.gz.asc crate-5.1.4.tar.gz     && rm -rf "$GNUPGHOME" crate-5.1.4.tar.gz.asc     && tar -xf crate-5.1.4.tar.gz -C /crate --strip-components=1     && rm crate-5.1.4.tar.gz
# Tue, 07 Feb 2023 01:39:52 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 07 Feb 2023 01:39:52 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 01:39:52 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 07 Feb 2023 01:39:52 GMT
RUN mkdir -p /data/data /data/log
# Tue, 07 Feb 2023 01:39:52 GMT
VOLUME [/data]
# Tue, 07 Feb 2023 01:39:52 GMT
WORKDIR /data
# Tue, 07 Feb 2023 01:39:53 GMT
EXPOSE 4200 4300 5432
# Tue, 07 Feb 2023 01:39:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 07 Feb 2023 01:39:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 07 Feb 2023 01:39:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-01T11:51:38.179251 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.1.4
# Tue, 07 Feb 2023 01:39:53 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 07 Feb 2023 01:39:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:39:53 GMT
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
	-	`sha256:446682f7e3dd9f925dc4da1b4c9263ce7b153028c1044e327f3063fa3687aac0`  
		Last Modified: Tue, 07 Feb 2023 01:40:31 GMT  
		Size: 218.0 MB (218036808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599cca18e205a5fa36b3392ae26c6e3c403da7d8b5c4534bbd74ff1aa03d5a50`  
		Last Modified: Tue, 07 Feb 2023 01:40:16 GMT  
		Size: 1.7 MB (1710764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fd2c737a55f68c3930ec035c69f3fbd3473bb03e48f7fbb39ccf98f23a5a1c`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d00c39e8815c827746e059be3468eaf450c676f04778d7b7c6014f84d851206`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cee2de362be09a8976cd0782120a39fe4f0f3e248f0b33a7cf9cecadef7743`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900be12b4b1ca0fc4fc115931cd5ab4c332bd3207bfb2356292280a71edacd14`  
		Last Modified: Tue, 07 Feb 2023 01:40:15 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2`

```console
$ docker pull crate@sha256:d8b7b78061042082d39825355ceb52fafd211cfe487b79f3d706d5657801e760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2` - linux; amd64

```console
$ docker pull crate@sha256:413d7219a34c4f095f55196b5b0faa8d03a9cfd2832042d86e2b96b12c8508a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305794375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adfbe2eb4f21afbea42f6b2654ee57aed94a11aaceec492cf48ca841d775be1c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 22 Feb 2023 18:20:29 GMT
ADD file:97cfcd4d2e9fb628ab2192a2c99ea93dc2b97c852191d6dda024a33def36ff98 in / 
# Wed, 22 Feb 2023 18:20:30 GMT
CMD ["/bin/bash"]
# Wed, 22 Feb 2023 18:44:20 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip openssl     && yum clean all     && rm -rf /var/cache/yum
# Fri, 03 Mar 2023 19:40:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.3.tar.gz.asc crate-5.2.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.3.tar.gz.asc     && tar -xf crate-5.2.3.tar.gz -C /crate --strip-components=1     && rm crate-5.2.3.tar.gz
# Fri, 03 Mar 2023 19:40:08 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 03 Mar 2023 19:40:08 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 19:40:08 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 03 Mar 2023 19:40:08 GMT
RUN mkdir -p /data/data /data/log
# Fri, 03 Mar 2023 19:40:09 GMT
VOLUME [/data]
# Fri, 03 Mar 2023 19:40:09 GMT
WORKDIR /data
# Fri, 03 Mar 2023 19:40:09 GMT
EXPOSE 4200 4300 5432
# Fri, 03 Mar 2023 19:40:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 03 Mar 2023 19:40:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 03 Mar 2023 19:40:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-23T18:33:34.841271 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.3
# Fri, 03 Mar 2023 19:40:09 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 03 Mar 2023 19:40:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 19:40:09 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:7a76c6018191c79083d136ece0e14591fa547d39614feadfbba0bfc01370169c`  
		Last Modified: Wed, 22 Feb 2023 18:21:49 GMT  
		Size: 69.4 MB (69369008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8567b5795a662eb2f4941e63c1a763d1f770e00ee76cf18582e7a0c333092db6`  
		Last Modified: Wed, 22 Feb 2023 18:45:09 GMT  
		Size: 7.6 MB (7597650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca660350c319b226dd1bc85170d3cf3f060d22264c4776f304456a54873da0e6`  
		Last Modified: Fri, 03 Mar 2023 19:40:49 GMT  
		Size: 227.1 MB (227116490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d728cbde6ec21c5a7dfc0de87313fdbe016c3e9d6a5183bf54b3c5448dae47`  
		Last Modified: Fri, 03 Mar 2023 19:40:31 GMT  
		Size: 1.7 MB (1709346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629842c4fb5c1e7eed693285abe48052a646c7b2c61209c0762335bc5e525e4b`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b8d5c1b4bf3f77d4398de44a6d57350e82a899d9bd70914d90e8b3795c8c9c`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60c58be34dd254b57ef47ade883b5d92f9548f30523e71e1bcd78e858f9019`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b5d04f804c81b4f9d4d0a82e3c5dda83d73989cd4771c0aee928b2a3e1681`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:a3f1eef2ec48b7451a84302b3b17815c8fb5e088bb2a6cc94306f9cf67dba2eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303286728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c171f3082c6e3ba68d073d8c636eb57a8faa9463b178fd3e178a2ded63b0e25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 22 Feb 2023 18:39:41 GMT
ADD file:5cfbd6a23404774b254bbb2adaca41ae6a30adebeba866ac7037d39dce172c2d in / 
# Wed, 22 Feb 2023 18:39:43 GMT
CMD ["/bin/bash"]
# Wed, 22 Feb 2023 20:48:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip openssl     && yum clean all     && rm -rf /var/cache/yum
# Fri, 03 Mar 2023 19:39:43 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.3.tar.gz.asc crate-5.2.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.3.tar.gz.asc     && tar -xf crate-5.2.3.tar.gz -C /crate --strip-components=1     && rm crate-5.2.3.tar.gz
# Fri, 03 Mar 2023 19:39:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 03 Mar 2023 19:39:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 19:39:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 03 Mar 2023 19:39:50 GMT
RUN mkdir -p /data/data /data/log
# Fri, 03 Mar 2023 19:39:50 GMT
VOLUME [/data]
# Fri, 03 Mar 2023 19:39:50 GMT
WORKDIR /data
# Fri, 03 Mar 2023 19:39:50 GMT
EXPOSE 4200 4300 5432
# Fri, 03 Mar 2023 19:39:50 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 03 Mar 2023 19:39:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 03 Mar 2023 19:39:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-23T18:33:34.841271 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.3
# Fri, 03 Mar 2023 19:39:50 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 03 Mar 2023 19:39:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 19:39:51 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:830857804d57387c8e38e13bdb43ca4b64c77c09f220a399a402fab613004669`  
		Last Modified: Wed, 22 Feb 2023 18:41:03 GMT  
		Size: 68.3 MB (68267771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5541b17e3e4c3835ddec68c11f9ed0ded2196e4fef43823262282822351c0ced`  
		Last Modified: Wed, 22 Feb 2023 20:48:55 GMT  
		Size: 7.4 MB (7447934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148b631d6877018228b8eaff44b7e2750e9a4b44c8374c9e041b0492321548a4`  
		Last Modified: Fri, 03 Mar 2023 19:40:27 GMT  
		Size: 225.9 MB (225859797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c27ea7245cb73ab4d24b832a733fcb045ea181cb008ddddb19636b2c81fa166`  
		Last Modified: Fri, 03 Mar 2023 19:40:08 GMT  
		Size: 1.7 MB (1709346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70c9fd8e61815fe32bc507bc624a5a16f502575aa825d74fec96089a2ac4a52`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2dd31449078e1cad593a8edf72d0db44765cd87bf97fa351fba338f2925e34`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef61db7460304198321877e0c86c2f4c1881d015d1020c3077818ef9b607d87b`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8bbf230eb1cc86eb39e9507438c1c1713ad21ee67ecc1ac3c0999514c78e0`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2.5`

**does not exist** (yet?)

## `crate:latest`

```console
$ docker pull crate@sha256:d8b7b78061042082d39825355ceb52fafd211cfe487b79f3d706d5657801e760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:413d7219a34c4f095f55196b5b0faa8d03a9cfd2832042d86e2b96b12c8508a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305794375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adfbe2eb4f21afbea42f6b2654ee57aed94a11aaceec492cf48ca841d775be1c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 22 Feb 2023 18:20:29 GMT
ADD file:97cfcd4d2e9fb628ab2192a2c99ea93dc2b97c852191d6dda024a33def36ff98 in / 
# Wed, 22 Feb 2023 18:20:30 GMT
CMD ["/bin/bash"]
# Wed, 22 Feb 2023 18:44:20 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip openssl     && yum clean all     && rm -rf /var/cache/yum
# Fri, 03 Mar 2023 19:40:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.3.tar.gz.asc crate-5.2.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.3.tar.gz.asc     && tar -xf crate-5.2.3.tar.gz -C /crate --strip-components=1     && rm crate-5.2.3.tar.gz
# Fri, 03 Mar 2023 19:40:08 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 03 Mar 2023 19:40:08 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 19:40:08 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 03 Mar 2023 19:40:08 GMT
RUN mkdir -p /data/data /data/log
# Fri, 03 Mar 2023 19:40:09 GMT
VOLUME [/data]
# Fri, 03 Mar 2023 19:40:09 GMT
WORKDIR /data
# Fri, 03 Mar 2023 19:40:09 GMT
EXPOSE 4200 4300 5432
# Fri, 03 Mar 2023 19:40:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 03 Mar 2023 19:40:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 03 Mar 2023 19:40:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-23T18:33:34.841271 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.3
# Fri, 03 Mar 2023 19:40:09 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 03 Mar 2023 19:40:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 19:40:09 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:7a76c6018191c79083d136ece0e14591fa547d39614feadfbba0bfc01370169c`  
		Last Modified: Wed, 22 Feb 2023 18:21:49 GMT  
		Size: 69.4 MB (69369008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8567b5795a662eb2f4941e63c1a763d1f770e00ee76cf18582e7a0c333092db6`  
		Last Modified: Wed, 22 Feb 2023 18:45:09 GMT  
		Size: 7.6 MB (7597650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca660350c319b226dd1bc85170d3cf3f060d22264c4776f304456a54873da0e6`  
		Last Modified: Fri, 03 Mar 2023 19:40:49 GMT  
		Size: 227.1 MB (227116490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d728cbde6ec21c5a7dfc0de87313fdbe016c3e9d6a5183bf54b3c5448dae47`  
		Last Modified: Fri, 03 Mar 2023 19:40:31 GMT  
		Size: 1.7 MB (1709346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629842c4fb5c1e7eed693285abe48052a646c7b2c61209c0762335bc5e525e4b`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b8d5c1b4bf3f77d4398de44a6d57350e82a899d9bd70914d90e8b3795c8c9c`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60c58be34dd254b57ef47ade883b5d92f9548f30523e71e1bcd78e858f9019`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b5d04f804c81b4f9d4d0a82e3c5dda83d73989cd4771c0aee928b2a3e1681`  
		Last Modified: Fri, 03 Mar 2023 19:40:30 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:a3f1eef2ec48b7451a84302b3b17815c8fb5e088bb2a6cc94306f9cf67dba2eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303286728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c171f3082c6e3ba68d073d8c636eb57a8faa9463b178fd3e178a2ded63b0e25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 22 Feb 2023 18:39:41 GMT
ADD file:5cfbd6a23404774b254bbb2adaca41ae6a30adebeba866ac7037d39dce172c2d in / 
# Wed, 22 Feb 2023 18:39:43 GMT
CMD ["/bin/bash"]
# Wed, 22 Feb 2023 20:48:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip openssl     && yum clean all     && rm -rf /var/cache/yum
# Fri, 03 Mar 2023 19:39:43 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.3.tar.gz.asc crate-5.2.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.3.tar.gz.asc     && tar -xf crate-5.2.3.tar.gz -C /crate --strip-components=1     && rm crate-5.2.3.tar.gz
# Fri, 03 Mar 2023 19:39:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 03 Mar 2023 19:39:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Mar 2023 19:39:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 03 Mar 2023 19:39:50 GMT
RUN mkdir -p /data/data /data/log
# Fri, 03 Mar 2023 19:39:50 GMT
VOLUME [/data]
# Fri, 03 Mar 2023 19:39:50 GMT
WORKDIR /data
# Fri, 03 Mar 2023 19:39:50 GMT
EXPOSE 4200 4300 5432
# Fri, 03 Mar 2023 19:39:50 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 03 Mar 2023 19:39:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 03 Mar 2023 19:39:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-23T18:33:34.841271 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.3
# Fri, 03 Mar 2023 19:39:50 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 03 Mar 2023 19:39:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Mar 2023 19:39:51 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:830857804d57387c8e38e13bdb43ca4b64c77c09f220a399a402fab613004669`  
		Last Modified: Wed, 22 Feb 2023 18:41:03 GMT  
		Size: 68.3 MB (68267771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5541b17e3e4c3835ddec68c11f9ed0ded2196e4fef43823262282822351c0ced`  
		Last Modified: Wed, 22 Feb 2023 20:48:55 GMT  
		Size: 7.4 MB (7447934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148b631d6877018228b8eaff44b7e2750e9a4b44c8374c9e041b0492321548a4`  
		Last Modified: Fri, 03 Mar 2023 19:40:27 GMT  
		Size: 225.9 MB (225859797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c27ea7245cb73ab4d24b832a733fcb045ea181cb008ddddb19636b2c81fa166`  
		Last Modified: Fri, 03 Mar 2023 19:40:08 GMT  
		Size: 1.7 MB (1709346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70c9fd8e61815fe32bc507bc624a5a16f502575aa825d74fec96089a2ac4a52`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2dd31449078e1cad593a8edf72d0db44765cd87bf97fa351fba338f2925e34`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef61db7460304198321877e0c86c2f4c1881d015d1020c3077818ef9b607d87b`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8bbf230eb1cc86eb39e9507438c1c1713ad21ee67ecc1ac3c0999514c78e0`  
		Last Modified: Fri, 03 Mar 2023 19:40:07 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
