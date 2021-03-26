<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:3.3`](#crate33)
-	[`crate:3.3.5`](#crate335)
-	[`crate:4.0`](#crate40)
-	[`crate:4.0.12`](#crate4012)
-	[`crate:4.1`](#crate41)
-	[`crate:4.1.8`](#crate418)
-	[`crate:4.2`](#crate42)
-	[`crate:4.2.7`](#crate427)
-	[`crate:4.3`](#crate43)
-	[`crate:4.3.4`](#crate434)
-	[`crate:4.4`](#crate44)
-	[`crate:4.4.3`](#crate443)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:442b92f3d3b76e974d1451331e4be9be221ac1a6a026f69b3b8731e23808a24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:3.3` - linux; amd64

```console
$ docker pull crate@sha256:a82b0d06d86500fb393004ddab798b710d7af384658595b7b23c6e9976478973
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346103954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:445a317709a88b0649fc4989a4013af56841f3a1a6e11b8059a8bc71f026b100`
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
# Tue, 09 Mar 2021 20:24:33 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 09 Mar 2021 20:24:34 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Tue, 09 Mar 2021 20:24:35 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Tue, 09 Mar 2021 20:24:59 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 09 Mar 2021 20:25:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:25:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:25:02 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:25:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:25:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:25:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:25:03 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:25:04 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:25:04 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:25:04 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:25:04 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:25:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Tue, 09 Mar 2021 20:25:05 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 09 Mar 2021 20:25:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:25:05 GMT
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
	-	`sha256:4c3cdcb3edc91d5b5e362b74a468101dac90b18657f37c367a68f33127d29439`  
		Last Modified: Tue, 09 Mar 2021 20:28:58 GMT  
		Size: 188.1 MB (188101411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbfde80d7fb442499d96fa7d043c6d009109720cb996e02c3100237dc125878`  
		Last Modified: Tue, 09 Mar 2021 20:28:41 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240968c311ddcf2ec6b03286b0d6e9bd97f49ce5825ebda21cda7828ff5e3e5`  
		Last Modified: Tue, 09 Mar 2021 20:28:50 GMT  
		Size: 80.6 MB (80605629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be938783f18b1b460f317bc3d4e6b5b2c6415dc618dbac3cc821431be5eb7b4e`  
		Last Modified: Tue, 09 Mar 2021 20:28:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d78096f881c0bebf622137b7f570033bf51523971c2eab2871eabae10c984b`  
		Last Modified: Tue, 09 Mar 2021 20:28:42 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87f75adadfe42f0c889a72d8d45994c1280ff0b234f9a26c58b71bbab15fc2b`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 1.3 MB (1294158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991cc49023fb7ca4c46787527fc51932751213cf75cf4cf7048c6e71d8030f4d`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65090910f7e4420775faf6e6ceae2da8aeb8066402154faba291d15e9abdfe6`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f9c03e8640842070897495b5c7ace8c627a9cc35acade0d10cdf70c521a1de`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d727cc776dca0e54c8d2e151bbb3bb69beb0866fc9aacd082ca5c4c2f0e662`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:3.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:ed2464dc32594e245352310614ce5af58b6a4902617828e36bb919578cc1528c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376280307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab779a95d11782b3d9d8dc3c58dbf84fd755c4926c0f0a74e4034556b08355d0`
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
# Sat, 14 Nov 2020 01:05:08 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 01:05:10 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Sat, 14 Nov 2020 01:05:12 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 01:05:44 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 01:05:46 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:05:47 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:05:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 01:05:50 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 01:05:51 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 01:05:53 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 01:05:53 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 01:05:54 GMT
WORKDIR /data
# Sat, 14 Nov 2020 01:05:55 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 01:05:56 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:05:56 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:05:57 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Sat, 14 Nov 2020 01:05:58 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:05:59 GMT
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
	-	`sha256:c30cda6499e26d716e28ee3ad7cde8a3d7fa001f4a29a99389c89f94c2a681ef`  
		Last Modified: Sat, 14 Nov 2020 01:10:17 GMT  
		Size: 188.1 MB (188101406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eb126b682cfde86c8ed0ee640a272c470f1ecd4750a8246077121cccc7f63b`  
		Last Modified: Sat, 14 Nov 2020 01:09:48 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f582a8190a4d8199aa22010881c019c9d376917a2d841aed420f57b71b6ee91`  
		Last Modified: Sat, 14 Nov 2020 01:10:03 GMT  
		Size: 78.5 MB (78504215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73900cbfd5cbe8c60cdc196bafeb64e0fb1807072a28237386fe93adb2bebc`  
		Last Modified: Sat, 14 Nov 2020 01:09:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca70d5ffe39424a0a50bfca44b066fd9881a124015e96b202e5ff6b2a4a0e6ba`  
		Last Modified: Sat, 14 Nov 2020 01:09:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f88bd25275ade38ab36ec5ba916d847038afbb8ab3834a992f72a2186e467e2`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 1.3 MB (1294144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58721756a33432a8170c1e77f6d3ff2f4097590b967df3a599b4a7f574ca18c1`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1529e276afbb97ccddf00035cb52c3246b538c34931c758b461ef7ed710c9011`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51065397e7e876c24ede8faac2eedd3d8384920afb7e9d58f898ea4f1d7a474`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e822ff220c837305d081afe63311d9356fb214af2359bd022edec64ad332beb3`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:3.3.5`

```console
$ docker pull crate@sha256:442b92f3d3b76e974d1451331e4be9be221ac1a6a026f69b3b8731e23808a24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:3.3.5` - linux; amd64

```console
$ docker pull crate@sha256:a82b0d06d86500fb393004ddab798b710d7af384658595b7b23c6e9976478973
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.1 MB (346103954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:445a317709a88b0649fc4989a4013af56841f3a1a6e11b8059a8bc71f026b100`
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
# Tue, 09 Mar 2021 20:24:33 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 09 Mar 2021 20:24:34 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Tue, 09 Mar 2021 20:24:35 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Tue, 09 Mar 2021 20:24:59 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 09 Mar 2021 20:25:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:25:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:25:02 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:25:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:25:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:25:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:25:03 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:25:04 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:25:04 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:25:04 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:25:04 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:25:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Tue, 09 Mar 2021 20:25:05 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 09 Mar 2021 20:25:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:25:05 GMT
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
	-	`sha256:4c3cdcb3edc91d5b5e362b74a468101dac90b18657f37c367a68f33127d29439`  
		Last Modified: Tue, 09 Mar 2021 20:28:58 GMT  
		Size: 188.1 MB (188101411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbfde80d7fb442499d96fa7d043c6d009109720cb996e02c3100237dc125878`  
		Last Modified: Tue, 09 Mar 2021 20:28:41 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240968c311ddcf2ec6b03286b0d6e9bd97f49ce5825ebda21cda7828ff5e3e5`  
		Last Modified: Tue, 09 Mar 2021 20:28:50 GMT  
		Size: 80.6 MB (80605629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be938783f18b1b460f317bc3d4e6b5b2c6415dc618dbac3cc821431be5eb7b4e`  
		Last Modified: Tue, 09 Mar 2021 20:28:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d78096f881c0bebf622137b7f570033bf51523971c2eab2871eabae10c984b`  
		Last Modified: Tue, 09 Mar 2021 20:28:42 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87f75adadfe42f0c889a72d8d45994c1280ff0b234f9a26c58b71bbab15fc2b`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 1.3 MB (1294158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991cc49023fb7ca4c46787527fc51932751213cf75cf4cf7048c6e71d8030f4d`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65090910f7e4420775faf6e6ceae2da8aeb8066402154faba291d15e9abdfe6`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f9c03e8640842070897495b5c7ace8c627a9cc35acade0d10cdf70c521a1de`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d727cc776dca0e54c8d2e151bbb3bb69beb0866fc9aacd082ca5c4c2f0e662`  
		Last Modified: Tue, 09 Mar 2021 20:28:39 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:3.3.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:ed2464dc32594e245352310614ce5af58b6a4902617828e36bb919578cc1528c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376280307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab779a95d11782b3d9d8dc3c58dbf84fd755c4926c0f0a74e4034556b08355d0`
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
# Sat, 14 Nov 2020 01:05:08 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 01:05:10 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Sat, 14 Nov 2020 01:05:12 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 01:05:44 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 01:05:46 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:05:47 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:05:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 01:05:50 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 01:05:51 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 01:05:53 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 01:05:53 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 01:05:54 GMT
WORKDIR /data
# Sat, 14 Nov 2020 01:05:55 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 01:05:56 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:05:56 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:05:57 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Sat, 14 Nov 2020 01:05:58 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 01:05:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:05:59 GMT
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
	-	`sha256:c30cda6499e26d716e28ee3ad7cde8a3d7fa001f4a29a99389c89f94c2a681ef`  
		Last Modified: Sat, 14 Nov 2020 01:10:17 GMT  
		Size: 188.1 MB (188101406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eb126b682cfde86c8ed0ee640a272c470f1ecd4750a8246077121cccc7f63b`  
		Last Modified: Sat, 14 Nov 2020 01:09:48 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f582a8190a4d8199aa22010881c019c9d376917a2d841aed420f57b71b6ee91`  
		Last Modified: Sat, 14 Nov 2020 01:10:03 GMT  
		Size: 78.5 MB (78504215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73900cbfd5cbe8c60cdc196bafeb64e0fb1807072a28237386fe93adb2bebc`  
		Last Modified: Sat, 14 Nov 2020 01:09:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca70d5ffe39424a0a50bfca44b066fd9881a124015e96b202e5ff6b2a4a0e6ba`  
		Last Modified: Sat, 14 Nov 2020 01:09:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f88bd25275ade38ab36ec5ba916d847038afbb8ab3834a992f72a2186e467e2`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 1.3 MB (1294144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58721756a33432a8170c1e77f6d3ff2f4097590b967df3a599b4a7f574ca18c1`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1529e276afbb97ccddf00035cb52c3246b538c34931c758b461ef7ed710c9011`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51065397e7e876c24ede8faac2eedd3d8384920afb7e9d58f898ea4f1d7a474`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e822ff220c837305d081afe63311d9356fb214af2359bd022edec64ad332beb3`  
		Last Modified: Sat, 14 Nov 2020 01:09:45 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0`

```console
$ docker pull crate@sha256:337d5715f6eadb12e9d7961223c1d8590ce4c4b43532d0b0fed22e5d97cb348b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0` - linux; amd64

```console
$ docker pull crate@sha256:1b1a205d40e862f200d5714a251e3648402ebe5516fa869fb6e06e6976e70329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339601287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e9e140adecbefb64a12073c8cf53a73c63e5bbdfe7e7a1966007c6b9490873`
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
# Tue, 09 Mar 2021 20:23:39 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 09 Mar 2021 20:23:40 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Tue, 09 Mar 2021 20:23:40 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Tue, 09 Mar 2021 20:24:01 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 09 Mar 2021 20:24:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:24:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:24:03 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:24:04 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:24:04 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:24:05 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:24:05 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:24:05 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:24:05 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:24:05 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:24:06 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:24:06 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Tue, 09 Mar 2021 20:24:06 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 09 Mar 2021 20:24:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:24:06 GMT
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
	-	`sha256:8d90b303814e663a2853a97cecf6efb57821f9c031801c5672ff1dfcb0f52f5d`  
		Last Modified: Tue, 09 Mar 2021 20:28:27 GMT  
		Size: 198.1 MB (198127552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6eec2be2bc7ab34ded15c1aae4c687cf6b69235b237cf59c7393a62c7edc97`  
		Last Modified: Tue, 09 Mar 2021 20:28:10 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1656d5f4f03bbadea977446dfb616eb66e914148e539d6b1b993c696bd6f23`  
		Last Modified: Tue, 09 Mar 2021 20:28:16 GMT  
		Size: 64.1 MB (64076833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb26155e177e8ad9cbf2d4a9cdef7ac078ea01ed91789721ffbfdc491385cf7`  
		Last Modified: Tue, 09 Mar 2021 20:28:09 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d3222d064a9ae335c9713e95b12725449a150896e7787717e98a9c1f0aee06`  
		Last Modified: Tue, 09 Mar 2021 20:28:10 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df2571c306c2f561183bf75a1aa927014cb2c5a71072bcc620b2cab1813cfdf`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 1.3 MB (1294154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce01a612b0809ad5ef6e9006e54486d7a300bab44f9a3e59e341e8da77662cfe`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a229942ddbc5fe514982ef95cad402fb7985f1b1058fb59035027b260c1316`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854cb63ccac690414dcf434ff4df5296788ad0a75f8450d88203861c2c080d64`  
		Last Modified: Tue, 09 Mar 2021 20:28:06 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43491b82817e24f7dafdbed495bc2d62b5ff8b0d2a75626c559d05d2543f2ddd`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.0` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:3e638a84d6dfb3c90f3778c61157197f16da57746eaf6ff8c4b97528b1d5a112
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.2 MB (370199240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147ed7d416bcf2c131fa20179f5861acd50c9c72fde9a9753b2da0c0b73e765c`
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
# Sat, 14 Nov 2020 01:03:06 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 01:03:08 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Sat, 14 Nov 2020 01:03:09 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 01:03:32 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 01:03:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:03:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:03:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 01:03:37 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 01:03:38 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 01:03:39 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 01:03:40 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 01:03:41 GMT
WORKDIR /data
# Sat, 14 Nov 2020 01:03:42 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 01:03:42 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:03:43 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:03:44 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Sat, 14 Nov 2020 01:03:44 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 01:03:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:03:46 GMT
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
	-	`sha256:8016751b8390a93560f6f8959eb3ee03b17ed42ac7c95c74b3e56f40adde2b2d`  
		Last Modified: Sat, 14 Nov 2020 01:09:36 GMT  
		Size: 198.1 MB (198127573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c8996d9f36a8cc428e7b31ae457dc7bbfbb1b2fd831db58b638d94c803b70e`  
		Last Modified: Sat, 14 Nov 2020 01:09:07 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b010c1c981c9b7e39e59ce7d26ec7ef44ec8207a60559c0455e0a5a64e8cf828`  
		Last Modified: Sat, 14 Nov 2020 01:09:16 GMT  
		Size: 62.4 MB (62396980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210178d78b5be7e2ae8e36c41a12fa3153f0f2094d1b03f7968afafa604c3a1c`  
		Last Modified: Sat, 14 Nov 2020 01:09:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf8af7f457558678b62899b5cea1e15ad79a8c81e9b2db521a523c93354c57a`  
		Last Modified: Sat, 14 Nov 2020 01:09:07 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9956c05e2b86256eb3b986678d24343eb12f967ba22fd6e8da4b89a6fe83a9`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 1.3 MB (1294145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86412a68a244d48f86dac70c5fa2cc30fef4dac02264e2b0f82ac987ce1a6ee2`  
		Last Modified: Sat, 14 Nov 2020 01:09:05 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dac671149947c7e466c59a5a88241064379c0438df29dbc105afac4bf2b27a`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a41e9f83b00be37f02626814c4581224b9491340d1a0b9b8fe7bf054e3b3b3`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70508db6dcaf43d3bb3e07f238334bd6d7b0f5c235e4aebaeefa827ea234d96f`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0.12`

```console
$ docker pull crate@sha256:337d5715f6eadb12e9d7961223c1d8590ce4c4b43532d0b0fed22e5d97cb348b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0.12` - linux; amd64

```console
$ docker pull crate@sha256:1b1a205d40e862f200d5714a251e3648402ebe5516fa869fb6e06e6976e70329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339601287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e9e140adecbefb64a12073c8cf53a73c63e5bbdfe7e7a1966007c6b9490873`
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
# Tue, 09 Mar 2021 20:23:39 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 09 Mar 2021 20:23:40 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Tue, 09 Mar 2021 20:23:40 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Tue, 09 Mar 2021 20:24:01 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 09 Mar 2021 20:24:01 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:24:02 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:24:03 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:24:04 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:24:04 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:24:05 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:24:05 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:24:05 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:24:05 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:24:05 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:24:06 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:24:06 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Tue, 09 Mar 2021 20:24:06 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 09 Mar 2021 20:24:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:24:06 GMT
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
	-	`sha256:8d90b303814e663a2853a97cecf6efb57821f9c031801c5672ff1dfcb0f52f5d`  
		Last Modified: Tue, 09 Mar 2021 20:28:27 GMT  
		Size: 198.1 MB (198127552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6eec2be2bc7ab34ded15c1aae4c687cf6b69235b237cf59c7393a62c7edc97`  
		Last Modified: Tue, 09 Mar 2021 20:28:10 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1656d5f4f03bbadea977446dfb616eb66e914148e539d6b1b993c696bd6f23`  
		Last Modified: Tue, 09 Mar 2021 20:28:16 GMT  
		Size: 64.1 MB (64076833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb26155e177e8ad9cbf2d4a9cdef7ac078ea01ed91789721ffbfdc491385cf7`  
		Last Modified: Tue, 09 Mar 2021 20:28:09 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d3222d064a9ae335c9713e95b12725449a150896e7787717e98a9c1f0aee06`  
		Last Modified: Tue, 09 Mar 2021 20:28:10 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df2571c306c2f561183bf75a1aa927014cb2c5a71072bcc620b2cab1813cfdf`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 1.3 MB (1294154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce01a612b0809ad5ef6e9006e54486d7a300bab44f9a3e59e341e8da77662cfe`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a229942ddbc5fe514982ef95cad402fb7985f1b1058fb59035027b260c1316`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854cb63ccac690414dcf434ff4df5296788ad0a75f8450d88203861c2c080d64`  
		Last Modified: Tue, 09 Mar 2021 20:28:06 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43491b82817e24f7dafdbed495bc2d62b5ff8b0d2a75626c559d05d2543f2ddd`  
		Last Modified: Tue, 09 Mar 2021 20:28:07 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.0.12` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:3e638a84d6dfb3c90f3778c61157197f16da57746eaf6ff8c4b97528b1d5a112
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.2 MB (370199240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147ed7d416bcf2c131fa20179f5861acd50c9c72fde9a9753b2da0c0b73e765c`
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
# Sat, 14 Nov 2020 01:03:06 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 01:03:08 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Sat, 14 Nov 2020 01:03:09 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 01:03:32 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 01:03:33 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:03:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:03:36 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 01:03:37 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 01:03:38 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 01:03:39 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 01:03:40 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 01:03:41 GMT
WORKDIR /data
# Sat, 14 Nov 2020 01:03:42 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 01:03:42 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:03:43 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:03:44 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Sat, 14 Nov 2020 01:03:44 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 01:03:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:03:46 GMT
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
	-	`sha256:8016751b8390a93560f6f8959eb3ee03b17ed42ac7c95c74b3e56f40adde2b2d`  
		Last Modified: Sat, 14 Nov 2020 01:09:36 GMT  
		Size: 198.1 MB (198127573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c8996d9f36a8cc428e7b31ae457dc7bbfbb1b2fd831db58b638d94c803b70e`  
		Last Modified: Sat, 14 Nov 2020 01:09:07 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b010c1c981c9b7e39e59ce7d26ec7ef44ec8207a60559c0455e0a5a64e8cf828`  
		Last Modified: Sat, 14 Nov 2020 01:09:16 GMT  
		Size: 62.4 MB (62396980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210178d78b5be7e2ae8e36c41a12fa3153f0f2094d1b03f7968afafa604c3a1c`  
		Last Modified: Sat, 14 Nov 2020 01:09:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf8af7f457558678b62899b5cea1e15ad79a8c81e9b2db521a523c93354c57a`  
		Last Modified: Sat, 14 Nov 2020 01:09:07 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9956c05e2b86256eb3b986678d24343eb12f967ba22fd6e8da4b89a6fe83a9`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 1.3 MB (1294145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86412a68a244d48f86dac70c5fa2cc30fef4dac02264e2b0f82ac987ce1a6ee2`  
		Last Modified: Sat, 14 Nov 2020 01:09:05 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dac671149947c7e466c59a5a88241064379c0438df29dbc105afac4bf2b27a`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a41e9f83b00be37f02626814c4581224b9491340d1a0b9b8fe7bf054e3b3b3`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70508db6dcaf43d3bb3e07f238334bd6d7b0f5c235e4aebaeefa827ea234d96f`  
		Last Modified: Sat, 14 Nov 2020 01:09:04 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1`

```console
$ docker pull crate@sha256:265c6bca05b6619a56c8adf77a926dd9e818c89169b9e391915e5393b485b7d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1` - linux; amd64

```console
$ docker pull crate@sha256:279e9eacda6261f59d293758786b0728ea49ff63b860036d76201bc86255ac7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.7 MB (352665948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e21c209f36baf5fc9ad01d301b9e3429fe50a5ea38ac3727d6465a59659b091`
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
# Tue, 09 Mar 2021 20:22:27 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 09 Mar 2021 20:22:28 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 09 Mar 2021 20:22:29 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 09 Mar 2021 20:22:54 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:22:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:22:56 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:22:56 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:22:57 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:22:57 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:22:58 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:22:58 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:22:58 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:22:58 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:22:58 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Tue, 09 Mar 2021 20:22:58 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 09 Mar 2021 20:22:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:22:59 GMT
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
	-	`sha256:9c5e042b21a9096cdd11f5bc92033a7b9d3cf4d15c452249d852268edd9ac2e5`  
		Last Modified: Tue, 09 Mar 2021 20:27:49 GMT  
		Size: 196.4 MB (196423258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac097586f2278fa6617cf446043c27e98dfce17b0e06dddcef95a2e0ae61830`  
		Last Modified: Tue, 09 Mar 2021 20:27:33 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c290b73d7e4b41e32c1bbe1be041b5c3ec7996e592d132f5d9e4a10bf146be67`  
		Last Modified: Tue, 09 Mar 2021 20:27:42 GMT  
		Size: 78.8 MB (78847001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682e83f445dc211edb4f8873f88602442617e26c1b941d94433c05d7eb45682`  
		Last Modified: Tue, 09 Mar 2021 20:27:31 GMT  
		Size: 1.3 MB (1294155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746e49caaac3b3c23061f8054911f58160d521e8dfb847808fa9fe3bbcac63e`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58251fb724ef678fbc8bff8edbe586ff90c622c9b21fcfc644073962de732de1`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f37cec38b59b3f87898e85e66e132f2eb754716f630a95c3ca7d14b495524ed`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa11813eeec378a5169d8300fe3838d844d4357dc5c001c0a32f6fa9d8ef2343`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:4e32e1626974c78ff8cc693c9d65829bae7cb97ef7c35a5ea00d9727cfce8b36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.9 MB (382857642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba028a2b41f9ad93b23849d7ab0af00b745cd2e2a0c2f1f73ad14988de48761e`
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
# Sat, 14 Nov 2020 01:00:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 01:00:54 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Sat, 14 Nov 2020 01:00:56 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 01:01:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 01:01:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 01:01:33 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 01:01:34 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 01:01:36 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 01:01:37 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 01:01:38 GMT
WORKDIR /data
# Sat, 14 Nov 2020 01:01:39 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 01:01:39 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:01:40 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:01:41 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Sat, 14 Nov 2020 01:01:42 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 01:01:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:01:43 GMT
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
	-	`sha256:84b33816c3034b4e993bc4a884e7f0a7142c8946a8905d20bf2d921e257f15c1`  
		Last Modified: Sat, 14 Nov 2020 01:08:55 GMT  
		Size: 196.4 MB (196423317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48e09ad69fc3688289cfaaca979674bd7cb465750ba08635e2024c7fc55343d`  
		Last Modified: Sat, 14 Nov 2020 01:08:09 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d737666b64d0add96611499114a49567b41c8a38ed33cd3d3d93d59b40b7e3b8`  
		Last Modified: Sat, 14 Nov 2020 01:08:23 GMT  
		Size: 76.8 MB (76760859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e0dd382946cde140d2c98d65b1539ecbe442c3112a1422eccc6520d37c0b2`  
		Last Modified: Sat, 14 Nov 2020 01:08:07 GMT  
		Size: 1.3 MB (1294146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5347203a32417b2218db4ad60061d7365a80b4ac7e858f3bde6d3d642332e2`  
		Last Modified: Sat, 14 Nov 2020 01:08:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa16c3f1ee501724c18e7a58291fd70326efb2e1c03c1a1cd53b5885448814`  
		Last Modified: Sat, 14 Nov 2020 01:08:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9546b60eecaddeddf16d5339aa39ce8af86f066eba5ab6804bcb7bf358f3cc78`  
		Last Modified: Sat, 14 Nov 2020 01:08:08 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f747a681c66ed054a8be93251f108d5ba0ea35f03a3f5a2cd54a2d198e9e18b`  
		Last Modified: Sat, 14 Nov 2020 01:08:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1.8`

```console
$ docker pull crate@sha256:265c6bca05b6619a56c8adf77a926dd9e818c89169b9e391915e5393b485b7d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1.8` - linux; amd64

```console
$ docker pull crate@sha256:279e9eacda6261f59d293758786b0728ea49ff63b860036d76201bc86255ac7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.7 MB (352665948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e21c209f36baf5fc9ad01d301b9e3429fe50a5ea38ac3727d6465a59659b091`
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
# Tue, 09 Mar 2021 20:22:27 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 09 Mar 2021 20:22:28 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Tue, 09 Mar 2021 20:22:29 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 09 Mar 2021 20:22:54 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:22:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:22:56 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:22:56 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:22:57 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:22:57 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:22:58 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:22:58 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:22:58 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:22:58 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:22:58 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Tue, 09 Mar 2021 20:22:58 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 09 Mar 2021 20:22:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:22:59 GMT
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
	-	`sha256:9c5e042b21a9096cdd11f5bc92033a7b9d3cf4d15c452249d852268edd9ac2e5`  
		Last Modified: Tue, 09 Mar 2021 20:27:49 GMT  
		Size: 196.4 MB (196423258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac097586f2278fa6617cf446043c27e98dfce17b0e06dddcef95a2e0ae61830`  
		Last Modified: Tue, 09 Mar 2021 20:27:33 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c290b73d7e4b41e32c1bbe1be041b5c3ec7996e592d132f5d9e4a10bf146be67`  
		Last Modified: Tue, 09 Mar 2021 20:27:42 GMT  
		Size: 78.8 MB (78847001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682e83f445dc211edb4f8873f88602442617e26c1b941d94433c05d7eb45682`  
		Last Modified: Tue, 09 Mar 2021 20:27:31 GMT  
		Size: 1.3 MB (1294155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746e49caaac3b3c23061f8054911f58160d521e8dfb847808fa9fe3bbcac63e`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58251fb724ef678fbc8bff8edbe586ff90c622c9b21fcfc644073962de732de1`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f37cec38b59b3f87898e85e66e132f2eb754716f630a95c3ca7d14b495524ed`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa11813eeec378a5169d8300fe3838d844d4357dc5c001c0a32f6fa9d8ef2343`  
		Last Modified: Tue, 09 Mar 2021 20:27:30 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:4e32e1626974c78ff8cc693c9d65829bae7cb97ef7c35a5ea00d9727cfce8b36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.9 MB (382857642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba028a2b41f9ad93b23849d7ab0af00b745cd2e2a0c2f1f73ad14988de48761e`
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
# Sat, 14 Nov 2020 01:00:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 01:00:54 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Sat, 14 Nov 2020 01:00:56 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 01:01:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 01:01:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 01:01:33 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 01:01:34 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 01:01:36 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 01:01:37 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 01:01:38 GMT
WORKDIR /data
# Sat, 14 Nov 2020 01:01:39 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 01:01:39 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 01:01:40 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 01:01:41 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Sat, 14 Nov 2020 01:01:42 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 01:01:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:01:43 GMT
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
	-	`sha256:84b33816c3034b4e993bc4a884e7f0a7142c8946a8905d20bf2d921e257f15c1`  
		Last Modified: Sat, 14 Nov 2020 01:08:55 GMT  
		Size: 196.4 MB (196423317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48e09ad69fc3688289cfaaca979674bd7cb465750ba08635e2024c7fc55343d`  
		Last Modified: Sat, 14 Nov 2020 01:08:09 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d737666b64d0add96611499114a49567b41c8a38ed33cd3d3d93d59b40b7e3b8`  
		Last Modified: Sat, 14 Nov 2020 01:08:23 GMT  
		Size: 76.8 MB (76760859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89e0dd382946cde140d2c98d65b1539ecbe442c3112a1422eccc6520d37c0b2`  
		Last Modified: Sat, 14 Nov 2020 01:08:07 GMT  
		Size: 1.3 MB (1294146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5347203a32417b2218db4ad60061d7365a80b4ac7e858f3bde6d3d642332e2`  
		Last Modified: Sat, 14 Nov 2020 01:08:08 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa16c3f1ee501724c18e7a58291fd70326efb2e1c03c1a1cd53b5885448814`  
		Last Modified: Sat, 14 Nov 2020 01:08:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9546b60eecaddeddf16d5339aa39ce8af86f066eba5ab6804bcb7bf358f3cc78`  
		Last Modified: Sat, 14 Nov 2020 01:08:08 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f747a681c66ed054a8be93251f108d5ba0ea35f03a3f5a2cd54a2d198e9e18b`  
		Last Modified: Sat, 14 Nov 2020 01:08:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2`

```console
$ docker pull crate@sha256:76666715aa0e15f20b1f2d8544e0010b5ff087f4afd544623e869119b164cfad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2` - linux; amd64

```console
$ docker pull crate@sha256:66c5c0b0244b1f24fd981c47e42436e884fc6f8bcf21cdae595579af4f8a5627
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334409593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c0b670b9756542b3de4ef8777818962e61b394d7cfb369df377ad1c02e40a8`
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
# Tue, 09 Mar 2021 20:21:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:21:50 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:21:51 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:21:51 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:21:52 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:21:52 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:21:52 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:21:52 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:21:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:21:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:21:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Tue, 09 Mar 2021 20:21:53 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 09 Mar 2021 20:21:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:21:53 GMT
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
	-	`sha256:d291fb4f0928f91e0795d2434913aada7f026a7a1f125e50046e7a69884ac394`  
		Last Modified: Tue, 09 Mar 2021 20:27:18 GMT  
		Size: 256.7 MB (256740482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3d7e91874c71b2c6418a0620bdcf2054a35f5488747b6d4cc468c881dddc8`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 1.6 MB (1567815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db8d861b569a75ee8cb6fc6c6f314f90469baad901f939ad3f6ff36a2fb0f5`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dcfdf3d19d60c9007839012f54b799bfd4ed0810880a023c56cdfabc6d70cb5`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465c4372757bedac965d4511aa94f3d831b25eb00576f3e5af1b69034c07892f`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae98a63236e6f3f30f5b79e9a41dce994a83152ace9967c19b1dcdd7733c6776`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8d9f46b0d437e180e82c52a07a683d45ec02e1a41f13c6f8cf30c7c6e033c3df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362005418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fbd2db5067630bed41e54cd340eb4c619b14f8c88df2d3ae861327d2d8fc91`
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
# Sat, 14 Nov 2020 00:59:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:59:43 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:59:43 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:59:44 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:59:47 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:59:47 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:59:48 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:59:49 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:59:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:59:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:59:51 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Sat, 14 Nov 2020 00:59:51 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 14 Nov 2020 00:59:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:59:53 GMT
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
	-	`sha256:49bad1fbd2a8bc1a16aac1327fd0b3c914fb92e31a7e28ccbee40eea7abba143`  
		Last Modified: Sat, 14 Nov 2020 01:07:58 GMT  
		Size: 252.1 MB (252058525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21eca8889b53bc356fde04f0dc3a7c5473df39ed6114ca60635206f420696bd`  
		Last Modified: Sat, 14 Nov 2020 01:07:15 GMT  
		Size: 1.6 MB (1567809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cad34d17dbcdd3916787c033b12d0c15cc448443b042a3891f37d90d42342f`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7f14ef075fd2b15806b9b5883e2bb89e5f7842073772afdd00bf3141879c3c`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113bd56b4ecdd189df4693655b420d2e5d28fce50b6e07b0536a60200556c214`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40d94ac5af702ee114152210d95c40c543d1df24a6ee520570f87a03ece1f4b`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2.7`

```console
$ docker pull crate@sha256:76666715aa0e15f20b1f2d8544e0010b5ff087f4afd544623e869119b164cfad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2.7` - linux; amd64

```console
$ docker pull crate@sha256:66c5c0b0244b1f24fd981c47e42436e884fc6f8bcf21cdae595579af4f8a5627
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334409593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c0b670b9756542b3de4ef8777818962e61b394d7cfb369df377ad1c02e40a8`
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
# Tue, 09 Mar 2021 20:21:47 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:21:50 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:21:51 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:21:51 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:21:52 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:21:52 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:21:52 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:21:52 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:21:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:21:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:21:53 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Tue, 09 Mar 2021 20:21:53 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 09 Mar 2021 20:21:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:21:53 GMT
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
	-	`sha256:d291fb4f0928f91e0795d2434913aada7f026a7a1f125e50046e7a69884ac394`  
		Last Modified: Tue, 09 Mar 2021 20:27:18 GMT  
		Size: 256.7 MB (256740482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3d7e91874c71b2c6418a0620bdcf2054a35f5488747b6d4cc468c881dddc8`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 1.6 MB (1567815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db8d861b569a75ee8cb6fc6c6f314f90469baad901f939ad3f6ff36a2fb0f5`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dcfdf3d19d60c9007839012f54b799bfd4ed0810880a023c56cdfabc6d70cb5`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465c4372757bedac965d4511aa94f3d831b25eb00576f3e5af1b69034c07892f`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae98a63236e6f3f30f5b79e9a41dce994a83152ace9967c19b1dcdd7733c6776`  
		Last Modified: Tue, 09 Mar 2021 20:26:53 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.2.7` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8d9f46b0d437e180e82c52a07a683d45ec02e1a41f13c6f8cf30c7c6e033c3df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (362005418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fbd2db5067630bed41e54cd340eb4c619b14f8c88df2d3ae861327d2d8fc91`
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
# Sat, 14 Nov 2020 00:59:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:59:43 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:59:43 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:59:44 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:59:47 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:59:47 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:59:48 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:59:49 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:59:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:59:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:59:51 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Sat, 14 Nov 2020 00:59:51 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 14 Nov 2020 00:59:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:59:53 GMT
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
	-	`sha256:49bad1fbd2a8bc1a16aac1327fd0b3c914fb92e31a7e28ccbee40eea7abba143`  
		Last Modified: Sat, 14 Nov 2020 01:07:58 GMT  
		Size: 252.1 MB (252058525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21eca8889b53bc356fde04f0dc3a7c5473df39ed6114ca60635206f420696bd`  
		Last Modified: Sat, 14 Nov 2020 01:07:15 GMT  
		Size: 1.6 MB (1567809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cad34d17dbcdd3916787c033b12d0c15cc448443b042a3891f37d90d42342f`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7f14ef075fd2b15806b9b5883e2bb89e5f7842073772afdd00bf3141879c3c`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113bd56b4ecdd189df4693655b420d2e5d28fce50b6e07b0536a60200556c214`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40d94ac5af702ee114152210d95c40c543d1df24a6ee520570f87a03ece1f4b`  
		Last Modified: Sat, 14 Nov 2020 01:07:14 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.3`

```console
$ docker pull crate@sha256:221c8c519e8d56c574df1232e72e2404bef3549b3cfcb3eb38669431c94988ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.3` - linux; amd64

```console
$ docker pull crate@sha256:4480012dc3f9c8a069bf5968cebea1da68ced728dd5d96407fe0471fd07033ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333120923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4ec6cc34b429afb12f6556973417ac864a05e9b71b96bac42e97bdafe73157`
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
# Tue, 09 Mar 2021 20:20:58 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.4.tar.gz.asc crate-4.3.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.4.tar.gz.asc     && tar -xf crate-4.3.4.tar.gz -C /crate --strip-components=1     && rm crate-4.3.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:21:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:21:01 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:21:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:21:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:21:03 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:21:03 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:21:03 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:21:03 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:21:04 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:21:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-19T14:19:50.388804 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.4
# Tue, 09 Mar 2021 20:21:04 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 09 Mar 2021 20:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:21:04 GMT
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
	-	`sha256:92308b23e7a00c0a9542f45da4c5b91ef78754f6836acf1447ad5709220ffdd8`  
		Last Modified: Tue, 09 Mar 2021 20:26:35 GMT  
		Size: 255.5 MB (255451807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3836518e59cd3ab1f3b627b46c9a0553e0a947e5133c568445ff3d8af064474f`  
		Last Modified: Tue, 09 Mar 2021 20:26:13 GMT  
		Size: 1.6 MB (1567825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0eb4cd76d2bc9b904469e63b35bec6bc587164d5c70be8f0cf2624d8a3093a3`  
		Last Modified: Tue, 09 Mar 2021 20:26:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376879a821a2da5875b8b3dd95c0e067780fc3866a64470eb2473afd34ede0e`  
		Last Modified: Tue, 09 Mar 2021 20:26:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea948d45090f75eabff92e70615d5bf471576fba9ed125b2325f085c184a5d`  
		Last Modified: Tue, 09 Mar 2021 20:26:10 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417a7d1fcc2cd717f1efe41df1222b530478b4bc76b8a5204cdd7663209aa32f`  
		Last Modified: Tue, 09 Mar 2021 20:26:10 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:545c596a371eb0a8f6db83ca9311eb677a4025dd078f03bad0ca0d590b623411
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362066652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb99cc3480364cb3884223bfb120ac3393b276028f4e9edaf9d17fa6b118d45`
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
# Sat, 23 Jan 2021 00:40:53 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.4.tar.gz.asc crate-4.3.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.4.tar.gz.asc     && tar -xf crate-4.3.4.tar.gz -C /crate --strip-components=1     && rm crate-4.3.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 23 Jan 2021 00:41:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 23 Jan 2021 00:41:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Jan 2021 00:41:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 23 Jan 2021 00:41:06 GMT
RUN mkdir -p /data/data /data/log
# Sat, 23 Jan 2021 00:41:07 GMT
VOLUME [/data]
# Sat, 23 Jan 2021 00:41:08 GMT
WORKDIR /data
# Sat, 23 Jan 2021 00:41:09 GMT
EXPOSE 4200 4300 5432
# Sat, 23 Jan 2021 00:41:10 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 23 Jan 2021 00:41:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 23 Jan 2021 00:41:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-19T14:19:50.388804 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.4
# Sat, 23 Jan 2021 00:41:13 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 23 Jan 2021 00:41:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 23 Jan 2021 00:41:17 GMT
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
	-	`sha256:f89746684a218c049e6e51d393d5bc65f06c0b413ab70473da2988d67eea8780`  
		Last Modified: Sat, 23 Jan 2021 00:42:37 GMT  
		Size: 252.1 MB (252119757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed64b83e6c07e8b21fef62d63cd9c158bf15744d44c55aefe7cab330842767b`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 1.6 MB (1567815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8f4018709979aa600ebcd253bbfeb4fa84fca3f41e73cdad6c77f3e061c5`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c418344346e216978616e84e23a8aeacc29e0ae35e164eb536a8bf37bc8f8d7`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a04696aad69a7be6f75a53dc3b26c14fd4cc1bdcc321408fcbb16644ca0ed`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46b3323073af2fe3703e2e5f5bfdebf00af17ccd3f6f429c65ae1d9c7c35457`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.3.4`

```console
$ docker pull crate@sha256:221c8c519e8d56c574df1232e72e2404bef3549b3cfcb3eb38669431c94988ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.3.4` - linux; amd64

```console
$ docker pull crate@sha256:4480012dc3f9c8a069bf5968cebea1da68ced728dd5d96407fe0471fd07033ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333120923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4ec6cc34b429afb12f6556973417ac864a05e9b71b96bac42e97bdafe73157`
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
# Tue, 09 Mar 2021 20:20:58 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.4.tar.gz.asc crate-4.3.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.4.tar.gz.asc     && tar -xf crate-4.3.4.tar.gz -C /crate --strip-components=1     && rm crate-4.3.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:21:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:21:01 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:21:02 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:21:03 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:21:03 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:21:03 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:21:03 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:21:03 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:21:04 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:21:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-19T14:19:50.388804 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.4
# Tue, 09 Mar 2021 20:21:04 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 09 Mar 2021 20:21:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:21:04 GMT
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
	-	`sha256:92308b23e7a00c0a9542f45da4c5b91ef78754f6836acf1447ad5709220ffdd8`  
		Last Modified: Tue, 09 Mar 2021 20:26:35 GMT  
		Size: 255.5 MB (255451807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3836518e59cd3ab1f3b627b46c9a0553e0a947e5133c568445ff3d8af064474f`  
		Last Modified: Tue, 09 Mar 2021 20:26:13 GMT  
		Size: 1.6 MB (1567825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0eb4cd76d2bc9b904469e63b35bec6bc587164d5c70be8f0cf2624d8a3093a3`  
		Last Modified: Tue, 09 Mar 2021 20:26:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376879a821a2da5875b8b3dd95c0e067780fc3866a64470eb2473afd34ede0e`  
		Last Modified: Tue, 09 Mar 2021 20:26:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea948d45090f75eabff92e70615d5bf471576fba9ed125b2325f085c184a5d`  
		Last Modified: Tue, 09 Mar 2021 20:26:10 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417a7d1fcc2cd717f1efe41df1222b530478b4bc76b8a5204cdd7663209aa32f`  
		Last Modified: Tue, 09 Mar 2021 20:26:10 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.3.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:545c596a371eb0a8f6db83ca9311eb677a4025dd078f03bad0ca0d590b623411
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362066652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb99cc3480364cb3884223bfb120ac3393b276028f4e9edaf9d17fa6b118d45`
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
# Sat, 23 Jan 2021 00:40:53 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.4.tar.gz.asc crate-4.3.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.4.tar.gz.asc     && tar -xf crate-4.3.4.tar.gz -C /crate --strip-components=1     && rm crate-4.3.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 23 Jan 2021 00:41:01 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 23 Jan 2021 00:41:02 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Jan 2021 00:41:03 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 23 Jan 2021 00:41:06 GMT
RUN mkdir -p /data/data /data/log
# Sat, 23 Jan 2021 00:41:07 GMT
VOLUME [/data]
# Sat, 23 Jan 2021 00:41:08 GMT
WORKDIR /data
# Sat, 23 Jan 2021 00:41:09 GMT
EXPOSE 4200 4300 5432
# Sat, 23 Jan 2021 00:41:10 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 23 Jan 2021 00:41:11 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 23 Jan 2021 00:41:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-19T14:19:50.388804 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.4
# Sat, 23 Jan 2021 00:41:13 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 23 Jan 2021 00:41:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 23 Jan 2021 00:41:17 GMT
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
	-	`sha256:f89746684a218c049e6e51d393d5bc65f06c0b413ab70473da2988d67eea8780`  
		Last Modified: Sat, 23 Jan 2021 00:42:37 GMT  
		Size: 252.1 MB (252119757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed64b83e6c07e8b21fef62d63cd9c158bf15744d44c55aefe7cab330842767b`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 1.6 MB (1567815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae8f4018709979aa600ebcd253bbfeb4fa84fca3f41e73cdad6c77f3e061c5`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c418344346e216978616e84e23a8aeacc29e0ae35e164eb536a8bf37bc8f8d7`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a04696aad69a7be6f75a53dc3b26c14fd4cc1bdcc321408fcbb16644ca0ed`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46b3323073af2fe3703e2e5f5bfdebf00af17ccd3f6f429c65ae1d9c7c35457`  
		Last Modified: Sat, 23 Jan 2021 00:41:59 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.4`

```console
$ docker pull crate@sha256:5253f283d636b8529d8a09e304bf895dd180af00783760b783338a439222bc55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.4` - linux; amd64

```console
$ docker pull crate@sha256:f71aa52c365e3d4563596dabd6d910957df589818d053e34c18bf46833f9aeca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333349777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e121af4830819912c731095f9031c675e6b6ede30f3bfd9b1b74e7ac808d0251`
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
# Tue, 09 Mar 2021 20:20:14 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.2.tar.gz.asc crate-4.4.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.2.tar.gz.asc     && tar -xf crate-4.4.2.tar.gz -C /crate --strip-components=1     && rm crate-4.4.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:20:19 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:20:19 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:20:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:20:20 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:20:20 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:20:20 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:20:20 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:20:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:20:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:20:21 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-02T12:28:51.122703 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.2
# Tue, 09 Mar 2021 20:20:21 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 09 Mar 2021 20:20:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:20:22 GMT
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
	-	`sha256:87ef33954498c60906eb2f6cd9dffe74bf9f44e507bec2aa1f8cd7488bfadd42`  
		Last Modified: Tue, 09 Mar 2021 20:25:54 GMT  
		Size: 255.7 MB (255680656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214b9598db8d12188af360d2562431278b65508282a4464feabe7c8e81426e40`  
		Last Modified: Tue, 09 Mar 2021 20:25:30 GMT  
		Size: 1.6 MB (1567826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65921ee79768cccf1dd00b81a077c5dc5058814946a5f5e7f60db2551758603a`  
		Last Modified: Tue, 09 Mar 2021 20:25:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cf72326ab57c854c08c0ad21639df36576b4cac3cfadcfafeed766d1656f28`  
		Last Modified: Tue, 09 Mar 2021 20:25:29 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb391120c341beb9eb51b376193bd5438bbddc26883c3592bff0990de2ff63a`  
		Last Modified: Tue, 09 Mar 2021 20:25:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c948863953e674a3f682d854e63023ef421c02521adbc1f5495bcf4acb263c30`  
		Last Modified: Tue, 09 Mar 2021 20:25:31 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f0e5bf2750bbe0ad2fdb3c01f9a7e54b2c60af07eb2af9b7f80bde56750793b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362399891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffa699e7afb89388d42c3996c99a2c2405541f5c5b9a90225d863998e0e1ba6`
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
# Fri, 26 Mar 2021 13:16:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Fri, 26 Mar 2021 13:16:16 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 26 Mar 2021 13:16:18 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 13:16:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 26 Mar 2021 13:16:23 GMT
RUN mkdir -p /data/data /data/log
# Fri, 26 Mar 2021 13:16:24 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 13:16:26 GMT
WORKDIR /data
# Fri, 26 Mar 2021 13:16:27 GMT
EXPOSE 4200 4300 5432
# Fri, 26 Mar 2021 13:16:29 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 26 Mar 2021 13:16:31 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 26 Mar 2021 13:16:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Fri, 26 Mar 2021 13:16:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 26 Mar 2021 13:16:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 26 Mar 2021 13:16:35 GMT
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
	-	`sha256:afd33dab412422921b82b88c88545801695aa7ad0a124218a257bd2b0aa3234e`  
		Last Modified: Fri, 26 Mar 2021 13:18:08 GMT  
		Size: 252.4 MB (252438619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9af035964e10f47a18e690d6876bf754df09c370b03b1950c66470485e66b0`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 1.6 MB (1582193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b489f5a9970b20492efef536af0287b2b6a46f70b0775dd621da048580b2bca2`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a87f16501a0fd58d065168c3913c014d940fe2e684dc451665b3effa819ae1`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db167b96a0c70c2bfcc863c28514bdbb9a3321033bd7c72f2c56679bf239ccb4`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c04c6eca1cdad4f0cec294ed3e24e27378f653d333f52037edb909c09cc0dc5`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.4.3`

```console
$ docker pull crate@sha256:820ddc8f51418dce87208f9e8b47395897dd5ce7e3a0c99c0f0d498966d53a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `crate:4.4.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f0e5bf2750bbe0ad2fdb3c01f9a7e54b2c60af07eb2af9b7f80bde56750793b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362399891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffa699e7afb89388d42c3996c99a2c2405541f5c5b9a90225d863998e0e1ba6`
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
# Fri, 26 Mar 2021 13:16:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Fri, 26 Mar 2021 13:16:16 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 26 Mar 2021 13:16:18 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 13:16:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 26 Mar 2021 13:16:23 GMT
RUN mkdir -p /data/data /data/log
# Fri, 26 Mar 2021 13:16:24 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 13:16:26 GMT
WORKDIR /data
# Fri, 26 Mar 2021 13:16:27 GMT
EXPOSE 4200 4300 5432
# Fri, 26 Mar 2021 13:16:29 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 26 Mar 2021 13:16:31 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 26 Mar 2021 13:16:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Fri, 26 Mar 2021 13:16:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 26 Mar 2021 13:16:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 26 Mar 2021 13:16:35 GMT
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
	-	`sha256:afd33dab412422921b82b88c88545801695aa7ad0a124218a257bd2b0aa3234e`  
		Last Modified: Fri, 26 Mar 2021 13:18:08 GMT  
		Size: 252.4 MB (252438619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9af035964e10f47a18e690d6876bf754df09c370b03b1950c66470485e66b0`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 1.6 MB (1582193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b489f5a9970b20492efef536af0287b2b6a46f70b0775dd621da048580b2bca2`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a87f16501a0fd58d065168c3913c014d940fe2e684dc451665b3effa819ae1`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db167b96a0c70c2bfcc863c28514bdbb9a3321033bd7c72f2c56679bf239ccb4`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c04c6eca1cdad4f0cec294ed3e24e27378f653d333f52037edb909c09cc0dc5`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:5253f283d636b8529d8a09e304bf895dd180af00783760b783338a439222bc55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:f71aa52c365e3d4563596dabd6d910957df589818d053e34c18bf46833f9aeca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333349777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e121af4830819912c731095f9031c675e6b6ede30f3bfd9b1b74e7ac808d0251`
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
# Tue, 09 Mar 2021 20:20:14 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.2.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.2.tar.gz.asc crate-4.4.2.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.2.tar.gz.asc     && tar -xf crate-4.4.2.tar.gz -C /crate --strip-components=1     && rm crate-4.4.2.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 09 Mar 2021 20:20:19 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 09 Mar 2021 20:20:19 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:20:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Mar 2021 20:20:20 GMT
RUN mkdir -p /data/data /data/log
# Tue, 09 Mar 2021 20:20:20 GMT
VOLUME [/data]
# Tue, 09 Mar 2021 20:20:20 GMT
WORKDIR /data
# Tue, 09 Mar 2021 20:20:20 GMT
EXPOSE 4200 4300 5432
# Tue, 09 Mar 2021 20:20:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 09 Mar 2021 20:20:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 09 Mar 2021 20:20:21 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-02T12:28:51.122703 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.2
# Tue, 09 Mar 2021 20:20:21 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 09 Mar 2021 20:20:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Mar 2021 20:20:22 GMT
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
	-	`sha256:87ef33954498c60906eb2f6cd9dffe74bf9f44e507bec2aa1f8cd7488bfadd42`  
		Last Modified: Tue, 09 Mar 2021 20:25:54 GMT  
		Size: 255.7 MB (255680656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214b9598db8d12188af360d2562431278b65508282a4464feabe7c8e81426e40`  
		Last Modified: Tue, 09 Mar 2021 20:25:30 GMT  
		Size: 1.6 MB (1567826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65921ee79768cccf1dd00b81a077c5dc5058814946a5f5e7f60db2551758603a`  
		Last Modified: Tue, 09 Mar 2021 20:25:29 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cf72326ab57c854c08c0ad21639df36576b4cac3cfadcfafeed766d1656f28`  
		Last Modified: Tue, 09 Mar 2021 20:25:29 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb391120c341beb9eb51b376193bd5438bbddc26883c3592bff0990de2ff63a`  
		Last Modified: Tue, 09 Mar 2021 20:25:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c948863953e674a3f682d854e63023ef421c02521adbc1f5495bcf4acb263c30`  
		Last Modified: Tue, 09 Mar 2021 20:25:31 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:f0e5bf2750bbe0ad2fdb3c01f9a7e54b2c60af07eb2af9b7f80bde56750793b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362399891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffa699e7afb89388d42c3996c99a2c2405541f5c5b9a90225d863998e0e1ba6`
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
# Fri, 26 Mar 2021 13:16:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Fri, 26 Mar 2021 13:16:16 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 26 Mar 2021 13:16:18 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 13:16:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 26 Mar 2021 13:16:23 GMT
RUN mkdir -p /data/data /data/log
# Fri, 26 Mar 2021 13:16:24 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 13:16:26 GMT
WORKDIR /data
# Fri, 26 Mar 2021 13:16:27 GMT
EXPOSE 4200 4300 5432
# Fri, 26 Mar 2021 13:16:29 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 26 Mar 2021 13:16:31 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 26 Mar 2021 13:16:32 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Fri, 26 Mar 2021 13:16:33 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 26 Mar 2021 13:16:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 26 Mar 2021 13:16:35 GMT
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
	-	`sha256:afd33dab412422921b82b88c88545801695aa7ad0a124218a257bd2b0aa3234e`  
		Last Modified: Fri, 26 Mar 2021 13:18:08 GMT  
		Size: 252.4 MB (252438619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9af035964e10f47a18e690d6876bf754df09c370b03b1950c66470485e66b0`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 1.6 MB (1582193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b489f5a9970b20492efef536af0287b2b6a46f70b0775dd621da048580b2bca2`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a87f16501a0fd58d065168c3913c014d940fe2e684dc451665b3effa819ae1`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db167b96a0c70c2bfcc863c28514bdbb9a3321033bd7c72f2c56679bf239ccb4`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c04c6eca1cdad4f0cec294ed3e24e27378f653d333f52037edb909c09cc0dc5`  
		Last Modified: Fri, 26 Mar 2021 13:17:28 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
