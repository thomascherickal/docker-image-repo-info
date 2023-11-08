## `crate:latest`

```console
$ docker pull crate@sha256:6991d5b1920bfca98521fb57cf05608300de220e08c136488d503900aaa6fcdf
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
$ docker pull crate@sha256:f7bdc90e17b14814195ac43682449518117a6249170900f2771941f0ba114c20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.1 MB (185144928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3a9407e467c8f850adb70e72c8b63613e1aa6e11f3e8a7f63fc69ba2ce44e61`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 18 Jul 2023 19:39:39 GMT
ADD file:40800ee585298348133157273f601922b26aea5ea4e21cd03223a28d6bb24c71 in / 
# Tue, 18 Jul 2023 19:39:41 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 19:44:21 GMT
RUN dnf install --nodocs --assumeyes gzip python3 shadow-utils tar     && dnf clean all     && rm -rf /var/cache/yum
# Tue, 07 Nov 2023 23:41:20 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.5.0.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.5.0.tar.gz.asc crate-5.5.0.tar.gz     && rm -rf "$GNUPGHOME" crate-5.5.0.tar.gz.asc     && tar -xf crate-5.5.0.tar.gz -C /crate --strip-components=1     && rm crate-5.5.0.tar.gz
# Tue, 07 Nov 2023 23:41:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.30.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.30.0.asc crash_standalone_0.30.0     && rm -rf "$GNUPGHOME" crash_standalone_0.30.0.asc     && mv crash_standalone_0.30.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 07 Nov 2023 23:41:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 23:41:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 07 Nov 2023 23:41:23 GMT
RUN mkdir -p /data/data /data/log
# Tue, 07 Nov 2023 23:41:23 GMT
VOLUME [/data]
# Tue, 07 Nov 2023 23:41:23 GMT
WORKDIR /data
# Tue, 07 Nov 2023 23:41:23 GMT
EXPOSE 4200 4300 5432
# Tue, 07 Nov 2023 23:41:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 07 Nov 2023 23:41:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 07 Nov 2023 23:41:24 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-10-27T11:44:30.874801 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.5.0
# Tue, 07 Nov 2023 23:41:24 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 07 Nov 2023 23:41:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Nov 2023 23:41:24 GMT
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
	-	`sha256:cf94576c99f51e9c62662751debdf3f5383d5ac56fec1bd4d4747a2119b157f6`  
		Last Modified: Tue, 07 Nov 2023 23:41:54 GMT  
		Size: 115.7 MB (115660898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495053ac8d57db97cb37eb17c3e0601622b5729c820a23b93ecbff383bc88f5b`  
		Last Modified: Tue, 07 Nov 2023 23:41:45 GMT  
		Size: 1.9 MB (1931734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc65cf876257bd2a4f10f65897a384ce48509ddb32c4cec4014f566c19f2b6ab`  
		Last Modified: Tue, 07 Nov 2023 23:41:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5024873c58b2747b373f92293083e0d0300727202c092a92e58ae2c49d9dd2b`  
		Last Modified: Tue, 07 Nov 2023 23:41:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb22bf4ff5353eb85278f5a038d06f16d4b573c6fa415d158141f61ee621797`  
		Last Modified: Tue, 07 Nov 2023 23:41:44 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd8d7821baca63474fb712d3de5328375f31ba154dd1e1f987346a94e06783b`  
		Last Modified: Tue, 07 Nov 2023 23:41:44 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
