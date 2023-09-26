<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.8`](#crate48)
-	[`crate:4.8.4`](#crate484)
-	[`crate:5.2`](#crate52)
-	[`crate:5.2.9`](#crate529)
-	[`crate:5.3`](#crate53)
-	[`crate:5.3.6`](#crate536)
-	[`crate:5.4`](#crate54)
-	[`crate:5.4.3`](#crate543)
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
$ docker pull crate@sha256:f0ec536e945ab08d546c6e93670b66175d452a43e39eb00d04ce72c227101282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2` - linux; amd64

```console
$ docker pull crate@sha256:ac9874a972beb6bf74f97aa9fc92c51ee8a3c017c5fe3e75de4c57049ad795f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.9 MB (304933138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd0e94d23fb55a967281bb1495084c4cd551723c0e4752e845d5804d26a4ca8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:19:42 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 26 Sep 2023 18:19:53 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.9.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.9.tar.gz.asc crate-5.2.9.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.9.tar.gz.asc     && tar -xf crate-5.2.9.tar.gz -C /crate --strip-components=1     && rm crate-5.2.9.tar.gz
# Tue, 26 Sep 2023 18:19:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 26 Sep 2023 18:19:56 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Sep 2023 18:19:56 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 26 Sep 2023 18:19:57 GMT
RUN mkdir -p /data/data /data/log
# Tue, 26 Sep 2023 18:19:57 GMT
VOLUME [/data]
# Tue, 26 Sep 2023 18:19:57 GMT
WORKDIR /data
# Tue, 26 Sep 2023 18:19:57 GMT
EXPOSE 4200 4300 5432
# Tue, 26 Sep 2023 18:19:57 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 26 Sep 2023 18:19:57 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 26 Sep 2023 18:19:57 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-22T11:18:05.424297 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.9
# Tue, 26 Sep 2023 18:19:57 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 26 Sep 2023 18:19:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 26 Sep 2023 18:19:57 GMT
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
	-	`sha256:e5c733671bb8906f934befefbf65e3c0b2e77e06818cfb0b3edf58b7a945a110`  
		Last Modified: Tue, 26 Sep 2023 18:20:34 GMT  
		Size: 227.1 MB (227117649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ad7c8b4ee2ff37af55b7d2c7264e4a540ee25738a93706d6f4721bbb79186b`  
		Last Modified: Tue, 26 Sep 2023 18:20:15 GMT  
		Size: 1.9 MB (1931732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7a2419c1b0f5b5e764f3724a3219f809c93d398241b7cb5a418f22cbe7357e`  
		Last Modified: Tue, 26 Sep 2023 18:20:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8995fab9d778cf4d064a2183dd93ee620d784c8f96777aca72e0b7cecd3daf38`  
		Last Modified: Tue, 26 Sep 2023 18:20:15 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd542d89d348e6e51cafb4a3f294a7d7338895ae76770371aa596522ef50458`  
		Last Modified: Tue, 26 Sep 2023 18:20:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb7e29910c70f881125e57153b0243810eec8157869d8be324116d9e6173c75`  
		Last Modified: Tue, 26 Sep 2023 18:20:14 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:159013eab641d086ee73f96945abf19fbd35b1f2659ba7ebefd5e486f553fa69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302429418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18e06294092825b2f19f27c9aa95a3e12056b0983fe46cd60e1aa3c526749757`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:39:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 26 Sep 2023 18:39:49 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.9.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.9.tar.gz.asc crate-5.2.9.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.9.tar.gz.asc     && tar -xf crate-5.2.9.tar.gz -C /crate --strip-components=1     && rm crate-5.2.9.tar.gz
# Tue, 26 Sep 2023 18:39:52 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 26 Sep 2023 18:39:53 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Sep 2023 18:39:53 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 26 Sep 2023 18:39:53 GMT
RUN mkdir -p /data/data /data/log
# Tue, 26 Sep 2023 18:39:53 GMT
VOLUME [/data]
# Tue, 26 Sep 2023 18:39:53 GMT
WORKDIR /data
# Tue, 26 Sep 2023 18:39:53 GMT
EXPOSE 4200 4300 5432
# Tue, 26 Sep 2023 18:39:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 26 Sep 2023 18:39:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 26 Sep 2023 18:39:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-22T11:18:05.424297 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.9
# Tue, 26 Sep 2023 18:39:54 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 26 Sep 2023 18:39:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 26 Sep 2023 18:39:54 GMT
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
	-	`sha256:93338846159796e3c814327e9a7555d0a2aaa1a1dfa932f63a1273d7ee764adc`  
		Last Modified: Tue, 26 Sep 2023 18:40:30 GMT  
		Size: 225.9 MB (225862152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42fbc2444985ba953022c97ff44632fd55694d2f347c8cee10384ec44084695`  
		Last Modified: Tue, 26 Sep 2023 18:40:14 GMT  
		Size: 1.9 MB (1931737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00983d2304d04174e2152f7f97616cfabf090c1a4137a5d3d8d425d1c382a89e`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf997b1caf55a7920e8fdcaa842fe27b86bdb81924c4751706139213d6530d`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744b5e4375954ac94baf202fd20e3203a6bdf025900f529a2df8eaf36c70d5c7`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ab13f18326ed6b494ec26c7cd958f9bc8d0fbaed97961440165b00e8bc51c4`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2.9`

```console
$ docker pull crate@sha256:f0ec536e945ab08d546c6e93670b66175d452a43e39eb00d04ce72c227101282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2.9` - linux; amd64

```console
$ docker pull crate@sha256:ac9874a972beb6bf74f97aa9fc92c51ee8a3c017c5fe3e75de4c57049ad795f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.9 MB (304933138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd0e94d23fb55a967281bb1495084c4cd551723c0e4752e845d5804d26a4ca8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:19:42 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 26 Sep 2023 18:19:53 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.9.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.9.tar.gz.asc crate-5.2.9.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.9.tar.gz.asc     && tar -xf crate-5.2.9.tar.gz -C /crate --strip-components=1     && rm crate-5.2.9.tar.gz
# Tue, 26 Sep 2023 18:19:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 26 Sep 2023 18:19:56 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Sep 2023 18:19:56 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 26 Sep 2023 18:19:57 GMT
RUN mkdir -p /data/data /data/log
# Tue, 26 Sep 2023 18:19:57 GMT
VOLUME [/data]
# Tue, 26 Sep 2023 18:19:57 GMT
WORKDIR /data
# Tue, 26 Sep 2023 18:19:57 GMT
EXPOSE 4200 4300 5432
# Tue, 26 Sep 2023 18:19:57 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 26 Sep 2023 18:19:57 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 26 Sep 2023 18:19:57 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-22T11:18:05.424297 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.9
# Tue, 26 Sep 2023 18:19:57 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 26 Sep 2023 18:19:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 26 Sep 2023 18:19:57 GMT
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
	-	`sha256:e5c733671bb8906f934befefbf65e3c0b2e77e06818cfb0b3edf58b7a945a110`  
		Last Modified: Tue, 26 Sep 2023 18:20:34 GMT  
		Size: 227.1 MB (227117649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ad7c8b4ee2ff37af55b7d2c7264e4a540ee25738a93706d6f4721bbb79186b`  
		Last Modified: Tue, 26 Sep 2023 18:20:15 GMT  
		Size: 1.9 MB (1931732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7a2419c1b0f5b5e764f3724a3219f809c93d398241b7cb5a418f22cbe7357e`  
		Last Modified: Tue, 26 Sep 2023 18:20:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8995fab9d778cf4d064a2183dd93ee620d784c8f96777aca72e0b7cecd3daf38`  
		Last Modified: Tue, 26 Sep 2023 18:20:15 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd542d89d348e6e51cafb4a3f294a7d7338895ae76770371aa596522ef50458`  
		Last Modified: Tue, 26 Sep 2023 18:20:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb7e29910c70f881125e57153b0243810eec8157869d8be324116d9e6173c75`  
		Last Modified: Tue, 26 Sep 2023 18:20:14 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2.9` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:159013eab641d086ee73f96945abf19fbd35b1f2659ba7ebefd5e486f553fa69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302429418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18e06294092825b2f19f27c9aa95a3e12056b0983fe46cd60e1aa3c526749757`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 26 Sep 2023 18:39:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 26 Sep 2023 18:39:49 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.9.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.9.tar.gz.asc crate-5.2.9.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.9.tar.gz.asc     && tar -xf crate-5.2.9.tar.gz -C /crate --strip-components=1     && rm crate-5.2.9.tar.gz
# Tue, 26 Sep 2023 18:39:52 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 26 Sep 2023 18:39:53 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 26 Sep 2023 18:39:53 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 26 Sep 2023 18:39:53 GMT
RUN mkdir -p /data/data /data/log
# Tue, 26 Sep 2023 18:39:53 GMT
VOLUME [/data]
# Tue, 26 Sep 2023 18:39:53 GMT
WORKDIR /data
# Tue, 26 Sep 2023 18:39:53 GMT
EXPOSE 4200 4300 5432
# Tue, 26 Sep 2023 18:39:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 26 Sep 2023 18:39:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 26 Sep 2023 18:39:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-22T11:18:05.424297 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.9
# Tue, 26 Sep 2023 18:39:54 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 26 Sep 2023 18:39:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 26 Sep 2023 18:39:54 GMT
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
	-	`sha256:93338846159796e3c814327e9a7555d0a2aaa1a1dfa932f63a1273d7ee764adc`  
		Last Modified: Tue, 26 Sep 2023 18:40:30 GMT  
		Size: 225.9 MB (225862152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42fbc2444985ba953022c97ff44632fd55694d2f347c8cee10384ec44084695`  
		Last Modified: Tue, 26 Sep 2023 18:40:14 GMT  
		Size: 1.9 MB (1931737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00983d2304d04174e2152f7f97616cfabf090c1a4137a5d3d8d425d1c382a89e`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf997b1caf55a7920e8fdcaa842fe27b86bdb81924c4751706139213d6530d`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744b5e4375954ac94baf202fd20e3203a6bdf025900f529a2df8eaf36c70d5c7`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ab13f18326ed6b494ec26c7cd958f9bc8d0fbaed97961440165b00e8bc51c4`  
		Last Modified: Tue, 26 Sep 2023 18:40:13 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3`

```console
$ docker pull crate@sha256:4b50545f0f1c7394c63a0d1cbbd63fe9c1a88655fb7908c70edc797533207154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3` - linux; amd64

```console
$ docker pull crate@sha256:8f625b20dd28a0187e885394e3d83e6fda8b501c3abca428ec6c5b8bf47067bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297907385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0cd5a6d1b574f7de7ad0fa6217c2d64918c53b0ec815ff4635a559537385f4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 14 Aug 2023 22:44:21 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.6.tar.gz.asc crate-5.3.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.6.tar.gz.asc     && tar -xf crate-5.3.6.tar.gz -C /crate --strip-components=1     && rm crate-5.3.6.tar.gz
# Mon, 14 Aug 2023 22:44:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Aug 2023 22:44:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 22:44:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Aug 2023 22:44:24 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Aug 2023 22:44:24 GMT
VOLUME [/data]
# Mon, 14 Aug 2023 22:44:24 GMT
WORKDIR /data
# Mon, 14 Aug 2023 22:44:24 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Aug 2023 22:44:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Aug 2023 22:44:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Aug 2023 22:44:24 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-08-11T10:18:11.381732 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.6
# Mon, 14 Aug 2023 22:44:25 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Aug 2023 22:44:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Aug 2023 22:44:25 GMT
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
	-	`sha256:232e327f7b094b6ca812bd8f463db0bcf39505eec82e345fbeab7661ab8e07f9`  
		Last Modified: Mon, 14 Aug 2023 22:45:28 GMT  
		Size: 227.3 MB (227333873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea426959c1f8c582fea0d3efb142b2ba3ffc78a94954b80bc5d921abfd4f49ef`  
		Last Modified: Mon, 14 Aug 2023 22:45:11 GMT  
		Size: 1.9 MB (1931732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711dbae18ddca6950df6df3693af0bb4126df1a459bd41b8edef5a0c00e9c272`  
		Last Modified: Mon, 14 Aug 2023 22:45:10 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aab77ce495705b10febe9ff7052fe1eb1bf08fafa96dd0207a4bb8b4c86163`  
		Last Modified: Mon, 14 Aug 2023 22:45:11 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730426185f2cd66fd5fa148ce82462c1330bc8f893fb7c60a5b57ae6375163d`  
		Last Modified: Mon, 14 Aug 2023 22:45:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8587d895e596c3bc6cd7eb30b5fd9d6ff572ed9c1a9360a2be16fc7f2476da7b`  
		Last Modified: Mon, 14 Aug 2023 22:45:10 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8d4940ec51fa6b79473441d10b0a454fb1f07847dffd2f75f512e5b08ab993cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295562750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7727e8acb24ffa124f304bc7008bd9787f9495b7397cd419665f5616a4d516e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 14 Aug 2023 21:19:13 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.6.tar.gz.asc crate-5.3.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.6.tar.gz.asc     && tar -xf crate-5.3.6.tar.gz -C /crate --strip-components=1     && rm crate-5.3.6.tar.gz
# Mon, 14 Aug 2023 21:19:17 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Aug 2023 21:19:17 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 21:19:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Aug 2023 21:19:17 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Aug 2023 21:19:18 GMT
VOLUME [/data]
# Mon, 14 Aug 2023 21:19:18 GMT
WORKDIR /data
# Mon, 14 Aug 2023 21:19:18 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Aug 2023 21:19:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Aug 2023 21:19:18 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Aug 2023 21:19:18 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-08-11T10:18:11.381732 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.6
# Mon, 14 Aug 2023 21:19:18 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Aug 2023 21:19:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Aug 2023 21:19:18 GMT
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
	-	`sha256:eac953fde019019eb9b7d4f0afcf84210d8becdd3a7f401cd180dfa872747039`  
		Last Modified: Mon, 14 Aug 2023 21:20:20 GMT  
		Size: 226.1 MB (226078721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39367bb71f0f6d7f68db6ad7c5068517c831594cdb4a76dfa422376941a505b3`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 1.9 MB (1931733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e429efcebab5bc32a6da9e8ef490f774773bff5225fd438f6824dd691ee40036`  
		Last Modified: Mon, 14 Aug 2023 21:20:06 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a1d7082a15808bff17bf195c9519a978fe508b0ffbaab704ebe9948838166c`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9de12b29da1448caa3ffeed210abed57b89daffbad3a42401853b5abf9afe2`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a7e2c100bdfd4152340fe0d8b292ac0fd9560df89fe9ef83e32c8f41a9b374`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3.6`

```console
$ docker pull crate@sha256:4b50545f0f1c7394c63a0d1cbbd63fe9c1a88655fb7908c70edc797533207154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3.6` - linux; amd64

```console
$ docker pull crate@sha256:8f625b20dd28a0187e885394e3d83e6fda8b501c3abca428ec6c5b8bf47067bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297907385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0cd5a6d1b574f7de7ad0fa6217c2d64918c53b0ec815ff4635a559537385f4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 14 Aug 2023 22:44:21 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.6.tar.gz.asc crate-5.3.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.6.tar.gz.asc     && tar -xf crate-5.3.6.tar.gz -C /crate --strip-components=1     && rm crate-5.3.6.tar.gz
# Mon, 14 Aug 2023 22:44:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Aug 2023 22:44:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 22:44:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Aug 2023 22:44:24 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Aug 2023 22:44:24 GMT
VOLUME [/data]
# Mon, 14 Aug 2023 22:44:24 GMT
WORKDIR /data
# Mon, 14 Aug 2023 22:44:24 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Aug 2023 22:44:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Aug 2023 22:44:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Aug 2023 22:44:24 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-08-11T10:18:11.381732 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.6
# Mon, 14 Aug 2023 22:44:25 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Aug 2023 22:44:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Aug 2023 22:44:25 GMT
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
	-	`sha256:232e327f7b094b6ca812bd8f463db0bcf39505eec82e345fbeab7661ab8e07f9`  
		Last Modified: Mon, 14 Aug 2023 22:45:28 GMT  
		Size: 227.3 MB (227333873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea426959c1f8c582fea0d3efb142b2ba3ffc78a94954b80bc5d921abfd4f49ef`  
		Last Modified: Mon, 14 Aug 2023 22:45:11 GMT  
		Size: 1.9 MB (1931732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711dbae18ddca6950df6df3693af0bb4126df1a459bd41b8edef5a0c00e9c272`  
		Last Modified: Mon, 14 Aug 2023 22:45:10 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aab77ce495705b10febe9ff7052fe1eb1bf08fafa96dd0207a4bb8b4c86163`  
		Last Modified: Mon, 14 Aug 2023 22:45:11 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730426185f2cd66fd5fa148ce82462c1330bc8f893fb7c60a5b57ae6375163d`  
		Last Modified: Mon, 14 Aug 2023 22:45:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8587d895e596c3bc6cd7eb30b5fd9d6ff572ed9c1a9360a2be16fc7f2476da7b`  
		Last Modified: Mon, 14 Aug 2023 22:45:10 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3.6` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8d4940ec51fa6b79473441d10b0a454fb1f07847dffd2f75f512e5b08ab993cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295562750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7727e8acb24ffa124f304bc7008bd9787f9495b7397cd419665f5616a4d516e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 14 Aug 2023 21:19:13 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.6.tar.gz.asc crate-5.3.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.6.tar.gz.asc     && tar -xf crate-5.3.6.tar.gz -C /crate --strip-components=1     && rm crate-5.3.6.tar.gz
# Mon, 14 Aug 2023 21:19:17 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 14 Aug 2023 21:19:17 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 21:19:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 14 Aug 2023 21:19:17 GMT
RUN mkdir -p /data/data /data/log
# Mon, 14 Aug 2023 21:19:18 GMT
VOLUME [/data]
# Mon, 14 Aug 2023 21:19:18 GMT
WORKDIR /data
# Mon, 14 Aug 2023 21:19:18 GMT
EXPOSE 4200 4300 5432
# Mon, 14 Aug 2023 21:19:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 14 Aug 2023 21:19:18 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 14 Aug 2023 21:19:18 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-08-11T10:18:11.381732 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.6
# Mon, 14 Aug 2023 21:19:18 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 14 Aug 2023 21:19:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 14 Aug 2023 21:19:18 GMT
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
	-	`sha256:eac953fde019019eb9b7d4f0afcf84210d8becdd3a7f401cd180dfa872747039`  
		Last Modified: Mon, 14 Aug 2023 21:20:20 GMT  
		Size: 226.1 MB (226078721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39367bb71f0f6d7f68db6ad7c5068517c831594cdb4a76dfa422376941a505b3`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 1.9 MB (1931733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e429efcebab5bc32a6da9e8ef490f774773bff5225fd438f6824dd691ee40036`  
		Last Modified: Mon, 14 Aug 2023 21:20:06 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a1d7082a15808bff17bf195c9519a978fe508b0ffbaab704ebe9948838166c`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9de12b29da1448caa3ffeed210abed57b89daffbad3a42401853b5abf9afe2`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a7e2c100bdfd4152340fe0d8b292ac0fd9560df89fe9ef83e32c8f41a9b374`  
		Last Modified: Mon, 14 Aug 2023 21:20:05 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.4`

```console
$ docker pull crate@sha256:08118fa7743662918bc87383ca1a72a761de1a56f93ea12ec2a970dd74f52a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.4` - linux; amd64

```console
$ docker pull crate@sha256:cbf5a06bc836f821db6200b3ba39039ae5693d1860399c534e6b42827a75271c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300133319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd5365c1c82aad542e9d2fe564cd19c2d1b6e88945a7c3f3bd3f328956a8ba6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 11 Sep 2023 19:24:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.3.tar.gz.asc crate-5.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.3.tar.gz.asc     && tar -xf crate-5.4.3.tar.gz -C /crate --strip-components=1     && rm crate-5.4.3.tar.gz
# Mon, 11 Sep 2023 19:24:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Sep 2023 19:24:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Sep 2023 19:24:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Sep 2023 19:24:27 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Sep 2023 19:24:27 GMT
VOLUME [/data]
# Mon, 11 Sep 2023 19:24:27 GMT
WORKDIR /data
# Mon, 11 Sep 2023 19:24:27 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Sep 2023 19:24:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Sep 2023 19:24:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Sep 2023 19:24:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-05T15:56:26.062030 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.3
# Mon, 11 Sep 2023 19:24:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Sep 2023 19:24:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Sep 2023 19:24:27 GMT
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
	-	`sha256:00496b7b747ea96f7c25e3624e25c56e90ffda85c16dbfc10c125202bbd06ab7`  
		Last Modified: Mon, 11 Sep 2023 19:25:04 GMT  
		Size: 229.6 MB (229559819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fed53f6f9533371c5f63d2d143db1776a93a8105711db5d6f14d436ca7f362e`  
		Last Modified: Mon, 11 Sep 2023 19:24:46 GMT  
		Size: 1.9 MB (1931725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73d06d5ba60a2d480a27f8e38cce410abd1bd9391eeabfb35b7962c74464ec`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9bc0b39fa0b55dc07d3d0868762a62b0f8c847d372c2a9cf77d87f0ab3125`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c2793b02829e9d21c5b15d932581b09870ef4db516705497477ca9aaa09a4`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bc4bc57ab4b41cf1cfcc6a8af335d90043cceac2c2f8b5cd5b0aabe6b8fe34`  
		Last Modified: Mon, 11 Sep 2023 19:24:46 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:87273c51646602a1b1583db306aecf2e6ad289732ccb3ecee480cbd0ba4d43ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297368509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368a4589387d261f52b3e4c06898c51e171a322f2aa8107545cee9c8da4e9260`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 11 Sep 2023 19:11:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.3.tar.gz.asc crate-5.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.3.tar.gz.asc     && tar -xf crate-5.4.3.tar.gz -C /crate --strip-components=1     && rm crate-5.4.3.tar.gz
# Mon, 11 Sep 2023 19:11:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Sep 2023 19:11:11 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Sep 2023 19:11:11 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Sep 2023 19:11:12 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Sep 2023 19:11:12 GMT
VOLUME [/data]
# Mon, 11 Sep 2023 19:11:12 GMT
WORKDIR /data
# Mon, 11 Sep 2023 19:11:12 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Sep 2023 19:11:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Sep 2023 19:11:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Sep 2023 19:11:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-05T15:56:26.062030 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.3
# Mon, 11 Sep 2023 19:11:12 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Sep 2023 19:11:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Sep 2023 19:11:13 GMT
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
	-	`sha256:f2621206c57c0c0098ad398821ee709e36cebfe123953f5597f1d7b402c6e5d4`  
		Last Modified: Mon, 11 Sep 2023 19:11:43 GMT  
		Size: 227.9 MB (227884477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9950269ca474d44b1776dead40b550798d30b495cd636ed7bb75c59960c52cb`  
		Last Modified: Mon, 11 Sep 2023 19:11:28 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74b6740d8b25c3d34a98692158f63ddd208579ba973fd0b2566ffcede32f219`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e9f5acae4f43a5830cdbac74dc110f38204780a8c57371c0aca42acaab2873`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe110aa0c4380d61573cfd39532fd45fcbac5169185decc032a0d498ba4a77`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee7e5b9253169e15c80ceb95a83c824b0ad56f6553b9a6f4bfccf68522aa99`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.4.3`

```console
$ docker pull crate@sha256:08118fa7743662918bc87383ca1a72a761de1a56f93ea12ec2a970dd74f52a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.4.3` - linux; amd64

```console
$ docker pull crate@sha256:cbf5a06bc836f821db6200b3ba39039ae5693d1860399c534e6b42827a75271c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300133319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd5365c1c82aad542e9d2fe564cd19c2d1b6e88945a7c3f3bd3f328956a8ba6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 11 Sep 2023 19:24:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.3.tar.gz.asc crate-5.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.3.tar.gz.asc     && tar -xf crate-5.4.3.tar.gz -C /crate --strip-components=1     && rm crate-5.4.3.tar.gz
# Mon, 11 Sep 2023 19:24:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Sep 2023 19:24:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Sep 2023 19:24:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Sep 2023 19:24:27 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Sep 2023 19:24:27 GMT
VOLUME [/data]
# Mon, 11 Sep 2023 19:24:27 GMT
WORKDIR /data
# Mon, 11 Sep 2023 19:24:27 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Sep 2023 19:24:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Sep 2023 19:24:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Sep 2023 19:24:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-05T15:56:26.062030 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.3
# Mon, 11 Sep 2023 19:24:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Sep 2023 19:24:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Sep 2023 19:24:27 GMT
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
	-	`sha256:00496b7b747ea96f7c25e3624e25c56e90ffda85c16dbfc10c125202bbd06ab7`  
		Last Modified: Mon, 11 Sep 2023 19:25:04 GMT  
		Size: 229.6 MB (229559819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fed53f6f9533371c5f63d2d143db1776a93a8105711db5d6f14d436ca7f362e`  
		Last Modified: Mon, 11 Sep 2023 19:24:46 GMT  
		Size: 1.9 MB (1931725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73d06d5ba60a2d480a27f8e38cce410abd1bd9391eeabfb35b7962c74464ec`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9bc0b39fa0b55dc07d3d0868762a62b0f8c847d372c2a9cf77d87f0ab3125`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c2793b02829e9d21c5b15d932581b09870ef4db516705497477ca9aaa09a4`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bc4bc57ab4b41cf1cfcc6a8af335d90043cceac2c2f8b5cd5b0aabe6b8fe34`  
		Last Modified: Mon, 11 Sep 2023 19:24:46 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.4.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:87273c51646602a1b1583db306aecf2e6ad289732ccb3ecee480cbd0ba4d43ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297368509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368a4589387d261f52b3e4c06898c51e171a322f2aa8107545cee9c8da4e9260`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 11 Sep 2023 19:11:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.3.tar.gz.asc crate-5.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.3.tar.gz.asc     && tar -xf crate-5.4.3.tar.gz -C /crate --strip-components=1     && rm crate-5.4.3.tar.gz
# Mon, 11 Sep 2023 19:11:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Sep 2023 19:11:11 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Sep 2023 19:11:11 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Sep 2023 19:11:12 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Sep 2023 19:11:12 GMT
VOLUME [/data]
# Mon, 11 Sep 2023 19:11:12 GMT
WORKDIR /data
# Mon, 11 Sep 2023 19:11:12 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Sep 2023 19:11:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Sep 2023 19:11:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Sep 2023 19:11:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-05T15:56:26.062030 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.3
# Mon, 11 Sep 2023 19:11:12 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Sep 2023 19:11:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Sep 2023 19:11:13 GMT
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
	-	`sha256:f2621206c57c0c0098ad398821ee709e36cebfe123953f5597f1d7b402c6e5d4`  
		Last Modified: Mon, 11 Sep 2023 19:11:43 GMT  
		Size: 227.9 MB (227884477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9950269ca474d44b1776dead40b550798d30b495cd636ed7bb75c59960c52cb`  
		Last Modified: Mon, 11 Sep 2023 19:11:28 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74b6740d8b25c3d34a98692158f63ddd208579ba973fd0b2566ffcede32f219`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e9f5acae4f43a5830cdbac74dc110f38204780a8c57371c0aca42acaab2873`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe110aa0c4380d61573cfd39532fd45fcbac5169185decc032a0d498ba4a77`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee7e5b9253169e15c80ceb95a83c824b0ad56f6553b9a6f4bfccf68522aa99`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:08118fa7743662918bc87383ca1a72a761de1a56f93ea12ec2a970dd74f52a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:cbf5a06bc836f821db6200b3ba39039ae5693d1860399c534e6b42827a75271c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.1 MB (300133319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd5365c1c82aad542e9d2fe564cd19c2d1b6e88945a7c3f3bd3f328956a8ba6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:20:21 GMT
ADD file:f1f574c0238642ba50927632ce79b8686be2da6793b9aa968b9556f567dc3437 in / 
# Tue, 18 Jul 2023 19:20:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:26:46 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 11 Sep 2023 19:24:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.3.tar.gz.asc crate-5.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.3.tar.gz.asc     && tar -xf crate-5.4.3.tar.gz -C /crate --strip-components=1     && rm crate-5.4.3.tar.gz
# Mon, 11 Sep 2023 19:24:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Sep 2023 19:24:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Sep 2023 19:24:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Sep 2023 19:24:27 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Sep 2023 19:24:27 GMT
VOLUME [/data]
# Mon, 11 Sep 2023 19:24:27 GMT
WORKDIR /data
# Mon, 11 Sep 2023 19:24:27 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Sep 2023 19:24:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Sep 2023 19:24:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Sep 2023 19:24:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-05T15:56:26.062030 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.3
# Mon, 11 Sep 2023 19:24:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Sep 2023 19:24:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Sep 2023 19:24:27 GMT
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
	-	`sha256:00496b7b747ea96f7c25e3624e25c56e90ffda85c16dbfc10c125202bbd06ab7`  
		Last Modified: Mon, 11 Sep 2023 19:25:04 GMT  
		Size: 229.6 MB (229559819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fed53f6f9533371c5f63d2d143db1776a93a8105711db5d6f14d436ca7f362e`  
		Last Modified: Mon, 11 Sep 2023 19:24:46 GMT  
		Size: 1.9 MB (1931725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73d06d5ba60a2d480a27f8e38cce410abd1bd9391eeabfb35b7962c74464ec`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9bc0b39fa0b55dc07d3d0868762a62b0f8c847d372c2a9cf77d87f0ab3125`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c2793b02829e9d21c5b15d932581b09870ef4db516705497477ca9aaa09a4`  
		Last Modified: Mon, 11 Sep 2023 19:24:45 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bc4bc57ab4b41cf1cfcc6a8af335d90043cceac2c2f8b5cd5b0aabe6b8fe34`  
		Last Modified: Mon, 11 Sep 2023 19:24:46 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:87273c51646602a1b1583db306aecf2e6ad289732ccb3ecee480cbd0ba4d43ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297368509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368a4589387d261f52b3e4c06898c51e171a322f2aa8107545cee9c8da4e9260`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Mon, 11 Sep 2023 19:11:05 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.4.3.tar.gz.asc crate-5.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-5.4.3.tar.gz.asc     && tar -xf crate-5.4.3.tar.gz -C /crate --strip-components=1     && rm crate-5.4.3.tar.gz
# Mon, 11 Sep 2023 19:11:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Sep 2023 19:11:11 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Sep 2023 19:11:11 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Sep 2023 19:11:12 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Sep 2023 19:11:12 GMT
VOLUME [/data]
# Mon, 11 Sep 2023 19:11:12 GMT
WORKDIR /data
# Mon, 11 Sep 2023 19:11:12 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Sep 2023 19:11:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Sep 2023 19:11:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Sep 2023 19:11:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-09-05T15:56:26.062030 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.4.3
# Mon, 11 Sep 2023 19:11:12 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Sep 2023 19:11:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Sep 2023 19:11:13 GMT
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
	-	`sha256:f2621206c57c0c0098ad398821ee709e36cebfe123953f5597f1d7b402c6e5d4`  
		Last Modified: Mon, 11 Sep 2023 19:11:43 GMT  
		Size: 227.9 MB (227884477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9950269ca474d44b1776dead40b550798d30b495cd636ed7bb75c59960c52cb`  
		Last Modified: Mon, 11 Sep 2023 19:11:28 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74b6740d8b25c3d34a98692158f63ddd208579ba973fd0b2566ffcede32f219`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e9f5acae4f43a5830cdbac74dc110f38204780a8c57371c0aca42acaab2873`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe110aa0c4380d61573cfd39532fd45fcbac5169185decc032a0d498ba4a77`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee7e5b9253169e15c80ceb95a83c824b0ad56f6553b9a6f4bfccf68522aa99`  
		Last Modified: Mon, 11 Sep 2023 19:11:27 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
