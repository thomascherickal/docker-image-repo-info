## `crate:latest`

```console
$ docker pull crate@sha256:45cd6ed75d65ddab683edebe810e47326411e39363935db1a086ca88c8bf70da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:6229772104eb3bf0d6c80ee29f4d7116869ea4a65034f9132bad4d3cb4f5213f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (305956753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f07c5b17951e1165b11543e01f03c959869d09924fc3a82e4993a25b5b010a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 11 Apr 2023 19:19:48 GMT
ADD file:9022dcd506469f7fa13db0072d1e4ed93f0ddf853bdd9ff02efc8d5a0345bb78 in / 
# Tue, 11 Apr 2023 19:19:49 GMT
CMD ["/bin/bash"]
# Tue, 11 Apr 2023 19:36:50 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip     && yum clean all     && rm -rf /var/cache/yum
# Tue, 11 Apr 2023 19:37:10 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.5.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.5.tar.gz.asc crate-5.2.5.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.5.tar.gz.asc     && tar -xf crate-5.2.5.tar.gz -C /crate --strip-components=1     && rm crate-5.2.5.tar.gz
# Tue, 11 Apr 2023 19:37:15 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.29.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.29.0.asc crash_standalone_0.29.0     && rm -rf "$GNUPGHOME" crash_standalone_0.29.0.asc     && mv crash_standalone_0.29.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 11 Apr 2023 19:37:15 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 11 Apr 2023 19:37:15 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 11 Apr 2023 19:37:15 GMT
RUN mkdir -p /data/data /data/log
# Tue, 11 Apr 2023 19:37:15 GMT
VOLUME [/data]
# Tue, 11 Apr 2023 19:37:15 GMT
WORKDIR /data
# Tue, 11 Apr 2023 19:37:15 GMT
EXPOSE 4200 4300 5432
# Tue, 11 Apr 2023 19:37:16 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 11 Apr 2023 19:37:16 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 11 Apr 2023 19:37:16 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-03-20T11:04:02.301203 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.5
# Tue, 11 Apr 2023 19:37:16 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 11 Apr 2023 19:37:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 Apr 2023 19:37:16 GMT
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
	-	`sha256:b7a27e8fff09ad5e02344a14d4f23ace8de5a3a9d048566cf881e870f4f7c851`  
		Last Modified: Tue, 11 Apr 2023 19:37:54 GMT  
		Size: 227.1 MB (227114609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a01f67eac00d96f75bcd51d1cca12c186023309548c70949b31697ae233a1fd`  
		Last Modified: Tue, 11 Apr 2023 19:37:36 GMT  
		Size: 1.9 MB (1857119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab43d5cce7206c61f797a11adae254c183cf01d3b88da82fc6ce3aba402b56e4`  
		Last Modified: Tue, 11 Apr 2023 19:37:35 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdccb8507578250520aecb3f6bcc23afd81b72db7417345f93618b0cc34471f6`  
		Last Modified: Tue, 11 Apr 2023 19:37:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6654086f5bff185c7cf504880a9016a0f93b4623627e1fb8431a691015ae3054`  
		Last Modified: Tue, 11 Apr 2023 19:37:35 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee8f5024ab7d5e67388701457f51ed4642d103347fd038f257ae9ba219badcc`  
		Last Modified: Tue, 11 Apr 2023 19:37:35 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

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
