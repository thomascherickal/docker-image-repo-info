## `crate:latest`

```console
$ docker pull crate@sha256:3da07c527a85a3c3f33f58ec3c1b8d5f35ba21f8c7dc680ebb249a14de2e777f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:a6fbf5c3362a2382407a66038062774ce5a801fb877f08830b675c40ef146c0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.1 MB (374137395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e7de268aa412ee75cd4a38650f7dd9cf080500cf54a54b4a1ff3af6705d8ba`
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
# Tue, 07 Feb 2023 02:30:22 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.1.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.1.4.tar.gz.asc crate-5.1.4.tar.gz     && rm -rf "$GNUPGHOME" crate-5.1.4.tar.gz.asc     && tar -xf crate-5.1.4.tar.gz -C /crate --strip-components=1     && rm crate-5.1.4.tar.gz
# Tue, 07 Feb 2023 02:30:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 07 Feb 2023 02:30:25 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 02:30:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 07 Feb 2023 02:30:26 GMT
RUN mkdir -p /data/data /data/log
# Tue, 07 Feb 2023 02:30:26 GMT
VOLUME [/data]
# Tue, 07 Feb 2023 02:30:26 GMT
WORKDIR /data
# Tue, 07 Feb 2023 02:30:26 GMT
EXPOSE 4200 4300 5432
# Tue, 07 Feb 2023 02:30:26 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 07 Feb 2023 02:30:26 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 07 Feb 2023 02:30:27 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-01T11:51:38.179251 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.1.4
# Tue, 07 Feb 2023 02:30:27 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 07 Feb 2023 02:30:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:30:27 GMT
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
	-	`sha256:058d69f0b9f069da294c8c8fa7d2f042723e5e3548932cd7f56e0b3300b52d69`  
		Last Modified: Tue, 07 Feb 2023 02:31:03 GMT  
		Size: 219.2 MB (219178229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208da7a8dc8bd96bbc524f06e5a4e8d1563995381d18fa5c175330d33ccc00e`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 1.7 MB (1710774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499754ae1fbf828294712397babe49c2ffb3671a90ef0e7011ec7a38c886c4d4`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701e5b0271c83b7daa100db79d3112c4b763a49dc52bd12ecf3df1289868e72`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f33d26a8afba44a242aef0966df625ad34a1cc88e71e46052ec441c9ada3da`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855ef2f7003b260cb8f7c7c19110870792e2216ef7675eaf6b813633ee9aea2`  
		Last Modified: Tue, 07 Feb 2023 02:30:44 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:5b2e929107f55d21365def6d734307dcdd31714bf0c63b4b6bc8f0e83fb4e8d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303285150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f9acd1d081659754bb38c2418066dfa328033dc8a7a43b65d221a26a50da81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Thu, 01 Dec 2022 23:39:35 GMT
ADD file:5066d79f89826364c29600221a8a14ee92e24325124c2b3bcebc4800255d09fa in / 
# Thu, 01 Dec 2022 23:39:38 GMT
CMD ["/bin/bash"]
# Mon, 13 Feb 2023 20:56:07 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python3 python3-pip openssl     && yum clean all     && rm -rf /var/cache/yum
# Mon, 13 Feb 2023 20:56:29 GMT
RUN groupadd crate     && useradd -u 1000 -g crate -d /crate crate     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-5.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-5.2.2.tar.gz.asc crate-5.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-5.2.2.tar.gz.asc     && tar -xf crate-5.2.2.tar.gz -C /crate --strip-components=1     && rm crate-5.2.2.tar.gz
# Mon, 13 Feb 2023 20:56:33 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.28.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.28.0.asc crash_standalone_0.28.0     && rm -rf "$GNUPGHOME" crash_standalone_0.28.0.asc     && mv crash_standalone_0.28.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 13 Feb 2023 20:56:33 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 20:56:34 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 13 Feb 2023 20:56:34 GMT
RUN mkdir -p /data/data /data/log
# Mon, 13 Feb 2023 20:56:34 GMT
VOLUME [/data]
# Mon, 13 Feb 2023 20:56:34 GMT
WORKDIR /data
# Mon, 13 Feb 2023 20:56:34 GMT
EXPOSE 4200 4300 5432
# Mon, 13 Feb 2023 20:56:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 13 Feb 2023 20:56:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 13 Feb 2023 20:56:35 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2023-02-09T10:53:55.573437 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database that handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=5.2.2
# Mon, 13 Feb 2023 20:56:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 13 Feb 2023 20:56:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 13 Feb 2023 20:56:35 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:2f298c8213b4208e3cf11c6fc574ad8188419f93f66d4a9f309c6f9db7d5cfac`  
		Last Modified: Thu, 01 Dec 2022 23:40:54 GMT  
		Size: 68.3 MB (68271371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0dc101c5d7fdd87b674f35dd61171ab35ce1e181e83b3b900bebe0ecbfb0c8`  
		Last Modified: Mon, 13 Feb 2023 20:56:56 GMT  
		Size: 7.4 MB (7444733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd52155b7ff738e3a8e96a73a0ddc0f97d7fa10d5ad3ee52bf79bb3e81658b`  
		Last Modified: Mon, 13 Feb 2023 20:57:09 GMT  
		Size: 225.9 MB (225857811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143817de359039a548a45c60ece7d0e3ff642b7b8f6f4f465e2b66b1f369f408`  
		Last Modified: Mon, 13 Feb 2023 20:56:53 GMT  
		Size: 1.7 MB (1709348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386586f3357031383f6631dcc7909fb692ec04e98cd122b98562c55a9af11a6`  
		Last Modified: Mon, 13 Feb 2023 20:56:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355245f499fe631e037376ceae12bb33489f3bb8ef6df214593a30b78b980249`  
		Last Modified: Mon, 13 Feb 2023 20:56:52 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7000fc3c20c014ed344717dc4243db4e68843b162b420eb9203341442ead08fa`  
		Last Modified: Mon, 13 Feb 2023 20:56:52 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acb119d6273d8e1fa809b66ead32cf434fc7f7b723112008d6dd2b77b5cff19`  
		Last Modified: Mon, 13 Feb 2023 20:56:52 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
