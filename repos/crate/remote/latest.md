## `crate:latest`

```console
$ docker pull crate@sha256:59ecf2188c9c311a9d0768c09fc722198c19a4b3fbf22db036d3dcbe0d892483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:c16df56d1e403666e3717a68723f07679f7e247ec289674530734fab78bc8354
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331203064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2740c514282ac9e80c527b5666ea40cfc6099b55e171065b1fe692b73ec714`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 00:37:20 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Sat, 14 Nov 2020 00:37:56 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.1.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.1.tar.gz.asc crate-4.3.1.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.1.tar.gz.asc     && tar -xf crate-4.3.1.tar.gz -C /crate --strip-components=1     && rm crate-4.3.1.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:38:00 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:38:00 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:38:00 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:38:01 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:38:01 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:38:01 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:38:01 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:38:02 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:38:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:38:02 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-29T10:42:21.484922 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.1
# Sat, 14 Nov 2020 00:38:02 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 14 Nov 2020 00:38:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:38:03 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51009734a299823465796326f91dc7b8be4a36f8102074b7d5682f4b160eef3d`  
		Last Modified: Sat, 14 Nov 2020 00:42:26 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd8b85af43652267039f4adde4de9aaa261ade58e36cf891d4852f8edbc378b`  
		Last Modified: Sat, 14 Nov 2020 00:42:50 GMT  
		Size: 253.5 MB (253534019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648107a4b1f2f236a1e4a269c6416711e9bb219f67adcbad406fcd41c086c097`  
		Last Modified: Sat, 14 Nov 2020 00:42:24 GMT  
		Size: 1.6 MB (1567809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d6df8e698097f16dd026fd83ff32f9f7922750fffdb1efef273796731ea61`  
		Last Modified: Sat, 14 Nov 2020 00:42:23 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3b2c9f120ba8ea49d90963414def709b092ca40ac8e3dee71e5acdd71ca55c`  
		Last Modified: Sat, 14 Nov 2020 00:42:24 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd51dba12bb261589180831438e2990ae0d8ab001e66c3898d0bf6e0624e252`  
		Last Modified: Sat, 14 Nov 2020 00:42:24 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1875cf4ee8ef67c738bfb55d090a2f0be45dd48ee0547632f6a03170bd31c72`  
		Last Modified: Sat, 14 Nov 2020 00:42:24 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:a5a2474c23dfa4b51da68483d2df8b897da748e6ace459aa93a31971d20b01da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.5 MB (360499489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1f7e0c146df5c6e81cf35d510c3e744ba0279519ba29e3aa619a3f1e8989e8a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Sat, 14 Nov 2020 00:40:26 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Sat, 14 Nov 2020 00:40:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:40:32 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 00:57:11 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 01 Dec 2020 22:44:53 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.2.tar.gz.asc crate-4.3.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.2.tar.gz.asc     && tar -xf crate-4.3.2.tar.gz -C /crate --strip-components=1     && rm crate-4.3.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 01 Dec 2020 22:45:00 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 01 Dec 2020 22:45:00 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Dec 2020 22:45:01 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 01 Dec 2020 22:45:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 01 Dec 2020 22:45:04 GMT
VOLUME [/data]
# Tue, 01 Dec 2020 22:45:05 GMT
WORKDIR /data
# Tue, 01 Dec 2020 22:45:05 GMT
EXPOSE 4200 4300 5432
# Tue, 01 Dec 2020 22:45:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 01 Dec 2020 22:45:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 01 Dec 2020 22:45:07 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-11-25T09:57:46.817607 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.2
# Tue, 01 Dec 2020 22:45:08 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 01 Dec 2020 22:45:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Dec 2020 22:45:09 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6312a055314d3cb5a347fd7eb62a5fb7ad8e03a999e1c964f320a28325cf017d`  
		Last Modified: Sat, 14 Nov 2020 01:06:26 GMT  
		Size: 2.3 KB (2254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a657c4f9dea343008e5dd9d105ca14a17753b001a65979d508804fe6a42f45`  
		Last Modified: Tue, 01 Dec 2020 22:46:31 GMT  
		Size: 250.6 MB (250552619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d0b62ccf8e1ade248fb25c961ce7d338e49981b524b6698368e36e3f08f389`  
		Last Modified: Tue, 01 Dec 2020 22:45:52 GMT  
		Size: 1.6 MB (1567788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8b3cb92ea8a107fdb9297a6a043d91cba012f367597e6b6f3f2b290c569144`  
		Last Modified: Tue, 01 Dec 2020 22:45:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c1654c31351f24a47957497ba49533a3873e474b7bb213a6969b53e09b764a`  
		Last Modified: Tue, 01 Dec 2020 22:45:52 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1177133152c5c9607e98febf24cdb3cb960297766fb8f166910df5899efc7bf0`  
		Last Modified: Tue, 01 Dec 2020 22:45:52 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62907543f65de299cb36dda41408cd0a7ab2adb92a2d90029b42c828c396346f`  
		Last Modified: Tue, 01 Dec 2020 22:45:52 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
