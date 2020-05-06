<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:3.3`](#crate33)
-	[`crate:3.3.5`](#crate335)
-	[`crate:4.0`](#crate40)
-	[`crate:4.0.12`](#crate4012)
-	[`crate:4.1`](#crate41)
-	[`crate:4.1.5`](#crate415)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:01ce15f2d819d2cdf5cdc9bcfff1dc4909d84d3d0e3f24db5ac3d16d170287f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:3.3` - linux; amd64

```console
$ docker pull crate@sha256:bc213e835be53508430a1f157ee699bcf54a432607bce65fb844e6e566b4d858
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344600898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffdffa6ef9a8658a7324eeff8c286b82e03fc56f987b246f3b7b7a0fb913b66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:50:37 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:50:37 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Tue, 05 May 2020 21:50:38 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:51:40 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:51:41 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:51:41 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:51:42 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:51:42 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:51:42 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:51:43 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:51:43 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:51:44 GMT
WORKDIR /data
# Tue, 05 May 2020 21:51:44 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:51:44 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:51:44 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:51:44 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2019-07-08T14:08:18.187344 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Tue, 05 May 2020 21:51:45 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:51:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:51:45 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5490c6a45b293946f1d5b6262e6c798629e9697bc9f29c96a280523c3f9cf451`  
		Last Modified: Tue, 05 May 2020 21:53:57 GMT  
		Size: 188.1 MB (188101303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dc1551b1c741bea84a3b20478e07bf46bdbac5d74d7474d5531803fc946733`  
		Last Modified: Tue, 05 May 2020 21:53:37 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b77b95d7651359c976797d8822429d25c8e3abcf6cd146f10810fd20e692afc`  
		Last Modified: Tue, 05 May 2020 21:53:49 GMT  
		Size: 79.3 MB (79319889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4615ed3f5dd1ee4846082b3a4ad8d2f20387a25d23df1c6426690ce231f92913`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9fa2991329aeaacc7c56af713735158cf01e86d3d0dae4f0aa45deb2c86903`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be31358e83a1a897db44a05cf143ed2282bade6d6f735ee6e59f459a11b34715`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 1.3 MB (1294037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd06d0ec6dbb07f4694547266227e70536319f321227b89fd476c8705e939361`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d42a263c58d8f6752153208bd4ca699443841b72171d337f7b4cc59c78c44a`  
		Last Modified: Tue, 05 May 2020 21:53:35 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b8bbd438475fb1c06925cf8983858b4eb9b5525e9b6a3fa113c41f69939d78`  
		Last Modified: Tue, 05 May 2020 21:53:35 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e68877c347eab8a1be098a80f32ea60b912a03921bcc29a5a682881bd38c`  
		Last Modified: Tue, 05 May 2020 21:53:35 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:3.3.5`

```console
$ docker pull crate@sha256:01ce15f2d819d2cdf5cdc9bcfff1dc4909d84d3d0e3f24db5ac3d16d170287f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:3.3.5` - linux; amd64

```console
$ docker pull crate@sha256:bc213e835be53508430a1f157ee699bcf54a432607bce65fb844e6e566b4d858
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344600898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ffdffa6ef9a8658a7324eeff8c286b82e03fc56f987b246f3b7b7a0fb913b66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:50:37 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:50:37 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Tue, 05 May 2020 21:50:38 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:51:40 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:51:41 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:51:41 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:51:42 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:51:42 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:51:42 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:51:43 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:51:43 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:51:44 GMT
WORKDIR /data
# Tue, 05 May 2020 21:51:44 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:51:44 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:51:44 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:51:44 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2019-07-08T14:08:18.187344 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Tue, 05 May 2020 21:51:45 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:51:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:51:45 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5490c6a45b293946f1d5b6262e6c798629e9697bc9f29c96a280523c3f9cf451`  
		Last Modified: Tue, 05 May 2020 21:53:57 GMT  
		Size: 188.1 MB (188101303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dc1551b1c741bea84a3b20478e07bf46bdbac5d74d7474d5531803fc946733`  
		Last Modified: Tue, 05 May 2020 21:53:37 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b77b95d7651359c976797d8822429d25c8e3abcf6cd146f10810fd20e692afc`  
		Last Modified: Tue, 05 May 2020 21:53:49 GMT  
		Size: 79.3 MB (79319889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4615ed3f5dd1ee4846082b3a4ad8d2f20387a25d23df1c6426690ce231f92913`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9fa2991329aeaacc7c56af713735158cf01e86d3d0dae4f0aa45deb2c86903`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be31358e83a1a897db44a05cf143ed2282bade6d6f735ee6e59f459a11b34715`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 1.3 MB (1294037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd06d0ec6dbb07f4694547266227e70536319f321227b89fd476c8705e939361`  
		Last Modified: Tue, 05 May 2020 21:53:36 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d42a263c58d8f6752153208bd4ca699443841b72171d337f7b4cc59c78c44a`  
		Last Modified: Tue, 05 May 2020 21:53:35 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b8bbd438475fb1c06925cf8983858b4eb9b5525e9b6a3fa113c41f69939d78`  
		Last Modified: Tue, 05 May 2020 21:53:35 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e68877c347eab8a1be098a80f32ea60b912a03921bcc29a5a682881bd38c`  
		Last Modified: Tue, 05 May 2020 21:53:35 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0`

```console
$ docker pull crate@sha256:640ea4196161236c3866d0672422d6ddb8c1bbc8bbd0f310363973217ae59c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0` - linux; amd64

```console
$ docker pull crate@sha256:4837c6da4b5c5c3275cd285f579be8ce146396c2c82b37c186ce62d0068aca89
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.2 MB (352203982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32151101857e336ab156656a9eff5c4f832c37964ae4c812033fcdf3274de84`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:48:40 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:48:40 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Tue, 05 May 2020 21:48:41 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:49:44 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:49:44 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:49:44 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:49:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:49:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:49:46 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:49:47 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:49:47 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:49:48 GMT
WORKDIR /data
# Tue, 05 May 2020 21:49:48 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:49:48 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:49:48 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:49:48 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Tue, 05 May 2020 21:49:49 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:49:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:49:49 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb45862ffabfdd79413ec3bb7d15be9ff59341ef2086195301b3f977338e5e`  
		Last Modified: Tue, 05 May 2020 21:53:31 GMT  
		Size: 198.1 MB (198127878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846496d1bced69e7973a5fe3f7f492750ffb7587c337135bd370e8917bbd5de9`  
		Last Modified: Tue, 05 May 2020 21:52:54 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ae04b96ae3bffe1394ce27d6e376913e5596881c20d7300caf6bcdaf01c49`  
		Last Modified: Tue, 05 May 2020 21:53:03 GMT  
		Size: 76.9 MB (76896391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0c2920d7c3ef39a82e56fcda9c14acf6b500bfdd0c8b136283a77fa7c2aee3`  
		Last Modified: Tue, 05 May 2020 21:52:54 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673b4bfbf1cba16f55a8f3fe7d79112febfcb53e932508a0d7a3bd7075d5c1fc`  
		Last Modified: Tue, 05 May 2020 21:52:53 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d4be2ab567364a35c8df526e0ad95fd62ca2b4ca6a99f4727562c3e788798c`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 1.3 MB (1294038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bb2b53c359dc1bf0f66ea5a1a36740470116a7b06c7ab3bb3ef4a246b3bc5e`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e8fc437796c9a4fba95a8a38282c290fc6ce5bce0d81a77a91d578bf446b6c`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed00125532c4a2a04ede93ffce6f27f09484ed5ab79de5e0fc916d9cb6f926e`  
		Last Modified: Tue, 05 May 2020 21:52:53 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dce78cc18bf63ee49f18128dad0daac190689f4a97bea9fb4092611fa78e20`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.0` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:e118d911bb6676e8f755c3155e6886f857e135c5486476b5ec0a369d5da5cc5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.7 MB (363698128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8060a6550b848abc4d9d65ac3b3161245cec73dc66a93c267b2386d0ee699f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:40:03 GMT
ADD file:8449a578596d0a7b4ce64f74355f602ee47b1a8782058356ae614cdcdf4639fb in / 
# Tue, 12 Nov 2019 00:40:05 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:40:06 GMT
CMD ["/bin/bash"]
# Wed, 05 Feb 2020 23:45:29 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 05 Feb 2020 23:47:30 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 05 Feb 2020 23:47:32 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Wed, 05 Feb 2020 23:47:34 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Fri, 07 Feb 2020 17:41:10 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Fri, 07 Feb 2020 17:41:11 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 07 Feb 2020 17:41:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 07 Feb 2020 17:41:15 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 07 Feb 2020 17:41:16 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 17:41:16 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 07 Feb 2020 17:41:18 GMT
RUN mkdir -p /data/data /data/log
# Fri, 07 Feb 2020 17:41:19 GMT
VOLUME [/data]
# Fri, 07 Feb 2020 17:41:20 GMT
WORKDIR /data
# Fri, 07 Feb 2020 17:41:20 GMT
EXPOSE 4200 4300 5432
# Fri, 07 Feb 2020 17:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 07 Feb 2020 17:41:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 07 Feb 2020 17:41:23 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Fri, 07 Feb 2020 17:41:23 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Fri, 07 Feb 2020 17:41:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 17:41:24 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:3f2696f8166ff69dd0c116674b19eebd351ed3fc4111a42dbd57c673601c725d`  
		Last Modified: Tue, 12 Nov 2019 00:40:46 GMT  
		Size: 103.6 MB (103619629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e11d48e7bd36dbc63110f197eefe11eb9a4f505370153c386e5938d14144b04`  
		Last Modified: Fri, 07 Feb 2020 17:42:20 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d7b3ef51b7bd60dec3d95f5c374a06e5bfe6d4ab1036a515cd905087c808f4`  
		Last Modified: Fri, 07 Feb 2020 17:42:56 GMT  
		Size: 198.1 MB (198127621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f4b8359b5803a8811af6a9b3523cbbdb0539445653cde4a98c549725f01969`  
		Last Modified: Fri, 07 Feb 2020 17:42:18 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb893855b5eef69ef93742a1a48a5b60fa245554da64c848ead80bcb8e4850`  
		Last Modified: Fri, 07 Feb 2020 17:42:26 GMT  
		Size: 60.7 MB (60651217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c9d0dbd3792de4cce6d472b5db0ca3f5c73d1afb6a474af88dfcf68e6cbfa4`  
		Last Modified: Fri, 07 Feb 2020 17:42:17 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c100f39ea29d146ba57133e818a7fee1153a4cd39f76103a8a83f933f725a30f`  
		Last Modified: Fri, 07 Feb 2020 17:42:17 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f304c3ddc63be0bd0a99be8ae60b8e50a792e61fe6cc754bb8e6e6da6f52f01`  
		Last Modified: Fri, 07 Feb 2020 17:42:18 GMT  
		Size: 1.3 MB (1294054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a3248827130dd0cdc6b3b750e99b024a6a51729dee9a5591300aa6063297d`  
		Last Modified: Fri, 07 Feb 2020 17:42:15 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52932d778d0ee38e9b36356b3d8a01520b370e8abcb7197a856b4f0792766a0`  
		Last Modified: Fri, 07 Feb 2020 17:42:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318e47c7046282f67573507dda274463a83b438e1fdb863bf3d1cfc3e990e78e`  
		Last Modified: Fri, 07 Feb 2020 17:42:15 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a00a7999f820e847e47c48a4bddf9911b2f353d78b944cb2eb350d520c5eab0`  
		Last Modified: Fri, 07 Feb 2020 17:42:16 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0.12`

```console
$ docker pull crate@sha256:640ea4196161236c3866d0672422d6ddb8c1bbc8bbd0f310363973217ae59c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0.12` - linux; amd64

```console
$ docker pull crate@sha256:4837c6da4b5c5c3275cd285f579be8ce146396c2c82b37c186ce62d0068aca89
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.2 MB (352203982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32151101857e336ab156656a9eff5c4f832c37964ae4c812033fcdf3274de84`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:48:40 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:48:40 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Tue, 05 May 2020 21:48:41 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:49:44 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:49:44 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:49:44 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:49:46 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:49:46 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:49:46 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:49:47 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:49:47 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:49:48 GMT
WORKDIR /data
# Tue, 05 May 2020 21:49:48 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:49:48 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:49:48 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:49:48 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Tue, 05 May 2020 21:49:49 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:49:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:49:49 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb45862ffabfdd79413ec3bb7d15be9ff59341ef2086195301b3f977338e5e`  
		Last Modified: Tue, 05 May 2020 21:53:31 GMT  
		Size: 198.1 MB (198127878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846496d1bced69e7973a5fe3f7f492750ffb7587c337135bd370e8917bbd5de9`  
		Last Modified: Tue, 05 May 2020 21:52:54 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ae04b96ae3bffe1394ce27d6e376913e5596881c20d7300caf6bcdaf01c49`  
		Last Modified: Tue, 05 May 2020 21:53:03 GMT  
		Size: 76.9 MB (76896391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0c2920d7c3ef39a82e56fcda9c14acf6b500bfdd0c8b136283a77fa7c2aee3`  
		Last Modified: Tue, 05 May 2020 21:52:54 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673b4bfbf1cba16f55a8f3fe7d79112febfcb53e932508a0d7a3bd7075d5c1fc`  
		Last Modified: Tue, 05 May 2020 21:52:53 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d4be2ab567364a35c8df526e0ad95fd62ca2b4ca6a99f4727562c3e788798c`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 1.3 MB (1294038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bb2b53c359dc1bf0f66ea5a1a36740470116a7b06c7ab3bb3ef4a246b3bc5e`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e8fc437796c9a4fba95a8a38282c290fc6ce5bce0d81a77a91d578bf446b6c`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed00125532c4a2a04ede93ffce6f27f09484ed5ab79de5e0fc916d9cb6f926e`  
		Last Modified: Tue, 05 May 2020 21:52:53 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dce78cc18bf63ee49f18128dad0daac190689f4a97bea9fb4092611fa78e20`  
		Last Modified: Tue, 05 May 2020 21:52:52 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.0.12` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:e118d911bb6676e8f755c3155e6886f857e135c5486476b5ec0a369d5da5cc5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.7 MB (363698128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8060a6550b848abc4d9d65ac3b3161245cec73dc66a93c267b2386d0ee699f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:40:03 GMT
ADD file:8449a578596d0a7b4ce64f74355f602ee47b1a8782058356ae614cdcdf4639fb in / 
# Tue, 12 Nov 2019 00:40:05 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:40:06 GMT
CMD ["/bin/bash"]
# Wed, 05 Feb 2020 23:45:29 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 05 Feb 2020 23:47:30 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 05 Feb 2020 23:47:32 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Wed, 05 Feb 2020 23:47:34 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Fri, 07 Feb 2020 17:41:10 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Fri, 07 Feb 2020 17:41:11 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 07 Feb 2020 17:41:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 07 Feb 2020 17:41:15 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 07 Feb 2020 17:41:16 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 17:41:16 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 07 Feb 2020 17:41:18 GMT
RUN mkdir -p /data/data /data/log
# Fri, 07 Feb 2020 17:41:19 GMT
VOLUME [/data]
# Fri, 07 Feb 2020 17:41:20 GMT
WORKDIR /data
# Fri, 07 Feb 2020 17:41:20 GMT
EXPOSE 4200 4300 5432
# Fri, 07 Feb 2020 17:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 07 Feb 2020 17:41:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 07 Feb 2020 17:41:23 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Fri, 07 Feb 2020 17:41:23 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Fri, 07 Feb 2020 17:41:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 17:41:24 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:3f2696f8166ff69dd0c116674b19eebd351ed3fc4111a42dbd57c673601c725d`  
		Last Modified: Tue, 12 Nov 2019 00:40:46 GMT  
		Size: 103.6 MB (103619629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e11d48e7bd36dbc63110f197eefe11eb9a4f505370153c386e5938d14144b04`  
		Last Modified: Fri, 07 Feb 2020 17:42:20 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d7b3ef51b7bd60dec3d95f5c374a06e5bfe6d4ab1036a515cd905087c808f4`  
		Last Modified: Fri, 07 Feb 2020 17:42:56 GMT  
		Size: 198.1 MB (198127621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f4b8359b5803a8811af6a9b3523cbbdb0539445653cde4a98c549725f01969`  
		Last Modified: Fri, 07 Feb 2020 17:42:18 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb893855b5eef69ef93742a1a48a5b60fa245554da64c848ead80bcb8e4850`  
		Last Modified: Fri, 07 Feb 2020 17:42:26 GMT  
		Size: 60.7 MB (60651217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c9d0dbd3792de4cce6d472b5db0ca3f5c73d1afb6a474af88dfcf68e6cbfa4`  
		Last Modified: Fri, 07 Feb 2020 17:42:17 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c100f39ea29d146ba57133e818a7fee1153a4cd39f76103a8a83f933f725a30f`  
		Last Modified: Fri, 07 Feb 2020 17:42:17 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f304c3ddc63be0bd0a99be8ae60b8e50a792e61fe6cc754bb8e6e6da6f52f01`  
		Last Modified: Fri, 07 Feb 2020 17:42:18 GMT  
		Size: 1.3 MB (1294054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a3248827130dd0cdc6b3b750e99b024a6a51729dee9a5591300aa6063297d`  
		Last Modified: Fri, 07 Feb 2020 17:42:15 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52932d778d0ee38e9b36356b3d8a01520b370e8abcb7197a856b4f0792766a0`  
		Last Modified: Fri, 07 Feb 2020 17:42:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318e47c7046282f67573507dda274463a83b438e1fdb863bf3d1cfc3e990e78e`  
		Last Modified: Fri, 07 Feb 2020 17:42:15 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a00a7999f820e847e47c48a4bddf9911b2f353d78b944cb2eb350d520c5eab0`  
		Last Modified: Fri, 07 Feb 2020 17:42:16 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1`

```console
$ docker pull crate@sha256:edfaf333d29ac809d71952b06c0654e1ff771c5e2e67c8062f8da0fc8fc2bb47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1` - linux; amd64

```console
$ docker pull crate@sha256:6d051a73c9ea33554c21fcf05e4e8a9ebc63304ac2c55077597cd75cf0db7313
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351169100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f52c09a2c68171d4426b3283ac9adb21320d08150c8c272d2a8eb69bb5554ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:47:21 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:47:22 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 05 May 2020 21:47:22 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:47:44 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.5.tar.gz.asc crate-4.1.5.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.5.tar.gz.asc     && tar -xf crate-4.1.5.tar.gz -C /crate --strip-components=1     && rm crate-4.1.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:47:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:47:47 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:47:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:47:48 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:47:48 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:47:48 GMT
WORKDIR /data
# Tue, 05 May 2020 21:47:49 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:47:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:47:49 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:47:49 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-04-24T09:34:17.477377 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.5
# Tue, 05 May 2020 21:47:49 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:47:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:47:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f1387b5ba8366a3891b3e1a0fed1418b2ad7e5acab59d784d711197333efe1`  
		Last Modified: Tue, 05 May 2020 21:52:48 GMT  
		Size: 196.4 MB (196423143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8301c448e63bb7d27fe72ed07696cfe892e51828e96684cf475a17360cbdbc`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95b33f6df2f0a1079d1fcc203dc695a3ca044292e5752851187302493e6a494`  
		Last Modified: Tue, 05 May 2020 21:52:04 GMT  
		Size: 77.6 MB (77567470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78afef4592f2681f29a90e2e0c782ed6397088dde7e0386e0428cc3f963d05af`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 1.3 MB (1294033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ae7ca8b418576838b672b1c5e9d2433957aa11be7b3530f227d9ce3949dfc8`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81e06b30d48695b06b680e862fa3260ecb75167d7ef8632fa9278cc6fe7d2d3`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f010083d8abab3d444dec5fad2bde0ebf144ae53d9d00b29f1190115e39f6907`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44cf5112b81e9cea56e5be0def3d8a484ac3dd16d67b01858099f205f3ce1c1`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:41dcfdb2c440f1e9259471537c1fe98073d02665d043cb6c9a59df93437c14d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.3 MB (378290980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f01df573ee22342b92e20cb3d41c13ded585d78393e7bb95f1e962a8df8b97`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:41:25 GMT
ADD file:d64254c17612e9076d442240e4e567c0467ab6c4ca282ba5553f602805ad89ac in / 
# Tue, 05 May 2020 21:41:30 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:41:31 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:57:47 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:58:08 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:58:10 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 05 May 2020 21:58:11 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:58:41 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.5.tar.gz.asc crate-4.1.5.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.5.tar.gz.asc     && tar -xf crate-4.1.5.tar.gz -C /crate --strip-components=1     && rm crate-4.1.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:58:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:58:47 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:58:48 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:58:49 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:58:50 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:58:51 GMT
WORKDIR /data
# Tue, 05 May 2020 21:58:51 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:58:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:58:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:58:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-04-24T09:34:17.477377 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.5
# Tue, 05 May 2020 21:58:54 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:58:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:58:55 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ae60b79047f8473e02511e923f461b869b62d2bf110b9fa282656e9f0128932d`  
		Last Modified: Tue, 05 May 2020 21:42:11 GMT  
		Size: 104.6 MB (104555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cbdaa35d65e895b1f8cdcdae19714a1be917bbc2886d43605e27eea7c5016d`  
		Last Modified: Tue, 05 May 2020 22:01:46 GMT  
		Size: 2.2 KB (2248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4da918b90a19f31a2065118c658cefcb9e13af76a45daa0742673eb7067147`  
		Last Modified: Tue, 05 May 2020 22:02:17 GMT  
		Size: 196.4 MB (196423275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1563ebec551778313976636e734e51d8a4f4d4a96766b78a310c0602da3b64d4`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2af2046d4e2bb9e4f6f09c988d9b62fed090dc05b007b41fa3716313c6043`  
		Last Modified: Tue, 05 May 2020 22:01:59 GMT  
		Size: 76.0 MB (76013928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bc82dfaa3cf5b669a81b57a4f36b2fa63491c85ed7c5fac622ee1fb25eeba8`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 1.3 MB (1294032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438726e25f92144a78f953c5663373fcaac4a7698b553b9c60f0a528727d3ab`  
		Last Modified: Tue, 05 May 2020 22:01:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd46551fd135778e1f30daeaed384bb140cfcd0ec5223e1205796319f362ff4`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d2ced395addf9dfd75088358f126f0639fecee4baa04232593bfef4c1ca224`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8a338b3cd6e0522d30c4bfc660c99839f0ae56389eed3baafac8904aad25cb`  
		Last Modified: Tue, 05 May 2020 22:01:43 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1.5`

```console
$ docker pull crate@sha256:edfaf333d29ac809d71952b06c0654e1ff771c5e2e67c8062f8da0fc8fc2bb47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1.5` - linux; amd64

```console
$ docker pull crate@sha256:6d051a73c9ea33554c21fcf05e4e8a9ebc63304ac2c55077597cd75cf0db7313
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351169100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f52c09a2c68171d4426b3283ac9adb21320d08150c8c272d2a8eb69bb5554ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:47:21 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:47:22 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 05 May 2020 21:47:22 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:47:44 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.5.tar.gz.asc crate-4.1.5.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.5.tar.gz.asc     && tar -xf crate-4.1.5.tar.gz -C /crate --strip-components=1     && rm crate-4.1.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:47:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:47:47 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:47:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:47:48 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:47:48 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:47:48 GMT
WORKDIR /data
# Tue, 05 May 2020 21:47:49 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:47:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:47:49 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:47:49 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-04-24T09:34:17.477377 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.5
# Tue, 05 May 2020 21:47:49 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:47:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:47:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f1387b5ba8366a3891b3e1a0fed1418b2ad7e5acab59d784d711197333efe1`  
		Last Modified: Tue, 05 May 2020 21:52:48 GMT  
		Size: 196.4 MB (196423143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8301c448e63bb7d27fe72ed07696cfe892e51828e96684cf475a17360cbdbc`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95b33f6df2f0a1079d1fcc203dc695a3ca044292e5752851187302493e6a494`  
		Last Modified: Tue, 05 May 2020 21:52:04 GMT  
		Size: 77.6 MB (77567470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78afef4592f2681f29a90e2e0c782ed6397088dde7e0386e0428cc3f963d05af`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 1.3 MB (1294033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ae7ca8b418576838b672b1c5e9d2433957aa11be7b3530f227d9ce3949dfc8`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81e06b30d48695b06b680e862fa3260ecb75167d7ef8632fa9278cc6fe7d2d3`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f010083d8abab3d444dec5fad2bde0ebf144ae53d9d00b29f1190115e39f6907`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44cf5112b81e9cea56e5be0def3d8a484ac3dd16d67b01858099f205f3ce1c1`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:41dcfdb2c440f1e9259471537c1fe98073d02665d043cb6c9a59df93437c14d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.3 MB (378290980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f01df573ee22342b92e20cb3d41c13ded585d78393e7bb95f1e962a8df8b97`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:41:25 GMT
ADD file:d64254c17612e9076d442240e4e567c0467ab6c4ca282ba5553f602805ad89ac in / 
# Tue, 05 May 2020 21:41:30 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:41:31 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:57:47 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:58:08 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:58:10 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 05 May 2020 21:58:11 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:58:41 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.5.tar.gz.asc crate-4.1.5.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.5.tar.gz.asc     && tar -xf crate-4.1.5.tar.gz -C /crate --strip-components=1     && rm crate-4.1.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:58:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:58:47 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:58:48 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:58:49 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:58:50 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:58:51 GMT
WORKDIR /data
# Tue, 05 May 2020 21:58:51 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:58:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:58:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:58:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-04-24T09:34:17.477377 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.5
# Tue, 05 May 2020 21:58:54 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:58:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:58:55 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ae60b79047f8473e02511e923f461b869b62d2bf110b9fa282656e9f0128932d`  
		Last Modified: Tue, 05 May 2020 21:42:11 GMT  
		Size: 104.6 MB (104555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cbdaa35d65e895b1f8cdcdae19714a1be917bbc2886d43605e27eea7c5016d`  
		Last Modified: Tue, 05 May 2020 22:01:46 GMT  
		Size: 2.2 KB (2248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4da918b90a19f31a2065118c658cefcb9e13af76a45daa0742673eb7067147`  
		Last Modified: Tue, 05 May 2020 22:02:17 GMT  
		Size: 196.4 MB (196423275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1563ebec551778313976636e734e51d8a4f4d4a96766b78a310c0602da3b64d4`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2af2046d4e2bb9e4f6f09c988d9b62fed090dc05b007b41fa3716313c6043`  
		Last Modified: Tue, 05 May 2020 22:01:59 GMT  
		Size: 76.0 MB (76013928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bc82dfaa3cf5b669a81b57a4f36b2fa63491c85ed7c5fac622ee1fb25eeba8`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 1.3 MB (1294032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438726e25f92144a78f953c5663373fcaac4a7698b553b9c60f0a528727d3ab`  
		Last Modified: Tue, 05 May 2020 22:01:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd46551fd135778e1f30daeaed384bb140cfcd0ec5223e1205796319f362ff4`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d2ced395addf9dfd75088358f126f0639fecee4baa04232593bfef4c1ca224`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8a338b3cd6e0522d30c4bfc660c99839f0ae56389eed3baafac8904aad25cb`  
		Last Modified: Tue, 05 May 2020 22:01:43 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:edfaf333d29ac809d71952b06c0654e1ff771c5e2e67c8062f8da0fc8fc2bb47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:6d051a73c9ea33554c21fcf05e4e8a9ebc63304ac2c55077597cd75cf0db7313
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351169100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f52c09a2c68171d4426b3283ac9adb21320d08150c8c272d2a8eb69bb5554ca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:46:48 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:47:21 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:47:22 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 05 May 2020 21:47:22 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:47:44 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.5.tar.gz.asc crate-4.1.5.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.5.tar.gz.asc     && tar -xf crate-4.1.5.tar.gz -C /crate --strip-components=1     && rm crate-4.1.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:47:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:47:47 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:47:47 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:47:48 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:47:48 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:47:48 GMT
WORKDIR /data
# Tue, 05 May 2020 21:47:49 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:47:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:47:49 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:47:49 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-04-24T09:34:17.477377 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.5
# Tue, 05 May 2020 21:47:49 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:47:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:47:50 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71257ebe0f3fef179a3b311dacc64581971431e33927c6c2107d2442d4dc1d7b`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f1387b5ba8366a3891b3e1a0fed1418b2ad7e5acab59d784d711197333efe1`  
		Last Modified: Tue, 05 May 2020 21:52:48 GMT  
		Size: 196.4 MB (196423143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8301c448e63bb7d27fe72ed07696cfe892e51828e96684cf475a17360cbdbc`  
		Last Modified: Tue, 05 May 2020 21:51:55 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95b33f6df2f0a1079d1fcc203dc695a3ca044292e5752851187302493e6a494`  
		Last Modified: Tue, 05 May 2020 21:52:04 GMT  
		Size: 77.6 MB (77567470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78afef4592f2681f29a90e2e0c782ed6397088dde7e0386e0428cc3f963d05af`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 1.3 MB (1294033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ae7ca8b418576838b672b1c5e9d2433957aa11be7b3530f227d9ce3949dfc8`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81e06b30d48695b06b680e862fa3260ecb75167d7ef8632fa9278cc6fe7d2d3`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f010083d8abab3d444dec5fad2bde0ebf144ae53d9d00b29f1190115e39f6907`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44cf5112b81e9cea56e5be0def3d8a484ac3dd16d67b01858099f205f3ce1c1`  
		Last Modified: Tue, 05 May 2020 21:51:54 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:41dcfdb2c440f1e9259471537c1fe98073d02665d043cb6c9a59df93437c14d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.3 MB (378290980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f01df573ee22342b92e20cb3d41c13ded585d78393e7bb95f1e962a8df8b97`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 05 May 2020 21:41:25 GMT
ADD file:d64254c17612e9076d442240e4e567c0467ab6c4ca282ba5553f602805ad89ac in / 
# Tue, 05 May 2020 21:41:30 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:41:31 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:57:47 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 05 May 2020 21:58:08 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 05 May 2020 21:58:10 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 05 May 2020 21:58:11 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 05 May 2020 21:58:41 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.5.tar.gz.asc crate-4.1.5.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.5.tar.gz.asc     && tar -xf crate-4.1.5.tar.gz -C /crate --strip-components=1     && rm crate-4.1.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 05 May 2020 21:58:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 05 May 2020 21:58:47 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 May 2020 21:58:48 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 05 May 2020 21:58:49 GMT
RUN mkdir -p /data/data /data/log
# Tue, 05 May 2020 21:58:50 GMT
VOLUME [/data]
# Tue, 05 May 2020 21:58:51 GMT
WORKDIR /data
# Tue, 05 May 2020 21:58:51 GMT
EXPOSE 4200 4300 5432
# Tue, 05 May 2020 21:58:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 05 May 2020 21:58:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 05 May 2020 21:58:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-04-24T09:34:17.477377 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.5
# Tue, 05 May 2020 21:58:54 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 05 May 2020 21:58:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 May 2020 21:58:55 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ae60b79047f8473e02511e923f461b869b62d2bf110b9fa282656e9f0128932d`  
		Last Modified: Tue, 05 May 2020 21:42:11 GMT  
		Size: 104.6 MB (104555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cbdaa35d65e895b1f8cdcdae19714a1be917bbc2886d43605e27eea7c5016d`  
		Last Modified: Tue, 05 May 2020 22:01:46 GMT  
		Size: 2.2 KB (2248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4da918b90a19f31a2065118c658cefcb9e13af76a45daa0742673eb7067147`  
		Last Modified: Tue, 05 May 2020 22:02:17 GMT  
		Size: 196.4 MB (196423275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1563ebec551778313976636e734e51d8a4f4d4a96766b78a310c0602da3b64d4`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2af2046d4e2bb9e4f6f09c988d9b62fed090dc05b007b41fa3716313c6043`  
		Last Modified: Tue, 05 May 2020 22:01:59 GMT  
		Size: 76.0 MB (76013928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bc82dfaa3cf5b669a81b57a4f36b2fa63491c85ed7c5fac622ee1fb25eeba8`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 1.3 MB (1294032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438726e25f92144a78f953c5663373fcaac4a7698b553b9c60f0a528727d3ab`  
		Last Modified: Tue, 05 May 2020 22:01:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd46551fd135778e1f30daeaed384bb140cfcd0ec5223e1205796319f362ff4`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d2ced395addf9dfd75088358f126f0639fecee4baa04232593bfef4c1ca224`  
		Last Modified: Tue, 05 May 2020 22:01:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8a338b3cd6e0522d30c4bfc660c99839f0ae56389eed3baafac8904aad25cb`  
		Last Modified: Tue, 05 May 2020 22:01:43 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
