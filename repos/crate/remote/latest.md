## `crate:latest`

```console
$ docker pull crate@sha256:53d50bdcf4f55759a128627c7074e73138e14cc80d2d5d6267d627de7b829129
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:2cb4def2c40399572ce2751b362e7ac3d66fd5339f988c0a65e594e424291ed1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331650641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972fb234916d4466032fcd1b10fde8f4e7f4a8715bfcdf1997064e474b505038`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Tue, 09 Mar 2021 20:19:32 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 24 Jun 2021 19:21:19 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 19:21:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 19:21:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 19:21:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 19:21:33 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 19:21:33 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:21:33 GMT
WORKDIR /data
# Thu, 24 Jun 2021 19:21:34 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 19:21:34 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 19:21:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 19:21:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 19:21:35 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926db4efe32a315f470abd127b4b539a23e0b3d91f7bd574eea57006cbc72b94`  
		Last Modified: Tue, 09 Mar 2021 20:25:32 GMT  
		Size: 2.3 KB (2254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc329942bda5a423587272a404accf60dbcb9ebcf0a7897cec067c73ed731d8`  
		Last Modified: Thu, 24 Jun 2021 19:22:36 GMT  
		Size: 254.0 MB (253967169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61053c3bf2c4ead0f73027e3524c34c9ae49f6861535c40bd8ad0a9e1c485730`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 1.6 MB (1582181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bab11a61bd1c7c2af14234136b0e58ff3641267df0b1461cd6e50d46ebc29a4`  
		Last Modified: Thu, 24 Jun 2021 19:22:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a238762f62ecad53037cc6ee1a8502d76e147222c5ef3c8294e9bf026a17a`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d6ff6f0a4903bd888409121f33fee3fc04a8bc25898ad1d7f99f457edece8`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c3c7b0444faf6034ad134fca95717b32fe02c9a275e42cf4b048b6455ed03`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:d177532e186aba61de4d54b1f437fa5d8e0f8dd33e1a499be039ba8a157800a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360685324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ed7d10f8d644721cbb42a72bd1765a6c66201b64a5131eb936272e45cc9d00`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Sat, 14 Nov 2020 00:40:26 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Sat, 14 Nov 2020 00:40:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:40:32 GMT
CMD ["/bin/bash"]
# Thu, 24 Jun 2021 18:41:15 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Thu, 24 Jun 2021 18:42:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:42:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:42:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:42:26 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:42:27 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:42:27 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:42:27 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:42:28 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 18:42:28 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:42:28 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0504bae3036b8b424fe4a0fb15ad01fd1048486db6c038a1e8ba073fb637bf`  
		Last Modified: Thu, 24 Jun 2021 18:50:44 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2913fc3db3db14b5c5965fa8bf1a4238cec1ad88a51953cee6879c9640e68600`  
		Last Modified: Thu, 24 Jun 2021 18:51:10 GMT  
		Size: 250.7 MB (250724036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd85191a67d5c23f76cf0af887841989f7824958426183ccb44826242a3c2d8a`  
		Last Modified: Thu, 24 Jun 2021 18:50:42 GMT  
		Size: 1.6 MB (1582201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f3c3711dd535b2a2b89ad7447fd1b7e48cb7bbc64b294e2b34b8f93318915`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ccf937bdf10288d078d2e76a470533844833d3e1be62283d14a7f0ac84fbdf`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1fbc52778409789c05f322f4fc484613b2b36aee708b48f6c27452a28cde9e`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b48081fa4b69263a82d3f6c260050f4596c08cfa730d2fae5eca13105459dd`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
