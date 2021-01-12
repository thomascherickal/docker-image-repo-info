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
-	[`crate:4.3.3`](#crate433)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:4f731f461c39083864777f4e50aac9048a8f7a4b48064b618e85a7e207fea602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:3.3` - linux; amd64

```console
$ docker pull crate@sha256:72a0b83bb3b5a2b761b0e70f81fafa614a9e9f825f8078b4886eb0b12040327b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.7 MB (344665952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dea0ade687ad0f526965fafef55329ab2af4d0290ee39fb21ad760b5c83c05`
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
# Sat, 14 Nov 2020 00:41:40 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 00:41:41 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Sat, 14 Nov 2020 00:41:42 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 00:42:02 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 00:42:03 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:42:03 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:42:04 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:42:05 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:42:05 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:42:06 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:42:06 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:42:06 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:42:06 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:42:07 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:42:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:42:07 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Sat, 14 Nov 2020 00:42:07 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 00:42:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:42:08 GMT
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
	-	`sha256:b2e0c50ab0d913b3a623ce34e90286d08d4b519e8f0e8914d1f78d4371d40f39`  
		Last Modified: Sat, 14 Nov 2020 00:44:49 GMT  
		Size: 188.1 MB (188101419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e587c52754ce105700af8f83a4d1efdc09949ec6ae629eff7f34561c0a44a1`  
		Last Modified: Sat, 14 Nov 2020 00:44:30 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c4b36ee4cdb3c11fdae87d6085c4f4932938aad1a4a7d6b0233102606d360e`  
		Last Modified: Sat, 14 Nov 2020 00:44:40 GMT  
		Size: 79.2 MB (79167696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa330b1af4fec0108d1c5f96b0d6da4d861a7db3b3bbad7f46d3555ebe875f5`  
		Last Modified: Sat, 14 Nov 2020 00:44:30 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0682885f8007f09f5a6e50c3c7e3025b670c269e6e28c4bbd9c1f158427bfe7`  
		Last Modified: Sat, 14 Nov 2020 00:44:31 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defcccec4fb6e6a14e796210e9138a57107c4dbe88164295d776c4b99a725811`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 1.3 MB (1294141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2d0299e47ce78e5b7d3fd37d43942de3c28d7fe35f729f6b43b2f8fdb009a`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958de259d214785907b3b76540af0e0161f06df20e30de4ad90ad8884b3b26fb`  
		Last Modified: Sat, 14 Nov 2020 00:44:28 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9278b45ccbb4e19151ba677d2adbb0bef8bce64ff46ac5c4d996587afe6a927d`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ef33062daed1b1f36c6874ebd520be388eaf8c0306ab79c0640f2d28331e6`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 527.0 B  
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
$ docker pull crate@sha256:4f731f461c39083864777f4e50aac9048a8f7a4b48064b618e85a7e207fea602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:3.3.5` - linux; amd64

```console
$ docker pull crate@sha256:72a0b83bb3b5a2b761b0e70f81fafa614a9e9f825f8078b4886eb0b12040327b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.7 MB (344665952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dea0ade687ad0f526965fafef55329ab2af4d0290ee39fb21ad760b5c83c05`
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
# Sat, 14 Nov 2020 00:41:40 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 00:41:41 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Sat, 14 Nov 2020 00:41:42 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 00:42:02 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 00:42:03 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:42:03 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:42:04 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:42:05 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:42:05 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:42:06 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:42:06 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:42:06 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:42:06 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:42:07 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:42:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:42:07 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Sat, 14 Nov 2020 00:42:07 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 00:42:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:42:08 GMT
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
	-	`sha256:b2e0c50ab0d913b3a623ce34e90286d08d4b519e8f0e8914d1f78d4371d40f39`  
		Last Modified: Sat, 14 Nov 2020 00:44:49 GMT  
		Size: 188.1 MB (188101419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e587c52754ce105700af8f83a4d1efdc09949ec6ae629eff7f34561c0a44a1`  
		Last Modified: Sat, 14 Nov 2020 00:44:30 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c4b36ee4cdb3c11fdae87d6085c4f4932938aad1a4a7d6b0233102606d360e`  
		Last Modified: Sat, 14 Nov 2020 00:44:40 GMT  
		Size: 79.2 MB (79167696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa330b1af4fec0108d1c5f96b0d6da4d861a7db3b3bbad7f46d3555ebe875f5`  
		Last Modified: Sat, 14 Nov 2020 00:44:30 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0682885f8007f09f5a6e50c3c7e3025b670c269e6e28c4bbd9c1f158427bfe7`  
		Last Modified: Sat, 14 Nov 2020 00:44:31 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defcccec4fb6e6a14e796210e9138a57107c4dbe88164295d776c4b99a725811`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 1.3 MB (1294141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2d0299e47ce78e5b7d3fd37d43942de3c28d7fe35f729f6b43b2f8fdb009a`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958de259d214785907b3b76540af0e0161f06df20e30de4ad90ad8884b3b26fb`  
		Last Modified: Sat, 14 Nov 2020 00:44:28 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9278b45ccbb4e19151ba677d2adbb0bef8bce64ff46ac5c4d996587afe6a927d`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ef33062daed1b1f36c6874ebd520be388eaf8c0306ab79c0640f2d28331e6`  
		Last Modified: Sat, 14 Nov 2020 00:44:29 GMT  
		Size: 527.0 B  
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
$ docker pull crate@sha256:d884fa7fa3927342ad65a336513c71589e0286a09471f17baa72fc15af0112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0` - linux; amd64

```console
$ docker pull crate@sha256:541f153a10b9589c33b2c76f6c15dab468757cf11313e9b5a6809fc89a4f7c9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338171832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2258e32b29552d77a6dc691358798ae9c4a936f88a360042fe289918fb38cc6a`
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
# Sat, 14 Nov 2020 00:40:37 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 00:40:37 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Sat, 14 Nov 2020 00:40:38 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 00:40:54 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 00:40:54 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:40:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:40:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:40:56 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:40:56 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:40:57 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:40:58 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:40:58 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:40:58 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:40:58 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:40:58 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:40:59 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Sat, 14 Nov 2020 00:40:59 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 00:40:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:40:59 GMT
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
	-	`sha256:709b24dce602c9fea975ce137e7220d377e4c8a55e7599bd8178e947f66becc2`  
		Last Modified: Sat, 14 Nov 2020 00:44:22 GMT  
		Size: 198.1 MB (198127883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633f5a4915402b145ca27e3ab4e99f9143c87733b526df616a604df70667e24e`  
		Last Modified: Sat, 14 Nov 2020 00:44:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc5763ff7e9a8e017294df072a56f28320a42f97503cb534f0a6127503e745`  
		Last Modified: Sat, 14 Nov 2020 00:44:09 GMT  
		Size: 62.6 MB (62647106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a2e0f9357f4f21d99e3eebc9dd45eb4dce76351844d1ec9bd8d33c1b6ea561`  
		Last Modified: Sat, 14 Nov 2020 00:44:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b0518dbaaee4c12263bc2352d8d63e19a36746dd1374828c8f1b0325b0448`  
		Last Modified: Sat, 14 Nov 2020 00:44:02 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5ea4e96e27868887e297780b1805185483203bc272a00515243dd822efce94`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 1.3 MB (1294145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa03700f5298f4c33082db02d20510ad49ca5b5b243829ca64604bf9e260906`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0220e4f80681bf78c381144e48edc851551849a496ad72235e05398bef68ffe`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfe2f91e01780224c62ca6e1f4a754250948a396815a4f0d6b1f79c2f922532`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d75f39e71fd643041c34f5202506507d1f8ab022d9ee119688b8856b2d9808a`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 529.0 B  
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
$ docker pull crate@sha256:d884fa7fa3927342ad65a336513c71589e0286a09471f17baa72fc15af0112c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0.12` - linux; amd64

```console
$ docker pull crate@sha256:541f153a10b9589c33b2c76f6c15dab468757cf11313e9b5a6809fc89a4f7c9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338171832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2258e32b29552d77a6dc691358798ae9c4a936f88a360042fe289918fb38cc6a`
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
# Sat, 14 Nov 2020 00:40:37 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 00:40:37 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Sat, 14 Nov 2020 00:40:38 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 00:40:54 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Sat, 14 Nov 2020 00:40:54 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:40:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:40:56 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:40:56 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:40:56 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:40:57 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:40:58 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:40:58 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:40:58 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:40:58 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:40:58 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:40:59 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Sat, 14 Nov 2020 00:40:59 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 00:40:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:40:59 GMT
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
	-	`sha256:709b24dce602c9fea975ce137e7220d377e4c8a55e7599bd8178e947f66becc2`  
		Last Modified: Sat, 14 Nov 2020 00:44:22 GMT  
		Size: 198.1 MB (198127883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633f5a4915402b145ca27e3ab4e99f9143c87733b526df616a604df70667e24e`  
		Last Modified: Sat, 14 Nov 2020 00:44:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc5763ff7e9a8e017294df072a56f28320a42f97503cb534f0a6127503e745`  
		Last Modified: Sat, 14 Nov 2020 00:44:09 GMT  
		Size: 62.6 MB (62647106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a2e0f9357f4f21d99e3eebc9dd45eb4dce76351844d1ec9bd8d33c1b6ea561`  
		Last Modified: Sat, 14 Nov 2020 00:44:03 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b0518dbaaee4c12263bc2352d8d63e19a36746dd1374828c8f1b0325b0448`  
		Last Modified: Sat, 14 Nov 2020 00:44:02 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5ea4e96e27868887e297780b1805185483203bc272a00515243dd822efce94`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 1.3 MB (1294145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa03700f5298f4c33082db02d20510ad49ca5b5b243829ca64604bf9e260906`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0220e4f80681bf78c381144e48edc851551849a496ad72235e05398bef68ffe`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfe2f91e01780224c62ca6e1f4a754250948a396815a4f0d6b1f79c2f922532`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d75f39e71fd643041c34f5202506507d1f8ab022d9ee119688b8856b2d9808a`  
		Last Modified: Sat, 14 Nov 2020 00:44:01 GMT  
		Size: 529.0 B  
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
$ docker pull crate@sha256:ac609ea2b1df19257b3daa644b6723cbc96a713f52d0a43af61171ace927f371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1` - linux; amd64

```console
$ docker pull crate@sha256:24caecfc1c57349105e2cd22b608782d0f1786496e6c593722decd896021ed9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351246674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f45ee62ac165007f458cebe91847b94d4b83927e19280604f01fdae4aef464`
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
# Sat, 14 Nov 2020 00:39:21 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 00:39:22 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Sat, 14 Nov 2020 00:39:23 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 00:39:48 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:39:51 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:39:51 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:39:51 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:39:52 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:39:53 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:39:53 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:39:53 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:39:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:39:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:39:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Sat, 14 Nov 2020 00:39:54 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 00:39:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:39:54 GMT
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
	-	`sha256:84b08ca39740a63c11eb27d866063d282770c98e7885f836496a2cb5aed0cc2c`  
		Last Modified: Sat, 14 Nov 2020 00:43:53 GMT  
		Size: 196.4 MB (196423227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cad712ed81f86a2d63dd8e419e7362122b130094fe07d15bbec02e647c609b`  
		Last Modified: Sat, 14 Nov 2020 00:43:35 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40038a989f4cb252af5a97d4790a969c115e52d0611458c31d6114e1c3b8f10`  
		Last Modified: Sat, 14 Nov 2020 00:43:43 GMT  
		Size: 77.4 MB (77427821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0954a97766736556f52105ef44ece38680fc2d61782fa1956e2005703344c8be`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 1.3 MB (1294153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5f1069478fe97ca25c9504a3c51046f5b87803cba6f4324c90955dd587c68f`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf995fdb3a06cd67c10335df0dbe2cf6b34aa3c6cc250ae35ea5b8fcac4da11`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3301a45d866be3550c10f67a2a291fc396f9add14785f90690ba094a80a1f2dd`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bacf3c2078160e88ce3a12445111c74f87db2a9472af6f553de406961901ffb`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
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
$ docker pull crate@sha256:ac609ea2b1df19257b3daa644b6723cbc96a713f52d0a43af61171ace927f371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1.8` - linux; amd64

```console
$ docker pull crate@sha256:24caecfc1c57349105e2cd22b608782d0f1786496e6c593722decd896021ed9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351246674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f45ee62ac165007f458cebe91847b94d4b83927e19280604f01fdae4aef464`
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
# Sat, 14 Nov 2020 00:39:21 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Sat, 14 Nov 2020 00:39:22 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Sat, 14 Nov 2020 00:39:23 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Sat, 14 Nov 2020 00:39:48 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:39:51 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:39:51 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:39:51 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:39:52 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:39:53 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:39:53 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:39:53 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:39:53 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:39:54 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:39:54 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Sat, 14 Nov 2020 00:39:54 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Sat, 14 Nov 2020 00:39:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:39:54 GMT
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
	-	`sha256:84b08ca39740a63c11eb27d866063d282770c98e7885f836496a2cb5aed0cc2c`  
		Last Modified: Sat, 14 Nov 2020 00:43:53 GMT  
		Size: 196.4 MB (196423227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cad712ed81f86a2d63dd8e419e7362122b130094fe07d15bbec02e647c609b`  
		Last Modified: Sat, 14 Nov 2020 00:43:35 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40038a989f4cb252af5a97d4790a969c115e52d0611458c31d6114e1c3b8f10`  
		Last Modified: Sat, 14 Nov 2020 00:43:43 GMT  
		Size: 77.4 MB (77427821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0954a97766736556f52105ef44ece38680fc2d61782fa1956e2005703344c8be`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 1.3 MB (1294153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5f1069478fe97ca25c9504a3c51046f5b87803cba6f4324c90955dd587c68f`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf995fdb3a06cd67c10335df0dbe2cf6b34aa3c6cc250ae35ea5b8fcac4da11`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3301a45d866be3550c10f67a2a291fc396f9add14785f90690ba094a80a1f2dd`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bacf3c2078160e88ce3a12445111c74f87db2a9472af6f553de406961901ffb`  
		Last Modified: Sat, 14 Nov 2020 00:43:33 GMT  
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
$ docker pull crate@sha256:aa1140e91e99e9c9cd05a79c5ac206bb10da26c4b1eb2db148d0989d74e0e006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2` - linux; amd64

```console
$ docker pull crate@sha256:f9e62e295f02353af94fcfd68f8ec50005738444f03e9553b416b399151f5a8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (332974301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69786fab753233c1e0b152f55358ce36083477e8ae0a5ef874baad1df26698d3`
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
# Sat, 14 Nov 2020 00:38:54 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:38:57 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:38:57 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:38:57 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:38:59 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:38:59 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:38:59 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:38:59 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:39:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:39:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:39:00 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Sat, 14 Nov 2020 00:39:00 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 14 Nov 2020 00:39:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:39:01 GMT
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
	-	`sha256:52f71680ff3d1777267c3c99ef75d3157075563412c9c607250b0a60af48d601`  
		Last Modified: Sat, 14 Nov 2020 00:43:24 GMT  
		Size: 255.3 MB (255305250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa83cbfa0d36d5b75bffcae8d8b45d4a3ab6e695b86c5849e6e7cb280817960`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 1.6 MB (1567814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb40b4a220e057ca8880dd80c2f5199c266f786bb9fbdc58911aa6522b5b3ed6`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750749da036803138bfa91f962fe8e0e6004cb46934e4f761985b93883c3c02`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4cc683a3d86ca84690ede161e388ae05facf1523519fba6aca83a5ab2fdec`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc004187b072627aa924f9d7ce601ceeda3f81613a60db9eee0957f4c754de4`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 504.0 B  
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
$ docker pull crate@sha256:aa1140e91e99e9c9cd05a79c5ac206bb10da26c4b1eb2db148d0989d74e0e006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2.7` - linux; amd64

```console
$ docker pull crate@sha256:f9e62e295f02353af94fcfd68f8ec50005738444f03e9553b416b399151f5a8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (332974301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69786fab753233c1e0b152f55358ce36083477e8ae0a5ef874baad1df26698d3`
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
# Sat, 14 Nov 2020 00:38:54 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Sat, 14 Nov 2020 00:38:57 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Sat, 14 Nov 2020 00:38:57 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 14 Nov 2020 00:38:57 GMT
ENV CRATE_HEAP_SIZE=512M
# Sat, 14 Nov 2020 00:38:59 GMT
RUN mkdir -p /data/data /data/log
# Sat, 14 Nov 2020 00:38:59 GMT
VOLUME [/data]
# Sat, 14 Nov 2020 00:38:59 GMT
WORKDIR /data
# Sat, 14 Nov 2020 00:38:59 GMT
EXPOSE 4200 4300 5432
# Sat, 14 Nov 2020 00:39:00 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Sat, 14 Nov 2020 00:39:00 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Sat, 14 Nov 2020 00:39:00 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Sat, 14 Nov 2020 00:39:00 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Sat, 14 Nov 2020 00:39:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 00:39:01 GMT
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
	-	`sha256:52f71680ff3d1777267c3c99ef75d3157075563412c9c607250b0a60af48d601`  
		Last Modified: Sat, 14 Nov 2020 00:43:24 GMT  
		Size: 255.3 MB (255305250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa83cbfa0d36d5b75bffcae8d8b45d4a3ab6e695b86c5849e6e7cb280817960`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 1.6 MB (1567814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb40b4a220e057ca8880dd80c2f5199c266f786bb9fbdc58911aa6522b5b3ed6`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750749da036803138bfa91f962fe8e0e6004cb46934e4f761985b93883c3c02`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d4cc683a3d86ca84690ede161e388ae05facf1523519fba6aca83a5ab2fdec`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc004187b072627aa924f9d7ce601ceeda3f81613a60db9eee0957f4c754de4`  
		Last Modified: Sat, 14 Nov 2020 00:42:57 GMT  
		Size: 504.0 B  
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
$ docker pull crate@sha256:3fd93f58231576e27e3410ce89753caec706b5c16d8107e4634c12a43bd0d613
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.3` - linux; amd64

```console
$ docker pull crate@sha256:47f4c283d5583b3817ca47e635166a3127345e18aacebf7def355b29a157282d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332740935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e806c51373744fd46cbd27adbe1fca45f6bd4bc3c69bc28b834759bdfa2d08c7`
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
# Tue, 12 Jan 2021 00:30:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.3.tar.gz.asc crate-4.3.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.3.tar.gz.asc     && tar -xf crate-4.3.3.tar.gz -C /crate --strip-components=1     && rm crate-4.3.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 12 Jan 2021 00:30:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 12 Jan 2021 00:30:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 00:30:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 12 Jan 2021 00:30:21 GMT
RUN mkdir -p /data/data /data/log
# Tue, 12 Jan 2021 00:30:22 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 00:30:22 GMT
WORKDIR /data
# Tue, 12 Jan 2021 00:30:22 GMT
EXPOSE 4200 4300 5432
# Tue, 12 Jan 2021 00:30:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Jan 2021 00:30:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Jan 2021 00:30:23 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-06T13:49:59.918942 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.3
# Tue, 12 Jan 2021 00:30:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 12 Jan 2021 00:30:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:30:23 GMT
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
	-	`sha256:22d1daca1ee8464c5952c258eaf51c30dfbc6217b2da9085a584b192b6bfcf88`  
		Last Modified: Tue, 12 Jan 2021 00:31:27 GMT  
		Size: 255.1 MB (255071873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922309b38ee41ce43c9f5aae3cb1b310831aee721ef4cc0ca4e1342ddad3f726`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 1.6 MB (1567827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfe390c691e9f882c5177921d39981973b7fc9cd12f12b7f776cbfcff3765de`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d52fd762724ae28092402a64a63c91fe752881d9f24fb208bac99a66af28d5`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9748f4d2e954dba0ccf95c3ad9ddb70856640e5803386a289c5fed5f2e803f6`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec8faa127363d72abbf4e78d9e4cd709eab5f7d6680f2e1c207ab78200238b`  
		Last Modified: Tue, 12 Jan 2021 00:31:02 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8223e2f6a253394aade82f137d4a4ee75850b3a10ac07f2f77d884818a6bc2aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.7 MB (361704668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f19b6ce48819d324fc8f34e1c3e5bf4ff0b859a9ca80fd7714b79072f469471`
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
# Mon, 11 Jan 2021 23:41:07 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.3.tar.gz.asc crate-4.3.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.3.tar.gz.asc     && tar -xf crate-4.3.3.tar.gz -C /crate --strip-components=1     && rm crate-4.3.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 11 Jan 2021 23:41:15 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Jan 2021 23:41:16 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Jan 2021 23:41:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Jan 2021 23:41:18 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Jan 2021 23:41:19 GMT
VOLUME [/data]
# Mon, 11 Jan 2021 23:41:20 GMT
WORKDIR /data
# Mon, 11 Jan 2021 23:41:20 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Jan 2021 23:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Jan 2021 23:41:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Jan 2021 23:41:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-06T13:49:59.918942 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.3
# Mon, 11 Jan 2021 23:41:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Jan 2021 23:41:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:41:24 GMT
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
	-	`sha256:6462066fbb7066c2d1d471f5f80480f5ab255c808156e607bba5ccdbb5645af9`  
		Last Modified: Mon, 11 Jan 2021 23:43:02 GMT  
		Size: 251.8 MB (251757765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b79aec7edb98837e07ce03e121c1e53fa2d7bd461ce193b97e53d9c9c25fef2`  
		Last Modified: Mon, 11 Jan 2021 23:42:22 GMT  
		Size: 1.6 MB (1567819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e6c15b4f707e090888017515775218b8607eb833fb5f8f69fd0aad6b85b1a1`  
		Last Modified: Mon, 11 Jan 2021 23:42:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ec98997042e5a3a67e8be78395c2f4242a336757ec73072aee56374d9f30a`  
		Last Modified: Mon, 11 Jan 2021 23:42:23 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9060a930557208ce82b3093c151b1f99aac6babbb92ddc3a865600d7312173e0`  
		Last Modified: Mon, 11 Jan 2021 23:42:23 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf77334e8035e468e8ef580cb7d57f9c9839781b851bd24558c207a1b6c26b`  
		Last Modified: Mon, 11 Jan 2021 23:42:24 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.3.3`

```console
$ docker pull crate@sha256:3fd93f58231576e27e3410ce89753caec706b5c16d8107e4634c12a43bd0d613
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.3.3` - linux; amd64

```console
$ docker pull crate@sha256:47f4c283d5583b3817ca47e635166a3127345e18aacebf7def355b29a157282d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332740935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e806c51373744fd46cbd27adbe1fca45f6bd4bc3c69bc28b834759bdfa2d08c7`
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
# Tue, 12 Jan 2021 00:30:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.3.tar.gz.asc crate-4.3.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.3.tar.gz.asc     && tar -xf crate-4.3.3.tar.gz -C /crate --strip-components=1     && rm crate-4.3.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 12 Jan 2021 00:30:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 12 Jan 2021 00:30:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 00:30:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 12 Jan 2021 00:30:21 GMT
RUN mkdir -p /data/data /data/log
# Tue, 12 Jan 2021 00:30:22 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 00:30:22 GMT
WORKDIR /data
# Tue, 12 Jan 2021 00:30:22 GMT
EXPOSE 4200 4300 5432
# Tue, 12 Jan 2021 00:30:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Jan 2021 00:30:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Jan 2021 00:30:23 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-06T13:49:59.918942 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.3
# Tue, 12 Jan 2021 00:30:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 12 Jan 2021 00:30:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:30:23 GMT
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
	-	`sha256:22d1daca1ee8464c5952c258eaf51c30dfbc6217b2da9085a584b192b6bfcf88`  
		Last Modified: Tue, 12 Jan 2021 00:31:27 GMT  
		Size: 255.1 MB (255071873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922309b38ee41ce43c9f5aae3cb1b310831aee721ef4cc0ca4e1342ddad3f726`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 1.6 MB (1567827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfe390c691e9f882c5177921d39981973b7fc9cd12f12b7f776cbfcff3765de`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d52fd762724ae28092402a64a63c91fe752881d9f24fb208bac99a66af28d5`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9748f4d2e954dba0ccf95c3ad9ddb70856640e5803386a289c5fed5f2e803f6`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec8faa127363d72abbf4e78d9e4cd709eab5f7d6680f2e1c207ab78200238b`  
		Last Modified: Tue, 12 Jan 2021 00:31:02 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.3.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8223e2f6a253394aade82f137d4a4ee75850b3a10ac07f2f77d884818a6bc2aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.7 MB (361704668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f19b6ce48819d324fc8f34e1c3e5bf4ff0b859a9ca80fd7714b79072f469471`
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
# Mon, 11 Jan 2021 23:41:07 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.3.tar.gz.asc crate-4.3.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.3.tar.gz.asc     && tar -xf crate-4.3.3.tar.gz -C /crate --strip-components=1     && rm crate-4.3.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 11 Jan 2021 23:41:15 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Jan 2021 23:41:16 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Jan 2021 23:41:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Jan 2021 23:41:18 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Jan 2021 23:41:19 GMT
VOLUME [/data]
# Mon, 11 Jan 2021 23:41:20 GMT
WORKDIR /data
# Mon, 11 Jan 2021 23:41:20 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Jan 2021 23:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Jan 2021 23:41:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Jan 2021 23:41:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-06T13:49:59.918942 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.3
# Mon, 11 Jan 2021 23:41:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Jan 2021 23:41:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:41:24 GMT
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
	-	`sha256:6462066fbb7066c2d1d471f5f80480f5ab255c808156e607bba5ccdbb5645af9`  
		Last Modified: Mon, 11 Jan 2021 23:43:02 GMT  
		Size: 251.8 MB (251757765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b79aec7edb98837e07ce03e121c1e53fa2d7bd461ce193b97e53d9c9c25fef2`  
		Last Modified: Mon, 11 Jan 2021 23:42:22 GMT  
		Size: 1.6 MB (1567819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e6c15b4f707e090888017515775218b8607eb833fb5f8f69fd0aad6b85b1a1`  
		Last Modified: Mon, 11 Jan 2021 23:42:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ec98997042e5a3a67e8be78395c2f4242a336757ec73072aee56374d9f30a`  
		Last Modified: Mon, 11 Jan 2021 23:42:23 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9060a930557208ce82b3093c151b1f99aac6babbb92ddc3a865600d7312173e0`  
		Last Modified: Mon, 11 Jan 2021 23:42:23 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf77334e8035e468e8ef580cb7d57f9c9839781b851bd24558c207a1b6c26b`  
		Last Modified: Mon, 11 Jan 2021 23:42:24 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:3fd93f58231576e27e3410ce89753caec706b5c16d8107e4634c12a43bd0d613
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:47f4c283d5583b3817ca47e635166a3127345e18aacebf7def355b29a157282d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332740935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e806c51373744fd46cbd27adbe1fca45f6bd4bc3c69bc28b834759bdfa2d08c7`
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
# Tue, 12 Jan 2021 00:30:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.3.tar.gz.asc crate-4.3.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.3.tar.gz.asc     && tar -xf crate-4.3.3.tar.gz -C /crate --strip-components=1     && rm crate-4.3.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Tue, 12 Jan 2021 00:30:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 12 Jan 2021 00:30:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 00:30:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 12 Jan 2021 00:30:21 GMT
RUN mkdir -p /data/data /data/log
# Tue, 12 Jan 2021 00:30:22 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 00:30:22 GMT
WORKDIR /data
# Tue, 12 Jan 2021 00:30:22 GMT
EXPOSE 4200 4300 5432
# Tue, 12 Jan 2021 00:30:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Jan 2021 00:30:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Jan 2021 00:30:23 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-06T13:49:59.918942 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.3
# Tue, 12 Jan 2021 00:30:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Tue, 12 Jan 2021 00:30:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:30:23 GMT
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
	-	`sha256:22d1daca1ee8464c5952c258eaf51c30dfbc6217b2da9085a584b192b6bfcf88`  
		Last Modified: Tue, 12 Jan 2021 00:31:27 GMT  
		Size: 255.1 MB (255071873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922309b38ee41ce43c9f5aae3cb1b310831aee721ef4cc0ca4e1342ddad3f726`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 1.6 MB (1567827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfe390c691e9f882c5177921d39981973b7fc9cd12f12b7f776cbfcff3765de`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d52fd762724ae28092402a64a63c91fe752881d9f24fb208bac99a66af28d5`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9748f4d2e954dba0ccf95c3ad9ddb70856640e5803386a289c5fed5f2e803f6`  
		Last Modified: Tue, 12 Jan 2021 00:31:01 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec8faa127363d72abbf4e78d9e4cd709eab5f7d6680f2e1c207ab78200238b`  
		Last Modified: Tue, 12 Jan 2021 00:31:02 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8223e2f6a253394aade82f137d4a4ee75850b3a10ac07f2f77d884818a6bc2aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.7 MB (361704668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f19b6ce48819d324fc8f34e1c3e5bf4ff0b859a9ca80fd7714b79072f469471`
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
# Mon, 11 Jan 2021 23:41:07 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.3.tar.gz.asc crate-4.3.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.3.tar.gz.asc     && tar -xf crate-4.3.3.tar.gz -C /crate --strip-components=1     && rm crate-4.3.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 11 Jan 2021 23:41:15 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 11 Jan 2021 23:41:16 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 11 Jan 2021 23:41:17 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 11 Jan 2021 23:41:18 GMT
RUN mkdir -p /data/data /data/log
# Mon, 11 Jan 2021 23:41:19 GMT
VOLUME [/data]
# Mon, 11 Jan 2021 23:41:20 GMT
WORKDIR /data
# Mon, 11 Jan 2021 23:41:20 GMT
EXPOSE 4200 4300 5432
# Mon, 11 Jan 2021 23:41:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 11 Jan 2021 23:41:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 11 Jan 2021 23:41:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-06T13:49:59.918942 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.3
# Mon, 11 Jan 2021 23:41:23 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Mon, 11 Jan 2021 23:41:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:41:24 GMT
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
	-	`sha256:6462066fbb7066c2d1d471f5f80480f5ab255c808156e607bba5ccdbb5645af9`  
		Last Modified: Mon, 11 Jan 2021 23:43:02 GMT  
		Size: 251.8 MB (251757765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b79aec7edb98837e07ce03e121c1e53fa2d7bd461ce193b97e53d9c9c25fef2`  
		Last Modified: Mon, 11 Jan 2021 23:42:22 GMT  
		Size: 1.6 MB (1567819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e6c15b4f707e090888017515775218b8607eb833fb5f8f69fd0aad6b85b1a1`  
		Last Modified: Mon, 11 Jan 2021 23:42:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0ec98997042e5a3a67e8be78395c2f4242a336757ec73072aee56374d9f30a`  
		Last Modified: Mon, 11 Jan 2021 23:42:23 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9060a930557208ce82b3093c151b1f99aac6babbb92ddc3a865600d7312173e0`  
		Last Modified: Mon, 11 Jan 2021 23:42:23 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf77334e8035e468e8ef580cb7d57f9c9839781b851bd24558c207a1b6c26b`  
		Last Modified: Mon, 11 Jan 2021 23:42:24 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
