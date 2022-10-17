## `crate:latest`

```console
$ docker pull crate@sha256:cdc99aa5b91281f7ef26cba6138db6dc2bec6a8701db81232d731e892c00569e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:636ea04b84ad7919c1fd2cc5fd75b79da267996b1a656f668c0b138967a30f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371123309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6276eb32d11cb49141419e1fd018d82a1224f72a0fa756e6369be3a6590d382d`
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
# Mon, 17 Oct 2022 20:26:01 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.0.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.0.2.tar.gz.asc crate-5.0.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.0.2.tar.gz.asc     && tar -xf crate-5.0.2.tar.gz -C /crate --strip-components=1     && rm crate-5.0.2.tar.gz
# Mon, 17 Oct 2022 20:26:06 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 17 Oct 2022 20:26:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Oct 2022 20:26:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 17 Oct 2022 20:26:07 GMT
RUN mkdir -p /data/data /data/log
# Mon, 17 Oct 2022 20:26:07 GMT
VOLUME [/data]
# Mon, 17 Oct 2022 20:26:08 GMT
WORKDIR /data
# Mon, 17 Oct 2022 20:26:08 GMT
EXPOSE 4200 4300 5432
# Mon, 17 Oct 2022 20:26:08 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 17 Oct 2022 20:26:08 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 17 Oct 2022 20:26:08 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-10-10T13:52:35.066838 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.0.2
# Mon, 17 Oct 2022 20:26:08 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 17 Oct 2022 20:26:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 17 Oct 2022 20:26:08 GMT
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
	-	`sha256:aa4513680edd3e500fc63779f7b9f8e5cdee342799df68da719364438141d632`  
		Last Modified: Mon, 17 Oct 2022 20:26:46 GMT  
		Size: 216.2 MB (216164137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c32a721d5ec6099fa7664797f8217b72d04fa884d67273b6e4ae4df93dc94dc`  
		Last Modified: Mon, 17 Oct 2022 20:26:27 GMT  
		Size: 1.7 MB (1710780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd93d2092222b0a6f91b088cb27835d701598466d43290fc3cad16f08ed9a7b`  
		Last Modified: Mon, 17 Oct 2022 20:26:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8a89919d90f2b2ceba51bab2bb04d93bd5528239f215240bd311ae49ec6f52`  
		Last Modified: Mon, 17 Oct 2022 20:26:26 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3e1ade16511c9bc4b5618aa566feb1d21108f6e6b515a0c6ed90409cdad2fc`  
		Last Modified: Mon, 17 Oct 2022 20:26:27 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af3c428ca30742d3bee8517f47b30d7982c082f85c8d9c0238c7a99a671f097`  
		Last Modified: Mon, 17 Oct 2022 20:26:26 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:a3e10c6013b4eb50bcf2223c99740e1b7cb58bdfae7ae7bf09f6d421ef7842c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **669.8 MB (669802341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:794d96da95625fdd9cf87fcdd26386828b216b859175e67968159663f1a85dc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 12 Sep 2022 18:41:37 GMT
RUN yum install -y yum-utils deltarpm     && yum makecache     && yum upgrade -y     && yum install -y python3 openssl     && pip3 install --upgrade pip     && yum clean all     && rm -rf /var/cache/yum
# Mon, 17 Oct 2022 20:56:35 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.0.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.0.2.tar.gz.asc crate-5.0.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.0.2.tar.gz.asc     && tar -xf crate-5.0.2.tar.gz -C /crate --strip-components=1     && rm crate-5.0.2.tar.gz
# Mon, 17 Oct 2022 20:56:40 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 17 Oct 2022 20:56:40 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Oct 2022 20:56:41 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 17 Oct 2022 20:56:43 GMT
RUN mkdir -p /data/data /data/log
# Mon, 17 Oct 2022 20:56:44 GMT
VOLUME [/data]
# Mon, 17 Oct 2022 20:56:44 GMT
WORKDIR /data
# Mon, 17 Oct 2022 20:56:45 GMT
EXPOSE 4200 4300 5432
# Mon, 17 Oct 2022 20:56:47 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 17 Oct 2022 20:56:48 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 17 Oct 2022 20:56:48 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2022-10-10T13:52:35.066838 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.0.2
# Mon, 17 Oct 2022 20:56:50 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 17 Oct 2022 20:56:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 17 Oct 2022 20:56:51 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedd238cd1f3b3e268d51c624ab3e844a43301b4842b7ce7a77ec4a3f87d42d8`  
		Last Modified: Mon, 12 Sep 2022 18:44:32 GMT  
		Size: 344.7 MB (344689460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0fc57c2807048a196ffd0490dd885b3e9f333ad9fb9714339457414943d72c`  
		Last Modified: Mon, 17 Oct 2022 20:57:49 GMT  
		Size: 215.0 MB (215026743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870eb83cf1363b55b7e3c4a2ef51768cc5a5595ce1ab874111f21a4208918031`  
		Last Modified: Mon, 17 Oct 2022 20:57:28 GMT  
		Size: 1.7 MB (1709339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a944009cabe80b17ddad3fe36ad241f580eb4124351746244fff09c854b5a3`  
		Last Modified: Mon, 17 Oct 2022 20:57:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259922db4d8cd5788e436aa937a41947fe18964a94b3daada0f2e924e26a10a8`  
		Last Modified: Mon, 17 Oct 2022 20:57:27 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9c69c6b96bfabaea36dc620beb90ee96dd6f88dc2e26d6a68cb9258de3de8d`  
		Last Modified: Mon, 17 Oct 2022 20:57:27 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fa0b7572d90a0616ad6ccd67028bab90aa27470af02e90402aff4063f6aa85`  
		Last Modified: Mon, 17 Oct 2022 20:57:27 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
