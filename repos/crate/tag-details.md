<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.8`](#crate48)
-	[`crate:4.8.4`](#crate484)
-	[`crate:5.2`](#crate52)
-	[`crate:5.2.6`](#crate526)
-	[`crate:5.3`](#crate53)
-	[`crate:5.3.0`](#crate530)
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
$ docker pull crate@sha256:c7a28d3cb589ce4bde2f074e14267f6699573c2a1ad7039cd0034ad732bfa8ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2` - linux; amd64

```console
$ docker pull crate@sha256:7a1367b86c5a7bd88195b1ddcda0402cfcd8448373506f46da74ab8fb341bfb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (305958858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f59bd1354757ce19854ee89ab40ea186080b1fdfe0168ad02d1a38f43b90a0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 19:19:48 GMT
ADD file:9022dcd506469f7fa13db0072d1e4ed93f0ddf853bdd9ff02efc8d5a0345bb78 in / 
# Tue, 11 Apr 2023 19:19:49 GMT
CMD ["/bin/bash"]
# Tue, 11 Apr 2023 19:36:50 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Wed, 12 Apr 2023 23:35:15 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.6.tar.gz.asc crate-5.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.6.tar.gz.asc     && tar -xf crate-5.2.6.tar.gz -C /crate --strip-components=1     && rm crate-5.2.6.tar.gz
# Wed, 12 Apr 2023 23:35:18 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 12 Apr 2023 23:35:18 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 23:35:18 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 12 Apr 2023 23:35:18 GMT
RUN mkdir -p /data/data /data/log
# Wed, 12 Apr 2023 23:35:18 GMT
VOLUME [/data]
# Wed, 12 Apr 2023 23:35:18 GMT
WORKDIR /data
# Wed, 12 Apr 2023 23:35:19 GMT
EXPOSE 4200 4300 5432
# Wed, 12 Apr 2023 23:35:19 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 12 Apr 2023 23:35:19 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 12 Apr 2023 23:35:19 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T08:45:48.121205 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.6
# Wed, 12 Apr 2023 23:35:19 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 12 Apr 2023 23:35:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 23:35:19 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:349bb8f337e406f9e6bd67c41b36a6481834ff3cf177d4eaa707dd54d730be7b`  
		Last Modified: Tue, 11 Apr 2023 19:21:00 GMT  
		Size: 69.4 MB (69379392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cb21b908980a44e421950e4143abc076d4fc74d81e34760821625dcda884fd`  
		Last Modified: Tue, 11 Apr 2023 19:37:39 GMT  
		Size: 7.6 MB (7603753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4664ae7d4ff7f3357d521f3e580038531ebd9ffe7a4f1993ed34e2ee872614`  
		Last Modified: Wed, 12 Apr 2023 23:35:49 GMT  
		Size: 227.1 MB (227116710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88637feddd69bcc3efa914790828ae93a2efe88b4bd9b31e94570581cb7ccd9`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 1.9 MB (1857123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fcb6338989fb6c33eb9704c6779197c9546c6c0ce91c3fb0a3e6994e4038b1`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd0f16083079ebd52814d2e1cca587d933701140bfdce0b201825c86a0839ab`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5957daf1cc916da90886881ba1fec705a3b8b6a6f49b02e03cbd45e7bbb2e20b`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee72a24c17b1bd55b91d33875e1d55d17dbca697eb64406f1c2c8384b06718b1`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:b2cd329fc48c2ff5445d4560ae947564420fc55db37e528357365698310c124f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303426631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cce886f489a0b26e0a0a546c2daecb3ebed543c6c5dcc66adf22d84b4b058cf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 20:06:33 GMT
ADD file:389251b1d16989bef7dd304f924df38271d5e1140aca5e6a76aca2a98db3914b in / 
# Tue, 11 Apr 2023 20:06:35 GMT
CMD ["/bin/bash"]
# Tue, 11 Apr 2023 20:23:16 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Wed, 12 Apr 2023 19:24:30 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.6.tar.gz.asc crate-5.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.6.tar.gz.asc     && tar -xf crate-5.2.6.tar.gz -C /crate --strip-components=1     && rm crate-5.2.6.tar.gz
# Wed, 12 Apr 2023 19:24:34 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 12 Apr 2023 19:24:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 19:24:35 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 12 Apr 2023 19:24:35 GMT
RUN mkdir -p /data/data /data/log
# Wed, 12 Apr 2023 19:24:35 GMT
VOLUME [/data]
# Wed, 12 Apr 2023 19:24:35 GMT
WORKDIR /data
# Wed, 12 Apr 2023 19:24:35 GMT
EXPOSE 4200 4300 5432
# Wed, 12 Apr 2023 19:24:35 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 12 Apr 2023 19:24:36 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 12 Apr 2023 19:24:36 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T08:45:48.121205 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.6
# Wed, 12 Apr 2023 19:24:36 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 12 Apr 2023 19:24:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 19:24:36 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:8bdbb90acb62176a24ad70eb522992bed0fbe2c7a53633cc96327b2ec7fa80cc`  
		Last Modified: Tue, 11 Apr 2023 20:07:38 GMT  
		Size: 68.3 MB (68265081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467cf7edb3b9c6580c686624142f9e30588104828318064248595eb719e98539`  
		Last Modified: Tue, 11 Apr 2023 20:23:58 GMT  
		Size: 7.4 MB (7446001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214e6f8c21a7f549f7f9522dc668d9afa8eddfbcdff16b2768522961b03e7191`  
		Last Modified: Wed, 12 Apr 2023 19:25:08 GMT  
		Size: 225.9 MB (225856544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b00917f5db375842be6901b98e1fd9a64220def41b26fd062737b2530eabd8`  
		Last Modified: Wed, 12 Apr 2023 19:24:53 GMT  
		Size: 1.9 MB (1857122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235d96a0a3c32879486eb87465085870437051b7c741e7c0a6ae49e66e1705df`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ae2be876aa966b99ca05bd564d6d4a0e56fb52577edfbffa47d094268b8f08`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce4b41a3ee697a992c0da59a73006308d0a9f6e7b26c8e3cd68a7b3c3bea562`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569a9dcc15b4fa06d4751a2d26c7537b0f6a4cd7ead883d1927586ddd8af071e`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.2.6`

```console
$ docker pull crate@sha256:c7a28d3cb589ce4bde2f074e14267f6699573c2a1ad7039cd0034ad732bfa8ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.2.6` - linux; amd64

```console
$ docker pull crate@sha256:7a1367b86c5a7bd88195b1ddcda0402cfcd8448373506f46da74ab8fb341bfb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (305958858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f59bd1354757ce19854ee89ab40ea186080b1fdfe0168ad02d1a38f43b90a0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 19:19:48 GMT
ADD file:9022dcd506469f7fa13db0072d1e4ed93f0ddf853bdd9ff02efc8d5a0345bb78 in / 
# Tue, 11 Apr 2023 19:19:49 GMT
CMD ["/bin/bash"]
# Tue, 11 Apr 2023 19:36:50 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Wed, 12 Apr 2023 23:35:15 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.6.tar.gz.asc crate-5.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.6.tar.gz.asc     && tar -xf crate-5.2.6.tar.gz -C /crate --strip-components=1     && rm crate-5.2.6.tar.gz
# Wed, 12 Apr 2023 23:35:18 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 12 Apr 2023 23:35:18 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 23:35:18 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 12 Apr 2023 23:35:18 GMT
RUN mkdir -p /data/data /data/log
# Wed, 12 Apr 2023 23:35:18 GMT
VOLUME [/data]
# Wed, 12 Apr 2023 23:35:18 GMT
WORKDIR /data
# Wed, 12 Apr 2023 23:35:19 GMT
EXPOSE 4200 4300 5432
# Wed, 12 Apr 2023 23:35:19 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 12 Apr 2023 23:35:19 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 12 Apr 2023 23:35:19 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T08:45:48.121205 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.6
# Wed, 12 Apr 2023 23:35:19 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 12 Apr 2023 23:35:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 23:35:19 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:349bb8f337e406f9e6bd67c41b36a6481834ff3cf177d4eaa707dd54d730be7b`  
		Last Modified: Tue, 11 Apr 2023 19:21:00 GMT  
		Size: 69.4 MB (69379392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cb21b908980a44e421950e4143abc076d4fc74d81e34760821625dcda884fd`  
		Last Modified: Tue, 11 Apr 2023 19:37:39 GMT  
		Size: 7.6 MB (7603753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4664ae7d4ff7f3357d521f3e580038531ebd9ffe7a4f1993ed34e2ee872614`  
		Last Modified: Wed, 12 Apr 2023 23:35:49 GMT  
		Size: 227.1 MB (227116710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88637feddd69bcc3efa914790828ae93a2efe88b4bd9b31e94570581cb7ccd9`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 1.9 MB (1857123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fcb6338989fb6c33eb9704c6779197c9546c6c0ce91c3fb0a3e6994e4038b1`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd0f16083079ebd52814d2e1cca587d933701140bfdce0b201825c86a0839ab`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5957daf1cc916da90886881ba1fec705a3b8b6a6f49b02e03cbd45e7bbb2e20b`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee72a24c17b1bd55b91d33875e1d55d17dbca697eb64406f1c2c8384b06718b1`  
		Last Modified: Wed, 12 Apr 2023 23:35:31 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.2.6` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:b2cd329fc48c2ff5445d4560ae947564420fc55db37e528357365698310c124f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303426631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cce886f489a0b26e0a0a546c2daecb3ebed543c6c5dcc66adf22d84b4b058cf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 20:06:33 GMT
ADD file:389251b1d16989bef7dd304f924df38271d5e1140aca5e6a76aca2a98db3914b in / 
# Tue, 11 Apr 2023 20:06:35 GMT
CMD ["/bin/bash"]
# Tue, 11 Apr 2023 20:23:16 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Wed, 12 Apr 2023 19:24:30 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.6.tar.gz.asc crate-5.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.6.tar.gz.asc     && tar -xf crate-5.2.6.tar.gz -C /crate --strip-components=1     && rm crate-5.2.6.tar.gz
# Wed, 12 Apr 2023 19:24:34 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 12 Apr 2023 19:24:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 19:24:35 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 12 Apr 2023 19:24:35 GMT
RUN mkdir -p /data/data /data/log
# Wed, 12 Apr 2023 19:24:35 GMT
VOLUME [/data]
# Wed, 12 Apr 2023 19:24:35 GMT
WORKDIR /data
# Wed, 12 Apr 2023 19:24:35 GMT
EXPOSE 4200 4300 5432
# Wed, 12 Apr 2023 19:24:35 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 12 Apr 2023 19:24:36 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 12 Apr 2023 19:24:36 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T08:45:48.121205 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.6
# Wed, 12 Apr 2023 19:24:36 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 12 Apr 2023 19:24:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 19:24:36 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:8bdbb90acb62176a24ad70eb522992bed0fbe2c7a53633cc96327b2ec7fa80cc`  
		Last Modified: Tue, 11 Apr 2023 20:07:38 GMT  
		Size: 68.3 MB (68265081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467cf7edb3b9c6580c686624142f9e30588104828318064248595eb719e98539`  
		Last Modified: Tue, 11 Apr 2023 20:23:58 GMT  
		Size: 7.4 MB (7446001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214e6f8c21a7f549f7f9522dc668d9afa8eddfbcdff16b2768522961b03e7191`  
		Last Modified: Wed, 12 Apr 2023 19:25:08 GMT  
		Size: 225.9 MB (225856544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b00917f5db375842be6901b98e1fd9a64220def41b26fd062737b2530eabd8`  
		Last Modified: Wed, 12 Apr 2023 19:24:53 GMT  
		Size: 1.9 MB (1857122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235d96a0a3c32879486eb87465085870437051b7c741e7c0a6ae49e66e1705df`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ae2be876aa966b99ca05bd564d6d4a0e56fb52577edfbffa47d094268b8f08`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce4b41a3ee697a992c0da59a73006308d0a9f6e7b26c8e3cd68a7b3c3bea562`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569a9dcc15b4fa06d4751a2d26c7537b0f6a4cd7ead883d1927586ddd8af071e`  
		Last Modified: Wed, 12 Apr 2023 19:24:52 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3`

```console
$ docker pull crate@sha256:6c9df8b343e551dbbabb105f266250f4ae56e1fdcdb70557c73371ec1e12c5fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3` - linux; amd64

```console
$ docker pull crate@sha256:9578962499fc4bf036c2978e3108987b556f4557cfa9093a096a9dc858395d77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.5 MB (277468494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73da05c8bdfc04167bc12661ced7d422963a24310b03e381d612e84101da5a46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 19:19:57 GMT
ADD file:bb680be7279e885f13401f2d43d5f3a04e577d5358a84c769a7bedf7a4891531 in / 
# Tue, 11 Apr 2023 19:19:58 GMT
CMD ["/bin/bash"]
# Fri, 14 Apr 2023 21:51:31 GMT
RUN microdnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && microdnf clean all     && rm -rf /var/cache/yum
# Fri, 14 Apr 2023 21:51:53 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.0.tar.gz.asc crate-5.3.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.0.tar.gz.asc     && tar -xf crate-5.3.0.tar.gz -C /crate --strip-components=1     && rm crate-5.3.0.tar.gz
# Fri, 14 Apr 2023 21:51:58 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 14 Apr 2023 21:51:58 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 14 Apr 2023 21:51:58 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 14 Apr 2023 21:51:59 GMT
RUN mkdir -p /data/data /data/log
# Fri, 14 Apr 2023 21:51:59 GMT
VOLUME [/data]
# Fri, 14 Apr 2023 21:51:59 GMT
WORKDIR /data
# Fri, 14 Apr 2023 21:51:59 GMT
EXPOSE 4200 4300 5432
# Fri, 14 Apr 2023 21:51:59 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 14 Apr 2023 21:51:59 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 14 Apr 2023 21:51:59 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T15:04:59.126585 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.0
# Fri, 14 Apr 2023 21:51:59 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 14 Apr 2023 21:51:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Apr 2023 21:51:59 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:5f587440817f7c56198a3cc9df5d654dd56b5394b2a2a83cf5e2fb635046f2f9`  
		Last Modified: Tue, 11 Apr 2023 19:21:15 GMT  
		Size: 33.5 MB (33467186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b97aefb6e6d3b744fe84d6f5149e898a47563ccc4db07bbd90f3d1b0174a2d`  
		Last Modified: Fri, 14 Apr 2023 21:52:18 GMT  
		Size: 14.8 MB (14824560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbb604bcbab3de99f71519a657d82145cb3f23171f1ee9183c4c3473e7245ce`  
		Last Modified: Fri, 14 Apr 2023 21:52:31 GMT  
		Size: 227.3 MB (227317743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0606117830f475881dfa7794de89790ccf02926ee1d4b640e13dc43e4e22bf`  
		Last Modified: Fri, 14 Apr 2023 21:52:14 GMT  
		Size: 1.9 MB (1857120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051dbacd53d77acac3cb2779f706e670b3d9fc9124b176237bfa8bc2658320c1`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92edd0ba6435e48db4f6ba103f9fca5b1e9302d0ac2f8e965c85cab3d7338149`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790aca4b4e1fc2a572672f5e232be434f2de9c6856829b3ffad380f1a8e7a15`  
		Last Modified: Fri, 14 Apr 2023 21:52:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e743b1eb7795a2222ac1c17b8d43e6a93f84b8964986b10e07f9449446989`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:49bbe5322a56e5931acab2e2df1c995848256e4031ff88361ba341463b5c0183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274776456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c3abadbe897214e185f640602dff00795268db609b46ec5831bfe56fc43dfb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 20:06:40 GMT
ADD file:7b1cc0c631fb6d63f3a750477dd632bc0ee267c1818e5c4f339238a8a35906f6 in / 
# Tue, 11 Apr 2023 20:06:41 GMT
CMD ["/bin/bash"]
# Fri, 14 Apr 2023 22:29:44 GMT
RUN microdnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && microdnf clean all     && rm -rf /var/cache/yum
# Fri, 14 Apr 2023 22:30:06 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.0.tar.gz.asc crate-5.3.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.0.tar.gz.asc     && tar -xf crate-5.3.0.tar.gz -C /crate --strip-components=1     && rm crate-5.3.0.tar.gz
# Fri, 14 Apr 2023 22:30:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 14 Apr 2023 22:30:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 14 Apr 2023 22:30:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 14 Apr 2023 22:30:11 GMT
RUN mkdir -p /data/data /data/log
# Fri, 14 Apr 2023 22:30:11 GMT
VOLUME [/data]
# Fri, 14 Apr 2023 22:30:11 GMT
WORKDIR /data
# Fri, 14 Apr 2023 22:30:11 GMT
EXPOSE 4200 4300 5432
# Fri, 14 Apr 2023 22:30:11 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 14 Apr 2023 22:30:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 14 Apr 2023 22:30:11 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T15:04:59.126585 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.0
# Fri, 14 Apr 2023 22:30:11 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 14 Apr 2023 22:30:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Apr 2023 22:30:11 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:5db0a18ae5e09df73bc7f6baeab441113e9b1b537214f753d9106e84e7322587`  
		Last Modified: Tue, 11 Apr 2023 20:07:52 GMT  
		Size: 32.1 MB (32110138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabc1d69caa37704b96a4bdcafaa96f09984997ce39da35c36c90ec8828d458`  
		Last Modified: Fri, 14 Apr 2023 22:30:29 GMT  
		Size: 14.7 MB (14744547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60416bd1a7b57527021cf743627f0cce34bc4d50ec8b7f4ef0e4d4c6f74cf282`  
		Last Modified: Fri, 14 Apr 2023 22:30:40 GMT  
		Size: 226.1 MB (226062760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fea9c282df6e198060df2fdb98bb8e3b730aa6f8e3b2417a97f220b8e74787c`  
		Last Modified: Fri, 14 Apr 2023 22:30:26 GMT  
		Size: 1.9 MB (1857129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc626bd6a77f779471f8394b2209afde3849784b31a8e00b03363e7460bd119`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd161b1d581eccb0a524abd6db33d78e7559e6d85fe4a6b9b986fa41efaad01b`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdddc6dd4fd6aafab2a3dda5e91971c99c4ac7853b72c8d85628f9ec0014bc7e`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e683d07951c609aa62a5bdf50802b18f932ba2d97da5a19e94b228580a3054`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:5.3.0`

```console
$ docker pull crate@sha256:6c9df8b343e551dbbabb105f266250f4ae56e1fdcdb70557c73371ec1e12c5fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:5.3.0` - linux; amd64

```console
$ docker pull crate@sha256:9578962499fc4bf036c2978e3108987b556f4557cfa9093a096a9dc858395d77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.5 MB (277468494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73da05c8bdfc04167bc12661ced7d422963a24310b03e381d612e84101da5a46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 19:19:57 GMT
ADD file:bb680be7279e885f13401f2d43d5f3a04e577d5358a84c769a7bedf7a4891531 in / 
# Tue, 11 Apr 2023 19:19:58 GMT
CMD ["/bin/bash"]
# Fri, 14 Apr 2023 21:51:31 GMT
RUN microdnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && microdnf clean all     && rm -rf /var/cache/yum
# Fri, 14 Apr 2023 21:51:53 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.0.tar.gz.asc crate-5.3.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.0.tar.gz.asc     && tar -xf crate-5.3.0.tar.gz -C /crate --strip-components=1     && rm crate-5.3.0.tar.gz
# Fri, 14 Apr 2023 21:51:58 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 14 Apr 2023 21:51:58 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 14 Apr 2023 21:51:58 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 14 Apr 2023 21:51:59 GMT
RUN mkdir -p /data/data /data/log
# Fri, 14 Apr 2023 21:51:59 GMT
VOLUME [/data]
# Fri, 14 Apr 2023 21:51:59 GMT
WORKDIR /data
# Fri, 14 Apr 2023 21:51:59 GMT
EXPOSE 4200 4300 5432
# Fri, 14 Apr 2023 21:51:59 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 14 Apr 2023 21:51:59 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 14 Apr 2023 21:51:59 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T15:04:59.126585 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.0
# Fri, 14 Apr 2023 21:51:59 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 14 Apr 2023 21:51:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Apr 2023 21:51:59 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:5f587440817f7c56198a3cc9df5d654dd56b5394b2a2a83cf5e2fb635046f2f9`  
		Last Modified: Tue, 11 Apr 2023 19:21:15 GMT  
		Size: 33.5 MB (33467186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b97aefb6e6d3b744fe84d6f5149e898a47563ccc4db07bbd90f3d1b0174a2d`  
		Last Modified: Fri, 14 Apr 2023 21:52:18 GMT  
		Size: 14.8 MB (14824560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbb604bcbab3de99f71519a657d82145cb3f23171f1ee9183c4c3473e7245ce`  
		Last Modified: Fri, 14 Apr 2023 21:52:31 GMT  
		Size: 227.3 MB (227317743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0606117830f475881dfa7794de89790ccf02926ee1d4b640e13dc43e4e22bf`  
		Last Modified: Fri, 14 Apr 2023 21:52:14 GMT  
		Size: 1.9 MB (1857120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051dbacd53d77acac3cb2779f706e670b3d9fc9124b176237bfa8bc2658320c1`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92edd0ba6435e48db4f6ba103f9fca5b1e9302d0ac2f8e965c85cab3d7338149`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790aca4b4e1fc2a572672f5e232be434f2de9c6856829b3ffad380f1a8e7a15`  
		Last Modified: Fri, 14 Apr 2023 21:52:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e743b1eb7795a2222ac1c17b8d43e6a93f84b8964986b10e07f9449446989`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:5.3.0` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:49bbe5322a56e5931acab2e2df1c995848256e4031ff88361ba341463b5c0183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274776456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c3abadbe897214e185f640602dff00795268db609b46ec5831bfe56fc43dfb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 20:06:40 GMT
ADD file:7b1cc0c631fb6d63f3a750477dd632bc0ee267c1818e5c4f339238a8a35906f6 in / 
# Tue, 11 Apr 2023 20:06:41 GMT
CMD ["/bin/bash"]
# Fri, 14 Apr 2023 22:29:44 GMT
RUN microdnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && microdnf clean all     && rm -rf /var/cache/yum
# Fri, 14 Apr 2023 22:30:06 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.0.tar.gz.asc crate-5.3.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.0.tar.gz.asc     && tar -xf crate-5.3.0.tar.gz -C /crate --strip-components=1     && rm crate-5.3.0.tar.gz
# Fri, 14 Apr 2023 22:30:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 14 Apr 2023 22:30:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 14 Apr 2023 22:30:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 14 Apr 2023 22:30:11 GMT
RUN mkdir -p /data/data /data/log
# Fri, 14 Apr 2023 22:30:11 GMT
VOLUME [/data]
# Fri, 14 Apr 2023 22:30:11 GMT
WORKDIR /data
# Fri, 14 Apr 2023 22:30:11 GMT
EXPOSE 4200 4300 5432
# Fri, 14 Apr 2023 22:30:11 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 14 Apr 2023 22:30:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 14 Apr 2023 22:30:11 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T15:04:59.126585 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.0
# Fri, 14 Apr 2023 22:30:11 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 14 Apr 2023 22:30:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Apr 2023 22:30:11 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:5db0a18ae5e09df73bc7f6baeab441113e9b1b537214f753d9106e84e7322587`  
		Last Modified: Tue, 11 Apr 2023 20:07:52 GMT  
		Size: 32.1 MB (32110138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabc1d69caa37704b96a4bdcafaa96f09984997ce39da35c36c90ec8828d458`  
		Last Modified: Fri, 14 Apr 2023 22:30:29 GMT  
		Size: 14.7 MB (14744547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60416bd1a7b57527021cf743627f0cce34bc4d50ec8b7f4ef0e4d4c6f74cf282`  
		Last Modified: Fri, 14 Apr 2023 22:30:40 GMT  
		Size: 226.1 MB (226062760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fea9c282df6e198060df2fdb98bb8e3b730aa6f8e3b2417a97f220b8e74787c`  
		Last Modified: Fri, 14 Apr 2023 22:30:26 GMT  
		Size: 1.9 MB (1857129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc626bd6a77f779471f8394b2209afde3849784b31a8e00b03363e7460bd119`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd161b1d581eccb0a524abd6db33d78e7559e6d85fe4a6b9b986fa41efaad01b`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdddc6dd4fd6aafab2a3dda5e91971c99c4ac7853b72c8d85628f9ec0014bc7e`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e683d07951c609aa62a5bdf50802b18f932ba2d97da5a19e94b228580a3054`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:6c9df8b343e551dbbabb105f266250f4ae56e1fdcdb70557c73371ec1e12c5fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:9578962499fc4bf036c2978e3108987b556f4557cfa9093a096a9dc858395d77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.5 MB (277468494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73da05c8bdfc04167bc12661ced7d422963a24310b03e381d612e84101da5a46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 19:19:57 GMT
ADD file:bb680be7279e885f13401f2d43d5f3a04e577d5358a84c769a7bedf7a4891531 in / 
# Tue, 11 Apr 2023 19:19:58 GMT
CMD ["/bin/bash"]
# Fri, 14 Apr 2023 21:51:31 GMT
RUN microdnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && microdnf clean all     && rm -rf /var/cache/yum
# Fri, 14 Apr 2023 21:51:53 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.0.tar.gz.asc crate-5.3.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.0.tar.gz.asc     && tar -xf crate-5.3.0.tar.gz -C /crate --strip-components=1     && rm crate-5.3.0.tar.gz
# Fri, 14 Apr 2023 21:51:58 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 14 Apr 2023 21:51:58 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 14 Apr 2023 21:51:58 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 14 Apr 2023 21:51:59 GMT
RUN mkdir -p /data/data /data/log
# Fri, 14 Apr 2023 21:51:59 GMT
VOLUME [/data]
# Fri, 14 Apr 2023 21:51:59 GMT
WORKDIR /data
# Fri, 14 Apr 2023 21:51:59 GMT
EXPOSE 4200 4300 5432
# Fri, 14 Apr 2023 21:51:59 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 14 Apr 2023 21:51:59 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 14 Apr 2023 21:51:59 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T15:04:59.126585 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.0
# Fri, 14 Apr 2023 21:51:59 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 14 Apr 2023 21:51:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Apr 2023 21:51:59 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:5f587440817f7c56198a3cc9df5d654dd56b5394b2a2a83cf5e2fb635046f2f9`  
		Last Modified: Tue, 11 Apr 2023 19:21:15 GMT  
		Size: 33.5 MB (33467186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b97aefb6e6d3b744fe84d6f5149e898a47563ccc4db07bbd90f3d1b0174a2d`  
		Last Modified: Fri, 14 Apr 2023 21:52:18 GMT  
		Size: 14.8 MB (14824560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbb604bcbab3de99f71519a657d82145cb3f23171f1ee9183c4c3473e7245ce`  
		Last Modified: Fri, 14 Apr 2023 21:52:31 GMT  
		Size: 227.3 MB (227317743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0606117830f475881dfa7794de89790ccf02926ee1d4b640e13dc43e4e22bf`  
		Last Modified: Fri, 14 Apr 2023 21:52:14 GMT  
		Size: 1.9 MB (1857120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051dbacd53d77acac3cb2779f706e670b3d9fc9124b176237bfa8bc2658320c1`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92edd0ba6435e48db4f6ba103f9fca5b1e9302d0ac2f8e965c85cab3d7338149`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790aca4b4e1fc2a572672f5e232be434f2de9c6856829b3ffad380f1a8e7a15`  
		Last Modified: Fri, 14 Apr 2023 21:52:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e743b1eb7795a2222ac1c17b8d43e6a93f84b8964986b10e07f9449446989`  
		Last Modified: Fri, 14 Apr 2023 21:52:13 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:49bbe5322a56e5931acab2e2df1c995848256e4031ff88361ba341463b5c0183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274776456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c3abadbe897214e185f640602dff00795268db609b46ec5831bfe56fc43dfb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 20:06:40 GMT
ADD file:7b1cc0c631fb6d63f3a750477dd632bc0ee267c1818e5c4f339238a8a35906f6 in / 
# Tue, 11 Apr 2023 20:06:41 GMT
CMD ["/bin/bash"]
# Fri, 14 Apr 2023 22:29:44 GMT
RUN microdnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && microdnf clean all     && rm -rf /var/cache/yum
# Fri, 14 Apr 2023 22:30:06 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.3.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.3.0.tar.gz.asc crate-5.3.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.3.0.tar.gz.asc     && tar -xf crate-5.3.0.tar.gz -C /crate --strip-components=1     && rm crate-5.3.0.tar.gz
# Fri, 14 Apr 2023 22:30:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 14 Apr 2023 22:30:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 14 Apr 2023 22:30:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 14 Apr 2023 22:30:11 GMT
RUN mkdir -p /data/data /data/log
# Fri, 14 Apr 2023 22:30:11 GMT
VOLUME [/data]
# Fri, 14 Apr 2023 22:30:11 GMT
WORKDIR /data
# Fri, 14 Apr 2023 22:30:11 GMT
EXPOSE 4200 4300 5432
# Fri, 14 Apr 2023 22:30:11 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 14 Apr 2023 22:30:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 14 Apr 2023 22:30:11 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-04-04T15:04:59.126585 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.3.0
# Fri, 14 Apr 2023 22:30:11 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 14 Apr 2023 22:30:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Apr 2023 22:30:11 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:5db0a18ae5e09df73bc7f6baeab441113e9b1b537214f753d9106e84e7322587`  
		Last Modified: Tue, 11 Apr 2023 20:07:52 GMT  
		Size: 32.1 MB (32110138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabc1d69caa37704b96a4bdcafaa96f09984997ce39da35c36c90ec8828d458`  
		Last Modified: Fri, 14 Apr 2023 22:30:29 GMT  
		Size: 14.7 MB (14744547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60416bd1a7b57527021cf743627f0cce34bc4d50ec8b7f4ef0e4d4c6f74cf282`  
		Last Modified: Fri, 14 Apr 2023 22:30:40 GMT  
		Size: 226.1 MB (226062760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fea9c282df6e198060df2fdb98bb8e3b730aa6f8e3b2417a97f220b8e74787c`  
		Last Modified: Fri, 14 Apr 2023 22:30:26 GMT  
		Size: 1.9 MB (1857129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc626bd6a77f779471f8394b2209afde3849784b31a8e00b03363e7460bd119`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd161b1d581eccb0a524abd6db33d78e7559e6d85fe4a6b9b986fa41efaad01b`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdddc6dd4fd6aafab2a3dda5e91971c99c4ac7853b72c8d85628f9ec0014bc7e`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e683d07951c609aa62a5bdf50802b18f932ba2d97da5a19e94b228580a3054`  
		Last Modified: Fri, 14 Apr 2023 22:30:25 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
