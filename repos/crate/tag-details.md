<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:4.6`](#crate46)
-	[`crate:4.6.6`](#crate466)
-	[`crate:latest`](#cratelatest)

## `crate:4.6`

```console
$ docker pull crate@sha256:7e9a6f7d9821ea6806e663cc102c2c9345be732740010f55c5cd11b4c3d0aebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.6` - linux; amd64

```console
$ docker pull crate@sha256:079921578e4d9ca41940fd0497e16ceec0b93861d92a04eb4538adc6eae8cff9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333284088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b809a874f7ee3611e1a313bd937b009355067ce097f0e60a0739e82f3a50e88`
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
# Wed, 15 Dec 2021 18:20:16 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.6.tar.gz.asc crate-4.6.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.6.tar.gz.asc     && tar -xf crate-4.6.6.tar.gz -C /crate --strip-components=1     && rm crate-4.6.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 15 Dec 2021 18:20:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 15 Dec 2021 18:20:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 18:20:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 15 Dec 2021 18:20:21 GMT
RUN mkdir -p /data/data /data/log
# Wed, 15 Dec 2021 18:20:21 GMT
VOLUME [/data]
# Wed, 15 Dec 2021 18:20:21 GMT
WORKDIR /data
# Wed, 15 Dec 2021 18:20:22 GMT
EXPOSE 4200 4300 5432
# Wed, 15 Dec 2021 18:20:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 15 Dec 2021 18:20:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 15 Dec 2021 18:20:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-12-13T11:12:49.493682 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.6
# Wed, 15 Dec 2021 18:20:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 15 Dec 2021 18:20:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 18:20:23 GMT
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
	-	`sha256:a6322f474bb37b8eee992a2dcc0c0eab3ea304e20353d1fea6ad4de0a7f2a5fe`  
		Last Modified: Wed, 15 Dec 2021 18:21:27 GMT  
		Size: 255.6 MB (255600599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07263f1d9ec74bc33c85f038efa374c0026a9869bdfb7173af894d6298116af`  
		Last Modified: Wed, 15 Dec 2021 18:21:03 GMT  
		Size: 1.6 MB (1582191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa05ad57e72cdf062d8ad03f8c10bfd64734c634feb4b321a2bfe39dbfeb6d68`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c672d1c03b4af1d7a329abce023c439100199f017c333ffa2392c9b6a81fd1b`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa262c91b5ccaf31547890daa9e97b582f463db7c7eb302c8f923918168c3eb`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2689748241fb7c8df8b5c656865fe4e668f904240f400c55e354da004914e4b5`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.6` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:34bcd1fe92ffd4db2f2ed4e5721fe433702ce8a54812601006a71d3d5c665a41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d8e8b83285a4c3e5471b3d109e74d665052da13455758e6ef17478564355bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 17:39:58 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Wed, 15 Sep 2021 17:39:58 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 17:39:59 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 17:39:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 15 Dec 2021 18:42:00 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.6.tar.gz.asc crate-4.6.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.6.tar.gz.asc     && tar -xf crate-4.6.6.tar.gz -C /crate --strip-components=1     && rm crate-4.6.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 15 Dec 2021 18:42:05 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 15 Dec 2021 18:42:06 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 18:42:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 15 Dec 2021 18:42:09 GMT
RUN mkdir -p /data/data /data/log
# Wed, 15 Dec 2021 18:42:09 GMT
VOLUME [/data]
# Wed, 15 Dec 2021 18:42:10 GMT
WORKDIR /data
# Wed, 15 Dec 2021 18:42:11 GMT
EXPOSE 4200 4300 5432
# Wed, 15 Dec 2021 18:42:13 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 15 Dec 2021 18:42:14 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 15 Dec 2021 18:42:14 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-12-13T11:12:49.493682 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.6
# Wed, 15 Dec 2021 18:42:16 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 15 Dec 2021 18:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 18:42:17 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e276594d35170abf49132218c828dbb53b9fc83765b7a2d3012449d3af249`  
		Last Modified: Fri, 19 Nov 2021 17:52:16 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174dd1e7af8c7bc1ff2df4ba200069ff5252a8a3b98252bc27983683bba6ecb`  
		Last Modified: Wed, 15 Dec 2021 18:45:34 GMT  
		Size: 252.4 MB (252384760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2038c0e0b63e6ab23095aae125c693daa729c6b4ecc37023399bd0829533d7f`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba526afd18fefe767f2fe38af4e8624cb07429449e44ac0f9bc63780b8d7ba`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98811ef1c8dbdb24035ef26fac6506fee87d875771495692659b242a5080bbdb`  
		Last Modified: Wed, 15 Dec 2021 18:45:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb0bb58a551e595688652109928b719e850207a2721257a00e878ca98ba88ff`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292cf669746a9a8e6bdb06bbacb7fb1a5cb4f13ba31e657cbcf4e04c13e05c6`  
		Last Modified: Wed, 15 Dec 2021 18:45:06 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.6.6`

```console
$ docker pull crate@sha256:7e9a6f7d9821ea6806e663cc102c2c9345be732740010f55c5cd11b4c3d0aebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.6.6` - linux; amd64

```console
$ docker pull crate@sha256:079921578e4d9ca41940fd0497e16ceec0b93861d92a04eb4538adc6eae8cff9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333284088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b809a874f7ee3611e1a313bd937b009355067ce097f0e60a0739e82f3a50e88`
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
# Wed, 15 Dec 2021 18:20:16 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.6.tar.gz.asc crate-4.6.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.6.tar.gz.asc     && tar -xf crate-4.6.6.tar.gz -C /crate --strip-components=1     && rm crate-4.6.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 15 Dec 2021 18:20:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 15 Dec 2021 18:20:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 18:20:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 15 Dec 2021 18:20:21 GMT
RUN mkdir -p /data/data /data/log
# Wed, 15 Dec 2021 18:20:21 GMT
VOLUME [/data]
# Wed, 15 Dec 2021 18:20:21 GMT
WORKDIR /data
# Wed, 15 Dec 2021 18:20:22 GMT
EXPOSE 4200 4300 5432
# Wed, 15 Dec 2021 18:20:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 15 Dec 2021 18:20:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 15 Dec 2021 18:20:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-12-13T11:12:49.493682 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.6
# Wed, 15 Dec 2021 18:20:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 15 Dec 2021 18:20:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 18:20:23 GMT
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
	-	`sha256:a6322f474bb37b8eee992a2dcc0c0eab3ea304e20353d1fea6ad4de0a7f2a5fe`  
		Last Modified: Wed, 15 Dec 2021 18:21:27 GMT  
		Size: 255.6 MB (255600599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07263f1d9ec74bc33c85f038efa374c0026a9869bdfb7173af894d6298116af`  
		Last Modified: Wed, 15 Dec 2021 18:21:03 GMT  
		Size: 1.6 MB (1582191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa05ad57e72cdf062d8ad03f8c10bfd64734c634feb4b321a2bfe39dbfeb6d68`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c672d1c03b4af1d7a329abce023c439100199f017c333ffa2392c9b6a81fd1b`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa262c91b5ccaf31547890daa9e97b582f463db7c7eb302c8f923918168c3eb`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2689748241fb7c8df8b5c656865fe4e668f904240f400c55e354da004914e4b5`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.6.6` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:34bcd1fe92ffd4db2f2ed4e5721fe433702ce8a54812601006a71d3d5c665a41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d8e8b83285a4c3e5471b3d109e74d665052da13455758e6ef17478564355bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 17:39:58 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Wed, 15 Sep 2021 17:39:58 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 17:39:59 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 17:39:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 15 Dec 2021 18:42:00 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.6.tar.gz.asc crate-4.6.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.6.tar.gz.asc     && tar -xf crate-4.6.6.tar.gz -C /crate --strip-components=1     && rm crate-4.6.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 15 Dec 2021 18:42:05 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 15 Dec 2021 18:42:06 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 18:42:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 15 Dec 2021 18:42:09 GMT
RUN mkdir -p /data/data /data/log
# Wed, 15 Dec 2021 18:42:09 GMT
VOLUME [/data]
# Wed, 15 Dec 2021 18:42:10 GMT
WORKDIR /data
# Wed, 15 Dec 2021 18:42:11 GMT
EXPOSE 4200 4300 5432
# Wed, 15 Dec 2021 18:42:13 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 15 Dec 2021 18:42:14 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 15 Dec 2021 18:42:14 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-12-13T11:12:49.493682 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.6
# Wed, 15 Dec 2021 18:42:16 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 15 Dec 2021 18:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 18:42:17 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e276594d35170abf49132218c828dbb53b9fc83765b7a2d3012449d3af249`  
		Last Modified: Fri, 19 Nov 2021 17:52:16 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174dd1e7af8c7bc1ff2df4ba200069ff5252a8a3b98252bc27983683bba6ecb`  
		Last Modified: Wed, 15 Dec 2021 18:45:34 GMT  
		Size: 252.4 MB (252384760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2038c0e0b63e6ab23095aae125c693daa729c6b4ecc37023399bd0829533d7f`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba526afd18fefe767f2fe38af4e8624cb07429449e44ac0f9bc63780b8d7ba`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98811ef1c8dbdb24035ef26fac6506fee87d875771495692659b242a5080bbdb`  
		Last Modified: Wed, 15 Dec 2021 18:45:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb0bb58a551e595688652109928b719e850207a2721257a00e878ca98ba88ff`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292cf669746a9a8e6bdb06bbacb7fb1a5cb4f13ba31e657cbcf4e04c13e05c6`  
		Last Modified: Wed, 15 Dec 2021 18:45:06 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:7e9a6f7d9821ea6806e663cc102c2c9345be732740010f55c5cd11b4c3d0aebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:079921578e4d9ca41940fd0497e16ceec0b93861d92a04eb4538adc6eae8cff9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333284088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b809a874f7ee3611e1a313bd937b009355067ce097f0e60a0739e82f3a50e88`
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
# Wed, 15 Dec 2021 18:20:16 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.6.tar.gz.asc crate-4.6.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.6.tar.gz.asc     && tar -xf crate-4.6.6.tar.gz -C /crate --strip-components=1     && rm crate-4.6.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 15 Dec 2021 18:20:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 15 Dec 2021 18:20:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 18:20:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 15 Dec 2021 18:20:21 GMT
RUN mkdir -p /data/data /data/log
# Wed, 15 Dec 2021 18:20:21 GMT
VOLUME [/data]
# Wed, 15 Dec 2021 18:20:21 GMT
WORKDIR /data
# Wed, 15 Dec 2021 18:20:22 GMT
EXPOSE 4200 4300 5432
# Wed, 15 Dec 2021 18:20:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 15 Dec 2021 18:20:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 15 Dec 2021 18:20:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-12-13T11:12:49.493682 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.6
# Wed, 15 Dec 2021 18:20:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 15 Dec 2021 18:20:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 18:20:23 GMT
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
	-	`sha256:a6322f474bb37b8eee992a2dcc0c0eab3ea304e20353d1fea6ad4de0a7f2a5fe`  
		Last Modified: Wed, 15 Dec 2021 18:21:27 GMT  
		Size: 255.6 MB (255600599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07263f1d9ec74bc33c85f038efa374c0026a9869bdfb7173af894d6298116af`  
		Last Modified: Wed, 15 Dec 2021 18:21:03 GMT  
		Size: 1.6 MB (1582191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa05ad57e72cdf062d8ad03f8c10bfd64734c634feb4b321a2bfe39dbfeb6d68`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c672d1c03b4af1d7a329abce023c439100199f017c333ffa2392c9b6a81fd1b`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa262c91b5ccaf31547890daa9e97b582f463db7c7eb302c8f923918168c3eb`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2689748241fb7c8df8b5c656865fe4e668f904240f400c55e354da004914e4b5`  
		Last Modified: Wed, 15 Dec 2021 18:21:02 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:34bcd1fe92ffd4db2f2ed4e5721fe433702ce8a54812601006a71d3d5c665a41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362344341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d8e8b83285a4c3e5471b3d109e74d665052da13455758e6ef17478564355bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Wed, 15 Sep 2021 17:39:58 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Wed, 15 Sep 2021 17:39:58 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 17:39:59 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 17:39:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 15 Dec 2021 18:42:00 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.6.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.6.6.tar.gz.asc crate-4.6.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.6.6.tar.gz.asc     && tar -xf crate-4.6.6.tar.gz -C /crate --strip-components=1     && rm crate-4.6.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 15 Dec 2021 18:42:05 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 15 Dec 2021 18:42:06 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Dec 2021 18:42:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 15 Dec 2021 18:42:09 GMT
RUN mkdir -p /data/data /data/log
# Wed, 15 Dec 2021 18:42:09 GMT
VOLUME [/data]
# Wed, 15 Dec 2021 18:42:10 GMT
WORKDIR /data
# Wed, 15 Dec 2021 18:42:11 GMT
EXPOSE 4200 4300 5432
# Wed, 15 Dec 2021 18:42:13 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 15 Dec 2021 18:42:14 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 15 Dec 2021 18:42:14 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-12-13T11:12:49.493682 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.6.6
# Wed, 15 Dec 2021 18:42:16 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 15 Dec 2021 18:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 18:42:17 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e276594d35170abf49132218c828dbb53b9fc83765b7a2d3012449d3af249`  
		Last Modified: Fri, 19 Nov 2021 17:52:16 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6174dd1e7af8c7bc1ff2df4ba200069ff5252a8a3b98252bc27983683bba6ecb`  
		Last Modified: Wed, 15 Dec 2021 18:45:34 GMT  
		Size: 252.4 MB (252384760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2038c0e0b63e6ab23095aae125c693daa729c6b4ecc37023399bd0829533d7f`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 1.6 MB (1580578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba526afd18fefe767f2fe38af4e8624cb07429449e44ac0f9bc63780b8d7ba`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98811ef1c8dbdb24035ef26fac6506fee87d875771495692659b242a5080bbdb`  
		Last Modified: Wed, 15 Dec 2021 18:45:09 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb0bb58a551e595688652109928b719e850207a2721257a00e878ca98ba88ff`  
		Last Modified: Wed, 15 Dec 2021 18:45:07 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292cf669746a9a8e6bdb06bbacb7fb1a5cb4f13ba31e657cbcf4e04c13e05c6`  
		Last Modified: Wed, 15 Dec 2021 18:45:06 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
