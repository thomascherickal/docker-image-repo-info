## `crate:latest`

```console
$ docker pull crate@sha256:4f1f670c6cf727a470aaf67bd2191e275755351c45b5e70448a2f3a4ddb44f57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:5a3001130e20edd66ac450f93b0a89cd8d728e92b7be28e11c671747f6c49da1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331651188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8449dee790943dcec917583ed5ee6dd0c69e5eeb85cd900a03fcfc79c64ed873`
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
# Mon, 19 Jul 2021 18:03:48 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.4.tar.gz.asc crate-4.5.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.4.tar.gz.asc     && tar -xf crate-4.5.4.tar.gz -C /crate --strip-components=1     && rm crate-4.5.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 19 Jul 2021 18:03:54 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 19 Jul 2021 18:03:54 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Jul 2021 18:03:54 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 19 Jul 2021 18:03:55 GMT
RUN mkdir -p /data/data /data/log
# Mon, 19 Jul 2021 18:03:55 GMT
VOLUME [/data]
# Mon, 19 Jul 2021 18:03:55 GMT
WORKDIR /data
# Mon, 19 Jul 2021 18:03:56 GMT
EXPOSE 4200 4300 5432
# Mon, 19 Jul 2021 18:03:56 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 19 Jul 2021 18:03:56 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 19 Jul 2021 18:03:56 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-07-13T10:39:35.065268 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.4
# Mon, 19 Jul 2021 18:03:57 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 19 Jul 2021 18:03:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 19 Jul 2021 18:03:57 GMT
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
	-	`sha256:d26faa655fd49fed3d07e708ae7bec1a29186fde24bf89a194e1941252c99933`  
		Last Modified: Mon, 19 Jul 2021 18:05:01 GMT  
		Size: 254.0 MB (253967716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbeb9d95bc3495ae49d83bf1558889ec848bcb15d6e0b06542a993c0947d6eb`  
		Last Modified: Mon, 19 Jul 2021 18:04:38 GMT  
		Size: 1.6 MB (1582178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b98266a9170077e3cf44f9a2d4ca60766c636112b45b7c34bb5bb1f8ea6da0`  
		Last Modified: Mon, 19 Jul 2021 18:04:37 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc21b6725d23804c05e73932af94a09980dbe6fd6375caf05fb9c6f0730e9695`  
		Last Modified: Mon, 19 Jul 2021 18:04:37 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da8a3aef7d5903c9bc70a0c36e32d29874ce92f4a6d996f85711c41a0b5bc76`  
		Last Modified: Mon, 19 Jul 2021 18:04:38 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a592903c0c58f97497d63b64a975185eee6e8fe2593ea88bea58d5dea38747`  
		Last Modified: Mon, 19 Jul 2021 18:04:38 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:bb8e9ca2f11435f6706edbf62e8245660354068758ea3de0dd36f0b4fe971107
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360687972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61c3291a8fa6484cc36906a61c3517048eeab641da14f21d01b2440cc142e673`
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
# Mon, 19 Jul 2021 18:52:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.4.tar.gz.asc crate-4.5.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.4.tar.gz.asc     && tar -xf crate-4.5.4.tar.gz -C /crate --strip-components=1     && rm crate-4.5.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 19 Jul 2021 18:52:35 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 19 Jul 2021 18:52:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 19 Jul 2021 18:52:35 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 19 Jul 2021 18:52:36 GMT
RUN mkdir -p /data/data /data/log
# Mon, 19 Jul 2021 18:52:36 GMT
VOLUME [/data]
# Mon, 19 Jul 2021 18:52:37 GMT
WORKDIR /data
# Mon, 19 Jul 2021 18:52:37 GMT
EXPOSE 4200 4300 5432
# Mon, 19 Jul 2021 18:52:37 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 19 Jul 2021 18:52:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 19 Jul 2021 18:52:38 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-07-13T10:39:35.065268 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.4
# Mon, 19 Jul 2021 18:52:38 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 19 Jul 2021 18:52:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 19 Jul 2021 18:52:38 GMT
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
	-	`sha256:87f14e581eb6050eb5c4505c5b0d80307e71c19bda78a2568614a812739eeb74`  
		Last Modified: Mon, 19 Jul 2021 18:54:13 GMT  
		Size: 250.7 MB (250726694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5db7b36696f7346415162a2ced577f6c4521d22931b180627cd4d7513397707`  
		Last Modified: Mon, 19 Jul 2021 18:53:44 GMT  
		Size: 1.6 MB (1582188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3020f514bd0a240ec9c03386b50555e2c08239940a896ad6af81cf9afe2c944`  
		Last Modified: Mon, 19 Jul 2021 18:53:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab5368f393b3d5ccc8b6d61c2d2167a37c6a1cb4e75f57be2cae4058a3c9a0b`  
		Last Modified: Mon, 19 Jul 2021 18:53:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c09b7199b8ec9612a154658b07990209b646451da487b55237cdcb07fe1588`  
		Last Modified: Mon, 19 Jul 2021 18:53:44 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c297cc0f36d8d153006589c3c07f11e6448c7b912f1dcfe14f2a460d98014105`  
		Last Modified: Mon, 19 Jul 2021 18:53:44 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
