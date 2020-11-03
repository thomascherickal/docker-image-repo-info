## `crate:latest`

```console
$ docker pull crate@sha256:755a6696c2307c7b3fa05d00897665aa59412bdab202f9acb32b0fce3753028f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:39b0b78dff75adaab706a1bad5415a137ec2775fcb8c40bfdb1004e843914958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331085052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:669228c39c8dd208476612ebaad456e03d1fb939acc7db785c2e6c5e27a7524e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 02 Nov 2020 23:24:11 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.1.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.1.tar.gz.asc crate-4.3.1.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.1.tar.gz.asc     && tar -xf crate-4.3.1.tar.gz -C /crate --strip-components=1     && rm crate-4.3.1.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 02 Nov 2020 23:24:14 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 02 Nov 2020 23:24:14 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 Nov 2020 23:24:15 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 02 Nov 2020 23:24:15 GMT
RUN mkdir -p /data/data /data/log
# Mon, 02 Nov 2020 23:24:16 GMT
VOLUME [/data]
# Mon, 02 Nov 2020 23:24:16 GMT
WORKDIR /data
# Mon, 02 Nov 2020 23:24:16 GMT
EXPOSE 4200 4300 5432
# Mon, 02 Nov 2020 23:24:16 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 02 Nov 2020 23:24:16 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 02 Nov 2020 23:24:17 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-29T10:42:21.484922 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.1
# Mon, 02 Nov 2020 23:24:17 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 02 Nov 2020 23:24:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:24:17 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa480d635450b303da0dd698cb73527a4de747be3f6d436f16f9d4a1229ecbf`  
		Last Modified: Mon, 02 Nov 2020 23:25:39 GMT  
		Size: 253.7 MB (253650081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67db97b872f95a06faf0761809f1a790fa630c213fd4486398a723c8a66eb793`  
		Last Modified: Mon, 02 Nov 2020 23:24:47 GMT  
		Size: 1.6 MB (1567709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641671de35c4a537a24659b593b6b3693671d499cf415302c0377278542c3cd7`  
		Last Modified: Mon, 02 Nov 2020 23:24:47 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb8b0836d4ef9ace4e36c4e19aa857d5e326f2015fff535ffd5cb9466f3e195`  
		Last Modified: Mon, 02 Nov 2020 23:24:47 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022ed61840906891b386c279f02e55fd6a41799eb5b0710edb78244212dde109`  
		Last Modified: Mon, 02 Nov 2020 23:24:47 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687084874b8c99d8c141af84c0b7194d6fc1f6c9dcf189d4b9237538d2415c4f`  
		Last Modified: Mon, 02 Nov 2020 23:24:48 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:ddeba0693b3b5955aa645be224c5155a6d8959d7781ea1204ba44958a62b58ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.1 MB (361108401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0281394e4bd939cf4b1122d2dd3513e3aea8039d1fe8c5f70244db6404baa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 21 Oct 2020 18:45:28 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 21 Oct 2020 18:45:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 21 Oct 2020 18:45:37 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Oct 2020 18:45:37 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 21 Oct 2020 18:45:39 GMT
RUN mkdir -p /data/data /data/log
# Wed, 21 Oct 2020 18:45:40 GMT
VOLUME [/data]
# Wed, 21 Oct 2020 18:45:43 GMT
WORKDIR /data
# Wed, 21 Oct 2020 18:45:45 GMT
EXPOSE 4200 4300 5432
# Wed, 21 Oct 2020 18:45:46 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 21 Oct 2020 18:45:46 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 21 Oct 2020 18:45:47 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Wed, 21 Oct 2020 18:45:48 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 21 Oct 2020 18:45:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 21 Oct 2020 18:45:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b9ea960ebf6e65605348a44e084562554d38e9b0ed141476c1018f30d7213`  
		Last Modified: Wed, 21 Oct 2020 18:47:11 GMT  
		Size: 252.2 MB (252205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9dc1882a2c88af802357a5f4356f5ceb5f970536c3bb4d50fe18352984ca23`  
		Last Modified: Wed, 21 Oct 2020 18:46:26 GMT  
		Size: 1.6 MB (1567709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582474d5349edab8fca7176d348673c08d163a6ecbb897365dbf3b5fc7ed00b1`  
		Last Modified: Wed, 21 Oct 2020 18:46:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767055ba88f249e7d7fe3801304389ae11abaefa1ef55fcf1a1783ec477a1777`  
		Last Modified: Wed, 21 Oct 2020 18:46:26 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c555c4568bcbab87dc048a094a958b9f8cc260c417f86adf20bd4fc32e4c1c95`  
		Last Modified: Wed, 21 Oct 2020 18:46:30 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037bddd58537d4d1b7d1a3044b781f659f79c59121f22f44568ee05e631ce6c2`  
		Last Modified: Wed, 21 Oct 2020 18:46:26 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
