<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:3.3`](#crate33)
-	[`crate:3.3.5`](#crate335)
-	[`crate:4.0`](#crate40)
-	[`crate:4.0.12`](#crate4012)
-	[`crate:4.1`](#crate41)
-	[`crate:4.1.8`](#crate418)
-	[`crate:4.2`](#crate42)
-	[`crate:4.2.2`](#crate422)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:50ede860f2a02e50d671e83cf54b350ca5ddeaeaf5ca7152a92293c9c0686fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `crate:3.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:12813c03074e6f319ad6ef7c1cfee4cf4e5122605449ec469bff98b9697ca6b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357922633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1225d14dd38f6a2fb20c46a22e2ac9e33774012d00bcb290146787c1ecd2aaa`
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
# Wed, 10 Jun 2020 18:47:13 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 10 Jun 2020 18:47:15 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Wed, 10 Jun 2020 18:47:17 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Wed, 10 Jun 2020 18:49:52 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Wed, 10 Jun 2020 18:49:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:49:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:49:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 10 Jun 2020 18:49:57 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 18:49:57 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 10 Jun 2020 18:49:59 GMT
RUN mkdir -p /data/data /data/log
# Wed, 10 Jun 2020 18:49:59 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 18:50:00 GMT
WORKDIR /data
# Wed, 10 Jun 2020 18:50:00 GMT
EXPOSE 4200 4300 5432
# Wed, 10 Jun 2020 18:50:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:50:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:50:02 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2019-07-08T14:08:18.187344 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Wed, 10 Jun 2020 18:50:03 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 10 Jun 2020 18:50:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 18:50:04 GMT
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
	-	`sha256:42b65e8e76759b528fbf478154a35bae9dc5cae82f4ea46ba9109dc974b1d040`  
		Last Modified: Wed, 10 Jun 2020 18:52:09 GMT  
		Size: 188.1 MB (188101365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dd833f60262e2e8739a74fc1426349754fd5c55927d80ff1c7a009dd2a0458`  
		Last Modified: Wed, 10 Jun 2020 18:51:39 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17f2cfc0b5b8f99949a4ed1601440b507b02055137b801383bd8ea1a829d8c1`  
		Last Modified: Wed, 10 Jun 2020 18:51:51 GMT  
		Size: 64.0 MB (63966262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aab02632f30e1771713b36acc3f7b44395f689cb8bb90e923fc9ab9acd1bd3`  
		Last Modified: Wed, 10 Jun 2020 18:51:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f646b9e13d58daaec0002de689894c69e00f4601914fc7f579f327fa4dc61a05`  
		Last Modified: Wed, 10 Jun 2020 18:51:39 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7f9092d9915dcecb9763b7f9b55c89455cfb0b2192749b3ebf90b29cd92f84`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 1.3 MB (1294038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e7c3aabcda41d7a1a75fc9ee324b90ea7768859ebfb2abcf2a7d7e29a935c7`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a56cbd215bea7720a803ab31bd66d403e95b3d028d5c233701eebce2116fde`  
		Last Modified: Wed, 10 Jun 2020 18:51:38 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5018b6f6ff37b30ffe93eee3679321b614a4e552b88322025264201dcd01554d`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd533bcfbfdfecc4138ea44c166ccdf5ada5ee1a7be5dd961bca909044d2c0c`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:3.3.5`

```console
$ docker pull crate@sha256:50ede860f2a02e50d671e83cf54b350ca5ddeaeaf5ca7152a92293c9c0686fa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `crate:3.3.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:12813c03074e6f319ad6ef7c1cfee4cf4e5122605449ec469bff98b9697ca6b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.9 MB (357922633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1225d14dd38f6a2fb20c46a22e2ac9e33774012d00bcb290146787c1ecd2aaa`
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
# Wed, 10 Jun 2020 18:47:13 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 10 Jun 2020 18:47:15 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Wed, 10 Jun 2020 18:47:17 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Wed, 10 Jun 2020 18:49:52 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Wed, 10 Jun 2020 18:49:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:49:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:49:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 10 Jun 2020 18:49:57 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 18:49:57 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 10 Jun 2020 18:49:59 GMT
RUN mkdir -p /data/data /data/log
# Wed, 10 Jun 2020 18:49:59 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 18:50:00 GMT
WORKDIR /data
# Wed, 10 Jun 2020 18:50:00 GMT
EXPOSE 4200 4300 5432
# Wed, 10 Jun 2020 18:50:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:50:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:50:02 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2019-07-08T14:08:18.187344 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Wed, 10 Jun 2020 18:50:03 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 10 Jun 2020 18:50:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 18:50:04 GMT
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
	-	`sha256:42b65e8e76759b528fbf478154a35bae9dc5cae82f4ea46ba9109dc974b1d040`  
		Last Modified: Wed, 10 Jun 2020 18:52:09 GMT  
		Size: 188.1 MB (188101365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dd833f60262e2e8739a74fc1426349754fd5c55927d80ff1c7a009dd2a0458`  
		Last Modified: Wed, 10 Jun 2020 18:51:39 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17f2cfc0b5b8f99949a4ed1601440b507b02055137b801383bd8ea1a829d8c1`  
		Last Modified: Wed, 10 Jun 2020 18:51:51 GMT  
		Size: 64.0 MB (63966262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aab02632f30e1771713b36acc3f7b44395f689cb8bb90e923fc9ab9acd1bd3`  
		Last Modified: Wed, 10 Jun 2020 18:51:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f646b9e13d58daaec0002de689894c69e00f4601914fc7f579f327fa4dc61a05`  
		Last Modified: Wed, 10 Jun 2020 18:51:39 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7f9092d9915dcecb9763b7f9b55c89455cfb0b2192749b3ebf90b29cd92f84`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 1.3 MB (1294038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e7c3aabcda41d7a1a75fc9ee324b90ea7768859ebfb2abcf2a7d7e29a935c7`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a56cbd215bea7720a803ab31bd66d403e95b3d028d5c233701eebce2116fde`  
		Last Modified: Wed, 10 Jun 2020 18:51:38 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5018b6f6ff37b30ffe93eee3679321b614a4e552b88322025264201dcd01554d`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd533bcfbfdfecc4138ea44c166ccdf5ada5ee1a7be5dd961bca909044d2c0c`  
		Last Modified: Wed, 10 Jun 2020 18:51:37 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0`

```console
$ docker pull crate@sha256:14d780d24d42a12293dd35ae4ef0b1e814a51ea3b54a9a201922251adcb58685
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
$ docker pull crate@sha256:98837cc92307195e2463b21df43b2d37a53f521f4ef021b1cf6a899b4c41cdda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.5 MB (365518204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78903036bea7e8aebd3f32d37a9384912d27432511ef751089e8c25c45eca01e`
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
# Wed, 10 Jun 2020 18:43:09 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 10 Jun 2020 18:43:11 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Wed, 10 Jun 2020 18:43:13 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Wed, 10 Jun 2020 18:45:55 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Wed, 10 Jun 2020 18:45:56 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:45:57 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:45:59 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 10 Jun 2020 18:46:01 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 18:46:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 10 Jun 2020 18:46:03 GMT
RUN mkdir -p /data/data /data/log
# Wed, 10 Jun 2020 18:46:04 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 18:46:05 GMT
WORKDIR /data
# Wed, 10 Jun 2020 18:46:06 GMT
EXPOSE 4200 4300 5432
# Wed, 10 Jun 2020 18:46:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:46:08 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:46:10 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Wed, 10 Jun 2020 18:46:11 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 10 Jun 2020 18:46:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 18:46:15 GMT
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
	-	`sha256:13bb058dace3e29fd10775283a52a16f4f165733d906f3c9249cff8f20687e3e`  
		Last Modified: Wed, 10 Jun 2020 18:51:30 GMT  
		Size: 198.1 MB (198127547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f5735c336e0f16e6d94fc95332ea8ebc5f95c87f898d3df07bd03ec13edb6e`  
		Last Modified: Wed, 10 Jun 2020 18:50:57 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e68802fc289041528dd3d23daada26a314bfa8b56f4dc9e4bd56d6bf06ce9`  
		Last Modified: Wed, 10 Jun 2020 18:51:06 GMT  
		Size: 61.5 MB (61535642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4f20b4a23f854363ac2255bbfb58329a7cb747c52ff623007d513d789a75c0`  
		Last Modified: Wed, 10 Jun 2020 18:50:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b64bdaa8c18ce9ac985f87da7231f4d6ae146421acf7d8994bf33ed2378bc0`  
		Last Modified: Wed, 10 Jun 2020 18:50:56 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602f7320a3b46f82f8d087dbcbe2eb9b24466acf6e29f08d6578fe893f1008e8`  
		Last Modified: Wed, 10 Jun 2020 18:50:55 GMT  
		Size: 1.3 MB (1294044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b842ed9fb387259eeabf6e21d28bf4fd58d02898b5eb3c13f94dc7ad582ba7`  
		Last Modified: Wed, 10 Jun 2020 18:50:55 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b5c20f553df3f2fbc25f5db94b5492d4a61e311181ce4a3ad6980b2c9e47f5`  
		Last Modified: Wed, 10 Jun 2020 18:50:54 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502aee01ff50555ab62a611955ba8f875752a36552d7761cf5d461077123c905`  
		Last Modified: Wed, 10 Jun 2020 18:50:54 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327e0030bc329534f801f4d2a2930eb2ea0c065945fe0e12545a75acb7704b51`  
		Last Modified: Wed, 10 Jun 2020 18:50:54 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0.12`

```console
$ docker pull crate@sha256:14d780d24d42a12293dd35ae4ef0b1e814a51ea3b54a9a201922251adcb58685
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
$ docker pull crate@sha256:98837cc92307195e2463b21df43b2d37a53f521f4ef021b1cf6a899b4c41cdda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.5 MB (365518204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78903036bea7e8aebd3f32d37a9384912d27432511ef751089e8c25c45eca01e`
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
# Wed, 10 Jun 2020 18:43:09 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 10 Jun 2020 18:43:11 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Wed, 10 Jun 2020 18:43:13 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Wed, 10 Jun 2020 18:45:55 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Wed, 10 Jun 2020 18:45:56 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:45:57 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:45:59 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 10 Jun 2020 18:46:01 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 18:46:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 10 Jun 2020 18:46:03 GMT
RUN mkdir -p /data/data /data/log
# Wed, 10 Jun 2020 18:46:04 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 18:46:05 GMT
WORKDIR /data
# Wed, 10 Jun 2020 18:46:06 GMT
EXPOSE 4200 4300 5432
# Wed, 10 Jun 2020 18:46:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:46:08 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:46:10 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Wed, 10 Jun 2020 18:46:11 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 10 Jun 2020 18:46:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 18:46:15 GMT
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
	-	`sha256:13bb058dace3e29fd10775283a52a16f4f165733d906f3c9249cff8f20687e3e`  
		Last Modified: Wed, 10 Jun 2020 18:51:30 GMT  
		Size: 198.1 MB (198127547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f5735c336e0f16e6d94fc95332ea8ebc5f95c87f898d3df07bd03ec13edb6e`  
		Last Modified: Wed, 10 Jun 2020 18:50:57 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e68802fc289041528dd3d23daada26a314bfa8b56f4dc9e4bd56d6bf06ce9`  
		Last Modified: Wed, 10 Jun 2020 18:51:06 GMT  
		Size: 61.5 MB (61535642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4f20b4a23f854363ac2255bbfb58329a7cb747c52ff623007d513d789a75c0`  
		Last Modified: Wed, 10 Jun 2020 18:50:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b64bdaa8c18ce9ac985f87da7231f4d6ae146421acf7d8994bf33ed2378bc0`  
		Last Modified: Wed, 10 Jun 2020 18:50:56 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602f7320a3b46f82f8d087dbcbe2eb9b24466acf6e29f08d6578fe893f1008e8`  
		Last Modified: Wed, 10 Jun 2020 18:50:55 GMT  
		Size: 1.3 MB (1294044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b842ed9fb387259eeabf6e21d28bf4fd58d02898b5eb3c13f94dc7ad582ba7`  
		Last Modified: Wed, 10 Jun 2020 18:50:55 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b5c20f553df3f2fbc25f5db94b5492d4a61e311181ce4a3ad6980b2c9e47f5`  
		Last Modified: Wed, 10 Jun 2020 18:50:54 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502aee01ff50555ab62a611955ba8f875752a36552d7761cf5d461077123c905`  
		Last Modified: Wed, 10 Jun 2020 18:50:54 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327e0030bc329534f801f4d2a2930eb2ea0c065945fe0e12545a75acb7704b51`  
		Last Modified: Wed, 10 Jun 2020 18:50:54 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1`

```console
$ docker pull crate@sha256:878e566faad981f7b0ebdbf35ac2203a16ff85c9855150c85e96caa4b2dddbd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1` - linux; amd64

```console
$ docker pull crate@sha256:92a8a499b25eeab4f4d404753669c35856cb638869dc698d6d9542325ce3ce75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351232248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8db1d2b270798813b1ad18a83295b5c26562dda2f48e39ee7a3a9e44ebd966`
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
# Thu, 09 Jul 2020 21:19:51 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 09 Jul 2020 21:19:53 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 09 Jul 2020 21:19:53 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jul 2020 21:19:53 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 09 Jul 2020 21:19:54 GMT
RUN mkdir -p /data/data /data/log
# Thu, 09 Jul 2020 21:19:54 GMT
VOLUME [/data]
# Thu, 09 Jul 2020 21:19:55 GMT
WORKDIR /data
# Thu, 09 Jul 2020 21:19:55 GMT
EXPOSE 4200 4300 5432
# Thu, 09 Jul 2020 21:19:55 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 09 Jul 2020 21:19:55 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 09 Jul 2020 21:19:55 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Thu, 09 Jul 2020 21:19:56 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 09 Jul 2020 21:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 09 Jul 2020 21:19:56 GMT
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
	-	`sha256:726877e2e4187e5b0d625801c9798e5fbf2ea4cc767f8218631fa6a7db2b6e95`  
		Last Modified: Thu, 09 Jul 2020 21:20:21 GMT  
		Size: 77.6 MB (77630607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b4b8b4396f63b076a06f6d25cfe8ede2a2f47300ab61a1bbc7c3abe7597777`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 1.3 MB (1294048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1222f72af97472fa260157afadf366133831bc7b73c3dacb7fcab75777f3a75f`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49d0665a0daa96aea38643a8e275fdfeeda8c5f06d23bbd62c5f4414982bb7`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96830eaca69dbdda09dfe57f46388fc0cab4550ea9c5b68f27f1b4e8ca1c33d7`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f5e4e23db5b8f05fa18c3db28858e0c450d7ce1455bae24d70ff907339cca`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:0397147b051bb0bc5a4af22b2e5b89b634ac0990acf4c899f1ee02945b6b7ad7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.4 MB (378372055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf018fa812ac56112ca2d7641bf4ea690c27143a731b0290856a98698ea855c`
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
# Thu, 09 Jul 2020 20:40:18 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 09 Jul 2020 20:40:22 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 09 Jul 2020 20:40:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jul 2020 20:40:24 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 09 Jul 2020 20:40:25 GMT
RUN mkdir -p /data/data /data/log
# Thu, 09 Jul 2020 20:40:26 GMT
VOLUME [/data]
# Thu, 09 Jul 2020 20:40:27 GMT
WORKDIR /data
# Thu, 09 Jul 2020 20:40:27 GMT
EXPOSE 4200 4300 5432
# Thu, 09 Jul 2020 20:40:28 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 09 Jul 2020 20:40:29 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 09 Jul 2020 20:40:31 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Thu, 09 Jul 2020 20:40:33 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 09 Jul 2020 20:40:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 09 Jul 2020 20:40:37 GMT
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
	-	`sha256:460af81dab5b05883aecafc5900e8970589031708a6e91c7970f1f90502ac5c2`  
		Last Modified: Thu, 09 Jul 2020 20:41:33 GMT  
		Size: 76.1 MB (76094992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1539f7927fe408070bc3406d88bd03d487f87eceadb51c1a26983c33fa6b93`  
		Last Modified: Thu, 09 Jul 2020 20:41:02 GMT  
		Size: 1.3 MB (1294050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de2b65f9dc4157952ff95be0ff00b4e1576e1d2a6581bf356ee434950474f1b`  
		Last Modified: Thu, 09 Jul 2020 20:41:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010a6d228114ea28b25311eb7ee57887205dc9e363b1f68f05abb06609e6fb00`  
		Last Modified: Thu, 09 Jul 2020 20:41:01 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6737efdaec3dfbbc1f25a67bbe89e1de9b83a3643292761d1fe87b0522aa7ce7`  
		Last Modified: Thu, 09 Jul 2020 20:41:01 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90106c6df949b02e9354ee34977a994a011ffc6afa6e60f0a6809158c73eaa0`  
		Last Modified: Thu, 09 Jul 2020 20:41:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1.8`

```console
$ docker pull crate@sha256:878e566faad981f7b0ebdbf35ac2203a16ff85c9855150c85e96caa4b2dddbd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1.8` - linux; amd64

```console
$ docker pull crate@sha256:92a8a499b25eeab4f4d404753669c35856cb638869dc698d6d9542325ce3ce75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351232248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8db1d2b270798813b1ad18a83295b5c26562dda2f48e39ee7a3a9e44ebd966`
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
# Thu, 09 Jul 2020 21:19:51 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 09 Jul 2020 21:19:53 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 09 Jul 2020 21:19:53 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jul 2020 21:19:53 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 09 Jul 2020 21:19:54 GMT
RUN mkdir -p /data/data /data/log
# Thu, 09 Jul 2020 21:19:54 GMT
VOLUME [/data]
# Thu, 09 Jul 2020 21:19:55 GMT
WORKDIR /data
# Thu, 09 Jul 2020 21:19:55 GMT
EXPOSE 4200 4300 5432
# Thu, 09 Jul 2020 21:19:55 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 09 Jul 2020 21:19:55 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 09 Jul 2020 21:19:55 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Thu, 09 Jul 2020 21:19:56 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 09 Jul 2020 21:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 09 Jul 2020 21:19:56 GMT
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
	-	`sha256:726877e2e4187e5b0d625801c9798e5fbf2ea4cc767f8218631fa6a7db2b6e95`  
		Last Modified: Thu, 09 Jul 2020 21:20:21 GMT  
		Size: 77.6 MB (77630607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b4b8b4396f63b076a06f6d25cfe8ede2a2f47300ab61a1bbc7c3abe7597777`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 1.3 MB (1294048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1222f72af97472fa260157afadf366133831bc7b73c3dacb7fcab75777f3a75f`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49d0665a0daa96aea38643a8e275fdfeeda8c5f06d23bbd62c5f4414982bb7`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96830eaca69dbdda09dfe57f46388fc0cab4550ea9c5b68f27f1b4e8ca1c33d7`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730f5e4e23db5b8f05fa18c3db28858e0c450d7ce1455bae24d70ff907339cca`  
		Last Modified: Thu, 09 Jul 2020 21:20:13 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:0397147b051bb0bc5a4af22b2e5b89b634ac0990acf4c899f1ee02945b6b7ad7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.4 MB (378372055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf018fa812ac56112ca2d7641bf4ea690c27143a731b0290856a98698ea855c`
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
# Thu, 09 Jul 2020 20:40:18 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 09 Jul 2020 20:40:22 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 09 Jul 2020 20:40:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Jul 2020 20:40:24 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 09 Jul 2020 20:40:25 GMT
RUN mkdir -p /data/data /data/log
# Thu, 09 Jul 2020 20:40:26 GMT
VOLUME [/data]
# Thu, 09 Jul 2020 20:40:27 GMT
WORKDIR /data
# Thu, 09 Jul 2020 20:40:27 GMT
EXPOSE 4200 4300 5432
# Thu, 09 Jul 2020 20:40:28 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 09 Jul 2020 20:40:29 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 09 Jul 2020 20:40:31 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Thu, 09 Jul 2020 20:40:33 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 09 Jul 2020 20:40:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 09 Jul 2020 20:40:37 GMT
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
	-	`sha256:460af81dab5b05883aecafc5900e8970589031708a6e91c7970f1f90502ac5c2`  
		Last Modified: Thu, 09 Jul 2020 20:41:33 GMT  
		Size: 76.1 MB (76094992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1539f7927fe408070bc3406d88bd03d487f87eceadb51c1a26983c33fa6b93`  
		Last Modified: Thu, 09 Jul 2020 20:41:02 GMT  
		Size: 1.3 MB (1294050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de2b65f9dc4157952ff95be0ff00b4e1576e1d2a6581bf356ee434950474f1b`  
		Last Modified: Thu, 09 Jul 2020 20:41:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010a6d228114ea28b25311eb7ee57887205dc9e363b1f68f05abb06609e6fb00`  
		Last Modified: Thu, 09 Jul 2020 20:41:01 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6737efdaec3dfbbc1f25a67bbe89e1de9b83a3643292761d1fe87b0522aa7ce7`  
		Last Modified: Thu, 09 Jul 2020 20:41:01 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90106c6df949b02e9354ee34977a994a011ffc6afa6e60f0a6809158c73eaa0`  
		Last Modified: Thu, 09 Jul 2020 20:41:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2`

```console
$ docker pull crate@sha256:44e5b0708b7d42e1a95c9360335c461b4227abed9f9a0d218cb2b7778c4215b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2` - linux; amd64

```console
$ docker pull crate@sha256:3cb31c77afb9f11e40964702db43a94191e0961c07fa1ea1833b197ee590184f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332894796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d24fc1d34d79144a360d3fca95a0c3849d17964f3887f092266b48c6995c60d9`
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
# Thu, 30 Jul 2020 19:20:04 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.2.tar.gz.asc crate-4.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.2.tar.gz.asc     && tar -xf crate-4.2.2.tar.gz -C /crate --strip-components=1     && rm crate-4.2.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 30 Jul 2020 19:20:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 30 Jul 2020 19:20:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 19:20:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 30 Jul 2020 19:20:08 GMT
RUN mkdir -p /data/data /data/log
# Thu, 30 Jul 2020 19:20:08 GMT
VOLUME [/data]
# Thu, 30 Jul 2020 19:20:08 GMT
WORKDIR /data
# Thu, 30 Jul 2020 19:20:08 GMT
EXPOSE 4200 4300 5432
# Thu, 30 Jul 2020 19:20:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 30 Jul 2020 19:20:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 30 Jul 2020 19:20:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-28T13:36:02.304329 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.2
# Thu, 30 Jul 2020 19:20:09 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 30 Jul 2020 19:20:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jul 2020 19:20:10 GMT
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
	-	`sha256:52ed411437212eb8b11f7f97d9a95aed58d58b9525579a69fd860e441a9daaf9`  
		Last Modified: Thu, 30 Jul 2020 19:20:55 GMT  
		Size: 255.5 MB (255507315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac5036b8d8ed811e7ae3ba2898ac35dbcd0fc776f887d5198e348c6853a9a4`  
		Last Modified: Thu, 30 Jul 2020 19:20:31 GMT  
		Size: 1.5 MB (1503270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746da4ff080bb311a4a86db7736337115b4ababd8dd9f9271c77e5ef4adbcda4`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582622b6da68422f94163a44a84f157a315bdff756d928cdf5f0af1116c981e8`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2aecf65e0400b5da0f6ea1c4ca31a6616ad85b122c5f27e6900ef02c8a82ff`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c77a4ec39e429d5000ec4e5fd4d9af0748c78a8e3a62428d6e1ef2ccfe1b7c`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:eb8086a02a93ad60ad6a1df00c0b72297141603e790ddba95b2353e69fd0f21a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357453672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4274ccb4bf21fef45695c419cc4512d5a9fba4f1ea268293ec61bee67e2fe515`
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
# Thu, 30 Jul 2020 19:40:55 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.2.tar.gz.asc crate-4.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.2.tar.gz.asc     && tar -xf crate-4.2.2.tar.gz -C /crate --strip-components=1     && rm crate-4.2.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 30 Jul 2020 19:41:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 30 Jul 2020 19:41:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 19:41:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 30 Jul 2020 19:41:05 GMT
RUN mkdir -p /data/data /data/log
# Thu, 30 Jul 2020 19:41:06 GMT
VOLUME [/data]
# Thu, 30 Jul 2020 19:41:07 GMT
WORKDIR /data
# Thu, 30 Jul 2020 19:41:08 GMT
EXPOSE 4200 4300 5432
# Thu, 30 Jul 2020 19:41:08 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 30 Jul 2020 19:41:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 30 Jul 2020 19:41:10 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-28T13:36:02.304329 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.2
# Thu, 30 Jul 2020 19:41:11 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 30 Jul 2020 19:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jul 2020 19:41:13 GMT
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
	-	`sha256:238ded818ae55c1fdd46b43d62a51adca81edd72b78f497ed1362f2ae6678889`  
		Last Modified: Thu, 30 Jul 2020 19:42:36 GMT  
		Size: 251.4 MB (251390891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be619999db7105e2079f6431f54b1ae54a27fff0c4cf22ab355397191bc34eb`  
		Last Modified: Thu, 30 Jul 2020 19:41:53 GMT  
		Size: 1.5 MB (1503279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb846e586c02bde989d3e11e68860a6c40f442e93d3219d537398a3badb9ec`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8244f27d2bf57c4e6671cb36595a2e502fc492e792916eead305d5742b2714ab`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3e347548c29ce18f09d0766c39538d0f1d4c4553559d41dada9db7278b666f`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ec6b00082c76d14034f8f5f58aa508285b6d10f91bf2683c33a86aa27403fe`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2.2`

```console
$ docker pull crate@sha256:44e5b0708b7d42e1a95c9360335c461b4227abed9f9a0d218cb2b7778c4215b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2.2` - linux; amd64

```console
$ docker pull crate@sha256:3cb31c77afb9f11e40964702db43a94191e0961c07fa1ea1833b197ee590184f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332894796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d24fc1d34d79144a360d3fca95a0c3849d17964f3887f092266b48c6995c60d9`
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
# Thu, 30 Jul 2020 19:20:04 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.2.tar.gz.asc crate-4.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.2.tar.gz.asc     && tar -xf crate-4.2.2.tar.gz -C /crate --strip-components=1     && rm crate-4.2.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 30 Jul 2020 19:20:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 30 Jul 2020 19:20:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 19:20:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 30 Jul 2020 19:20:08 GMT
RUN mkdir -p /data/data /data/log
# Thu, 30 Jul 2020 19:20:08 GMT
VOLUME [/data]
# Thu, 30 Jul 2020 19:20:08 GMT
WORKDIR /data
# Thu, 30 Jul 2020 19:20:08 GMT
EXPOSE 4200 4300 5432
# Thu, 30 Jul 2020 19:20:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 30 Jul 2020 19:20:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 30 Jul 2020 19:20:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-28T13:36:02.304329 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.2
# Thu, 30 Jul 2020 19:20:09 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 30 Jul 2020 19:20:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jul 2020 19:20:10 GMT
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
	-	`sha256:52ed411437212eb8b11f7f97d9a95aed58d58b9525579a69fd860e441a9daaf9`  
		Last Modified: Thu, 30 Jul 2020 19:20:55 GMT  
		Size: 255.5 MB (255507315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac5036b8d8ed811e7ae3ba2898ac35dbcd0fc776f887d5198e348c6853a9a4`  
		Last Modified: Thu, 30 Jul 2020 19:20:31 GMT  
		Size: 1.5 MB (1503270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746da4ff080bb311a4a86db7736337115b4ababd8dd9f9271c77e5ef4adbcda4`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582622b6da68422f94163a44a84f157a315bdff756d928cdf5f0af1116c981e8`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2aecf65e0400b5da0f6ea1c4ca31a6616ad85b122c5f27e6900ef02c8a82ff`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c77a4ec39e429d5000ec4e5fd4d9af0748c78a8e3a62428d6e1ef2ccfe1b7c`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.2.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:eb8086a02a93ad60ad6a1df00c0b72297141603e790ddba95b2353e69fd0f21a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357453672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4274ccb4bf21fef45695c419cc4512d5a9fba4f1ea268293ec61bee67e2fe515`
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
# Thu, 30 Jul 2020 19:40:55 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.2.tar.gz.asc crate-4.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.2.tar.gz.asc     && tar -xf crate-4.2.2.tar.gz -C /crate --strip-components=1     && rm crate-4.2.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 30 Jul 2020 19:41:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 30 Jul 2020 19:41:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 19:41:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 30 Jul 2020 19:41:05 GMT
RUN mkdir -p /data/data /data/log
# Thu, 30 Jul 2020 19:41:06 GMT
VOLUME [/data]
# Thu, 30 Jul 2020 19:41:07 GMT
WORKDIR /data
# Thu, 30 Jul 2020 19:41:08 GMT
EXPOSE 4200 4300 5432
# Thu, 30 Jul 2020 19:41:08 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 30 Jul 2020 19:41:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 30 Jul 2020 19:41:10 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-28T13:36:02.304329 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.2
# Thu, 30 Jul 2020 19:41:11 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 30 Jul 2020 19:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jul 2020 19:41:13 GMT
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
	-	`sha256:238ded818ae55c1fdd46b43d62a51adca81edd72b78f497ed1362f2ae6678889`  
		Last Modified: Thu, 30 Jul 2020 19:42:36 GMT  
		Size: 251.4 MB (251390891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be619999db7105e2079f6431f54b1ae54a27fff0c4cf22ab355397191bc34eb`  
		Last Modified: Thu, 30 Jul 2020 19:41:53 GMT  
		Size: 1.5 MB (1503279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb846e586c02bde989d3e11e68860a6c40f442e93d3219d537398a3badb9ec`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8244f27d2bf57c4e6671cb36595a2e502fc492e792916eead305d5742b2714ab`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3e347548c29ce18f09d0766c39538d0f1d4c4553559d41dada9db7278b666f`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ec6b00082c76d14034f8f5f58aa508285b6d10f91bf2683c33a86aa27403fe`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:44e5b0708b7d42e1a95c9360335c461b4227abed9f9a0d218cb2b7778c4215b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:3cb31c77afb9f11e40964702db43a94191e0961c07fa1ea1833b197ee590184f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332894796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d24fc1d34d79144a360d3fca95a0c3849d17964f3887f092266b48c6995c60d9`
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
# Thu, 30 Jul 2020 19:20:04 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.2.tar.gz.asc crate-4.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.2.tar.gz.asc     && tar -xf crate-4.2.2.tar.gz -C /crate --strip-components=1     && rm crate-4.2.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 30 Jul 2020 19:20:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 30 Jul 2020 19:20:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 19:20:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 30 Jul 2020 19:20:08 GMT
RUN mkdir -p /data/data /data/log
# Thu, 30 Jul 2020 19:20:08 GMT
VOLUME [/data]
# Thu, 30 Jul 2020 19:20:08 GMT
WORKDIR /data
# Thu, 30 Jul 2020 19:20:08 GMT
EXPOSE 4200 4300 5432
# Thu, 30 Jul 2020 19:20:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 30 Jul 2020 19:20:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 30 Jul 2020 19:20:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-28T13:36:02.304329 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.2
# Thu, 30 Jul 2020 19:20:09 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 30 Jul 2020 19:20:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jul 2020 19:20:10 GMT
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
	-	`sha256:52ed411437212eb8b11f7f97d9a95aed58d58b9525579a69fd860e441a9daaf9`  
		Last Modified: Thu, 30 Jul 2020 19:20:55 GMT  
		Size: 255.5 MB (255507315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ac5036b8d8ed811e7ae3ba2898ac35dbcd0fc776f887d5198e348c6853a9a4`  
		Last Modified: Thu, 30 Jul 2020 19:20:31 GMT  
		Size: 1.5 MB (1503270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746da4ff080bb311a4a86db7736337115b4ababd8dd9f9271c77e5ef4adbcda4`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582622b6da68422f94163a44a84f157a315bdff756d928cdf5f0af1116c981e8`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2aecf65e0400b5da0f6ea1c4ca31a6616ad85b122c5f27e6900ef02c8a82ff`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c77a4ec39e429d5000ec4e5fd4d9af0748c78a8e3a62428d6e1ef2ccfe1b7c`  
		Last Modified: Thu, 30 Jul 2020 19:20:30 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:eb8086a02a93ad60ad6a1df00c0b72297141603e790ddba95b2353e69fd0f21a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357453672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4274ccb4bf21fef45695c419cc4512d5a9fba4f1ea268293ec61bee67e2fe515`
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
# Thu, 30 Jul 2020 19:40:55 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.2.tar.gz.asc crate-4.2.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.2.tar.gz.asc     && tar -xf crate-4.2.2.tar.gz -C /crate --strip-components=1     && rm crate-4.2.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 30 Jul 2020 19:41:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 30 Jul 2020 19:41:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 19:41:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 30 Jul 2020 19:41:05 GMT
RUN mkdir -p /data/data /data/log
# Thu, 30 Jul 2020 19:41:06 GMT
VOLUME [/data]
# Thu, 30 Jul 2020 19:41:07 GMT
WORKDIR /data
# Thu, 30 Jul 2020 19:41:08 GMT
EXPOSE 4200 4300 5432
# Thu, 30 Jul 2020 19:41:08 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 30 Jul 2020 19:41:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 30 Jul 2020 19:41:10 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-28T13:36:02.304329 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.2
# Thu, 30 Jul 2020 19:41:11 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 30 Jul 2020 19:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Jul 2020 19:41:13 GMT
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
	-	`sha256:238ded818ae55c1fdd46b43d62a51adca81edd72b78f497ed1362f2ae6678889`  
		Last Modified: Thu, 30 Jul 2020 19:42:36 GMT  
		Size: 251.4 MB (251390891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be619999db7105e2079f6431f54b1ae54a27fff0c4cf22ab355397191bc34eb`  
		Last Modified: Thu, 30 Jul 2020 19:41:53 GMT  
		Size: 1.5 MB (1503279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bb846e586c02bde989d3e11e68860a6c40f442e93d3219d537398a3badb9ec`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8244f27d2bf57c4e6671cb36595a2e502fc492e792916eead305d5742b2714ab`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3e347548c29ce18f09d0766c39538d0f1d4c4553559d41dada9db7278b666f`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ec6b00082c76d14034f8f5f58aa508285b6d10f91bf2683c33a86aa27403fe`  
		Last Modified: Thu, 30 Jul 2020 19:41:52 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
