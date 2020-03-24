<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:3.3`](#crate33)
-	[`crate:3.3.5`](#crate335)
-	[`crate:4.0`](#crate40)
-	[`crate:4.0.12`](#crate4012)
-	[`crate:4.1`](#crate41)
-	[`crate:4.1.4`](#crate414)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:1220d3a66ba7434b40edd63308e7ebb931f7d20dfc03a7f40f24846525d96261
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:3.3` - linux; amd64

```console
$ docker pull crate@sha256:28029e531f7aceb85666b0bd67a5d3c1fe45f4467e3ac14bf98e617018a23ce2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.4 MB (344428347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e96aeb3894ea7c822a0142a9fab1a1d0dffe6efa890ef860e56d50476f0adf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:25:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 12 Nov 2019 02:27:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 12 Nov 2019 02:27:49 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Tue, 12 Nov 2019 02:27:49 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Tue, 12 Nov 2019 02:28:47 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 12 Nov 2019 02:28:47 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Nov 2019 02:28:47 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Nov 2019 02:28:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 12 Nov 2019 02:28:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Nov 2019 02:28:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 12 Nov 2019 02:28:50 GMT
RUN mkdir -p /data/data /data/log
# Tue, 12 Nov 2019 02:28:50 GMT
VOLUME [/data]
# Tue, 12 Nov 2019 02:28:50 GMT
WORKDIR /data
# Tue, 12 Nov 2019 02:28:50 GMT
EXPOSE 4200 4300 5432
# Tue, 12 Nov 2019 02:28:51 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Nov 2019 02:28:51 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Nov 2019 02:28:51 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2019-07-08T14:08:18.187344 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Tue, 12 Nov 2019 02:28:51 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 12 Nov 2019 02:28:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:28:51 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82aa4130eb2a175e62f98b2ce60e9b2e0d68d8ae342810b26c821bedc428983`  
		Last Modified: Tue, 12 Nov 2019 02:30:36 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8f68504ec2c5765db548cc2ddcb32937b1072af2e37e1ba56c9e867adc9bb3`  
		Last Modified: Tue, 12 Nov 2019 02:31:20 GMT  
		Size: 188.1 MB (188101325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ad843ad2701b18cddae3f025111abfe91edc8b78735988cfdc7759a30edd9`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ffb4e6dc1ab19b4589ff57e77221320783bce3f50cf263975446e9b166a775`  
		Last Modified: Tue, 12 Nov 2019 02:31:12 GMT  
		Size: 79.2 MB (79246730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e48d3344e9f6d20d253cc9b8c0e62020a424d8d5c1405ea4066f688b01f110`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2105112ea016388d5b835aa32be8f5dfba2e84a40dff93803043b5fcff806`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df92165a3a99469b9cfa588d35c040aa8b7bc8e114422d38cd501397a93563f`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 1.3 MB (1294045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5bbfb4acf75aa2021bd49d72b641da8541333fdd2b67ec378cc391a7aee815`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c192e02a2b87f83721595e911d909829d9aaca448c37c17403a9b63b6a2abc8a`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe1f645884d2346dcef4fe9aaa190fc5ad5614bd3313a541039cd99aaf31b30`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded610082ee63d998ec7c77cb724405d7a42b6c42a5c42f8d824c1a23b279384`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:3.3.5`

```console
$ docker pull crate@sha256:1220d3a66ba7434b40edd63308e7ebb931f7d20dfc03a7f40f24846525d96261
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:3.3.5` - linux; amd64

```console
$ docker pull crate@sha256:28029e531f7aceb85666b0bd67a5d3c1fe45f4467e3ac14bf98e617018a23ce2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.4 MB (344428347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e96aeb3894ea7c822a0142a9fab1a1d0dffe6efa890ef860e56d50476f0adf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:25:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 12 Nov 2019 02:27:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 12 Nov 2019 02:27:49 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Tue, 12 Nov 2019 02:27:49 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Tue, 12 Nov 2019 02:28:47 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 12 Nov 2019 02:28:47 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Nov 2019 02:28:47 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Nov 2019 02:28:49 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 12 Nov 2019 02:28:49 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Nov 2019 02:28:49 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 12 Nov 2019 02:28:50 GMT
RUN mkdir -p /data/data /data/log
# Tue, 12 Nov 2019 02:28:50 GMT
VOLUME [/data]
# Tue, 12 Nov 2019 02:28:50 GMT
WORKDIR /data
# Tue, 12 Nov 2019 02:28:50 GMT
EXPOSE 4200 4300 5432
# Tue, 12 Nov 2019 02:28:51 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 12 Nov 2019 02:28:51 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 12 Nov 2019 02:28:51 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2019-07-08T14:08:18.187344 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Tue, 12 Nov 2019 02:28:51 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 12 Nov 2019 02:28:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:28:51 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82aa4130eb2a175e62f98b2ce60e9b2e0d68d8ae342810b26c821bedc428983`  
		Last Modified: Tue, 12 Nov 2019 02:30:36 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8f68504ec2c5765db548cc2ddcb32937b1072af2e37e1ba56c9e867adc9bb3`  
		Last Modified: Tue, 12 Nov 2019 02:31:20 GMT  
		Size: 188.1 MB (188101325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ad843ad2701b18cddae3f025111abfe91edc8b78735988cfdc7759a30edd9`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ffb4e6dc1ab19b4589ff57e77221320783bce3f50cf263975446e9b166a775`  
		Last Modified: Tue, 12 Nov 2019 02:31:12 GMT  
		Size: 79.2 MB (79246730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e48d3344e9f6d20d253cc9b8c0e62020a424d8d5c1405ea4066f688b01f110`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2105112ea016388d5b835aa32be8f5dfba2e84a40dff93803043b5fcff806`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df92165a3a99469b9cfa588d35c040aa8b7bc8e114422d38cd501397a93563f`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 1.3 MB (1294045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5bbfb4acf75aa2021bd49d72b641da8541333fdd2b67ec378cc391a7aee815`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c192e02a2b87f83721595e911d909829d9aaca448c37c17403a9b63b6a2abc8a`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe1f645884d2346dcef4fe9aaa190fc5ad5614bd3313a541039cd99aaf31b30`  
		Last Modified: Tue, 12 Nov 2019 02:31:02 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded610082ee63d998ec7c77cb724405d7a42b6c42a5c42f8d824c1a23b279384`  
		Last Modified: Tue, 12 Nov 2019 02:31:01 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0`

```console
$ docker pull crate@sha256:957f0c118cd4808e3d6aa97ca06b733f9f0c68901e4202476bd9b72074857f69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0` - linux; amd64

```console
$ docker pull crate@sha256:eba1122386179b7aa6d67b181a4a42ba26c6f05e8d732c1f5bae040672111cbd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.0 MB (352022399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc05a5dc108e7dd6a94118eae7f0489568d10642674a3622431fe6a1f3c78fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:25:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 12 Nov 2019 02:26:04 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 12 Nov 2019 02:26:05 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Tue, 12 Nov 2019 02:26:05 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Wed, 05 Feb 2020 23:28:21 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Wed, 05 Feb 2020 23:28:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 05 Feb 2020 23:28:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 05 Feb 2020 23:28:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 05 Feb 2020 23:28:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Feb 2020 23:28:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 05 Feb 2020 23:28:24 GMT
RUN mkdir -p /data/data /data/log
# Wed, 05 Feb 2020 23:28:24 GMT
VOLUME [/data]
# Wed, 05 Feb 2020 23:28:24 GMT
WORKDIR /data
# Wed, 05 Feb 2020 23:28:24 GMT
EXPOSE 4200 4300 5432
# Wed, 05 Feb 2020 23:28:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 05 Feb 2020 23:28:25 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 05 Feb 2020 23:28:25 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Wed, 05 Feb 2020 23:28:25 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 05 Feb 2020 23:28:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:28:25 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82aa4130eb2a175e62f98b2ce60e9b2e0d68d8ae342810b26c821bedc428983`  
		Last Modified: Tue, 12 Nov 2019 02:30:36 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794e274fac32ce9a1fa51077c71a5a03077860c10720987adf900dd957270484`  
		Last Modified: Tue, 12 Nov 2019 02:30:56 GMT  
		Size: 198.1 MB (198127895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a44dfe8d003796a7049dcb6923f2e20d1b4bb030cdf23106d22efff36b353a`  
		Last Modified: Tue, 12 Nov 2019 02:30:35 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5a199fb495c5b2f3ff0afafbee43b1f0ae2f12e0dca6e257e930900be86f8`  
		Last Modified: Wed, 05 Feb 2020 23:31:24 GMT  
		Size: 76.8 MB (76814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4f1596f6fa95f8c532861539b04d2cc80190200aaa01c0f0faedc1e2b27bc`  
		Last Modified: Wed, 05 Feb 2020 23:31:14 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9d8c7c981007c1414a9bfedbe41fbbedd94a5ac4609eccd3376bb66fa1f190`  
		Last Modified: Wed, 05 Feb 2020 23:31:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c91cb0e57f432b2f906e70c5dd04de3d0179b32016040daf79175bce70434`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 1.3 MB (1294049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b312f52e3c364501045394d02f09c97b7b4d05d79e54cdbc77407f06dba770ee`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b95ab09be9163d9f23fb6a13401fdc99f9daf00b8d60bcc2d2806feb8403ea`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2bb7e315daebf3d61f603c9fdeddb47170c8fe74af2a03421ec272c16da005`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36eeef08904fddf0f34061d92561752ec38c2ae4681d8334c323056e80e13cd`  
		Last Modified: Wed, 05 Feb 2020 23:31:14 GMT  
		Size: 527.0 B  
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
$ docker pull crate@sha256:957f0c118cd4808e3d6aa97ca06b733f9f0c68901e4202476bd9b72074857f69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0.12` - linux; amd64

```console
$ docker pull crate@sha256:eba1122386179b7aa6d67b181a4a42ba26c6f05e8d732c1f5bae040672111cbd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.0 MB (352022399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc05a5dc108e7dd6a94118eae7f0489568d10642674a3622431fe6a1f3c78fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:25:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Tue, 12 Nov 2019 02:26:04 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Tue, 12 Nov 2019 02:26:05 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Tue, 12 Nov 2019 02:26:05 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Wed, 05 Feb 2020 23:28:21 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Wed, 05 Feb 2020 23:28:21 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 05 Feb 2020 23:28:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 05 Feb 2020 23:28:23 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 05 Feb 2020 23:28:23 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Feb 2020 23:28:23 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 05 Feb 2020 23:28:24 GMT
RUN mkdir -p /data/data /data/log
# Wed, 05 Feb 2020 23:28:24 GMT
VOLUME [/data]
# Wed, 05 Feb 2020 23:28:24 GMT
WORKDIR /data
# Wed, 05 Feb 2020 23:28:24 GMT
EXPOSE 4200 4300 5432
# Wed, 05 Feb 2020 23:28:24 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 05 Feb 2020 23:28:25 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 05 Feb 2020 23:28:25 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Wed, 05 Feb 2020 23:28:25 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 05 Feb 2020 23:28:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 23:28:25 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82aa4130eb2a175e62f98b2ce60e9b2e0d68d8ae342810b26c821bedc428983`  
		Last Modified: Tue, 12 Nov 2019 02:30:36 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794e274fac32ce9a1fa51077c71a5a03077860c10720987adf900dd957270484`  
		Last Modified: Tue, 12 Nov 2019 02:30:56 GMT  
		Size: 198.1 MB (198127895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a44dfe8d003796a7049dcb6923f2e20d1b4bb030cdf23106d22efff36b353a`  
		Last Modified: Tue, 12 Nov 2019 02:30:35 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5a199fb495c5b2f3ff0afafbee43b1f0ae2f12e0dca6e257e930900be86f8`  
		Last Modified: Wed, 05 Feb 2020 23:31:24 GMT  
		Size: 76.8 MB (76814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4f1596f6fa95f8c532861539b04d2cc80190200aaa01c0f0faedc1e2b27bc`  
		Last Modified: Wed, 05 Feb 2020 23:31:14 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9d8c7c981007c1414a9bfedbe41fbbedd94a5ac4609eccd3376bb66fa1f190`  
		Last Modified: Wed, 05 Feb 2020 23:31:14 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c91cb0e57f432b2f906e70c5dd04de3d0179b32016040daf79175bce70434`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 1.3 MB (1294049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b312f52e3c364501045394d02f09c97b7b4d05d79e54cdbc77407f06dba770ee`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b95ab09be9163d9f23fb6a13401fdc99f9daf00b8d60bcc2d2806feb8403ea`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2bb7e315daebf3d61f603c9fdeddb47170c8fe74af2a03421ec272c16da005`  
		Last Modified: Wed, 05 Feb 2020 23:31:13 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36eeef08904fddf0f34061d92561752ec38c2ae4681d8334c323056e80e13cd`  
		Last Modified: Wed, 05 Feb 2020 23:31:14 GMT  
		Size: 527.0 B  
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
$ docker pull crate@sha256:844be694aa8e28f3b7d65c4fadfe126cb783ec4dce492bebade75030699ff4bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1` - linux; amd64

```console
$ docker pull crate@sha256:d784e271d0ea301617b8ed6ace22e6844db1768ff2faf097075580d3cc1e5c02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (350987275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9864b9a05d3699433e84bb07844d98df3a065435e2dcc1a0b531ef483ef1ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:25:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 05 Feb 2020 23:25:54 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 05 Feb 2020 23:25:54 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Wed, 05 Feb 2020 23:25:55 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 10 Mar 2020 23:20:07 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.3.tar.gz.asc crate-4.1.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.3.tar.gz.asc     && tar -xf crate-4.1.3.tar.gz -C /crate --strip-components=1     && rm crate-4.1.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 10 Mar 2020 23:20:07 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 23:20:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 23:20:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 10 Mar 2020 23:20:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Mar 2020 23:20:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 10 Mar 2020 23:20:11 GMT
RUN mkdir -p /data/data /data/log
# Tue, 10 Mar 2020 23:20:11 GMT
VOLUME [/data]
# Tue, 10 Mar 2020 23:20:11 GMT
WORKDIR /data
# Tue, 10 Mar 2020 23:20:12 GMT
EXPOSE 4200 4300 5432
# Tue, 10 Mar 2020 23:20:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 23:20:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 23:20:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-03-05T16:12:47.636379 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.3
# Tue, 10 Mar 2020 23:20:12 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 10 Mar 2020 23:20:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 10 Mar 2020 23:20:13 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82aa4130eb2a175e62f98b2ce60e9b2e0d68d8ae342810b26c821bedc428983`  
		Last Modified: Tue, 12 Nov 2019 02:30:36 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c132278b93b3443fafff8460382be10690caf0702bc22339ea0dd7b81d5cf8b`  
		Last Modified: Wed, 05 Feb 2020 23:31:07 GMT  
		Size: 196.4 MB (196423227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42807ee70d40e75fddd4f32ee923cedd85714cfe1339b0e13e317438a447e721`  
		Last Modified: Wed, 05 Feb 2020 23:28:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b71cea01ab267fb926b2d84eb5c2518cc594ecd2dac127122deaa3513d9ba0`  
		Last Modified: Tue, 10 Mar 2020 23:20:41 GMT  
		Size: 77.5 MB (77483750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db39538c033a122467b822270cdf73160fdeb03696fea64030b894cc1c3d54cb`  
		Last Modified: Tue, 10 Mar 2020 23:20:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f1feb5b39f7493ac238b311d4c808c91a91d813883772b37a98ebcc296a5e`  
		Last Modified: Tue, 10 Mar 2020 23:20:33 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddadaabd46bbafeb6d6bba5703faa44fb3f6a0e2d34939b94cc8795c58964dca`  
		Last Modified: Tue, 10 Mar 2020 23:20:33 GMT  
		Size: 1.3 MB (1294056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0e985529e9a537e9ad8a1d8e1c7cb9473cdda26694a0cdc12e910de2c6112f`  
		Last Modified: Tue, 10 Mar 2020 23:20:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e91d88011d6ad457db85dd5ce3968ff72d57f80860b440d5d2d47b080a6faf6`  
		Last Modified: Tue, 10 Mar 2020 23:20:32 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ce60a679cde4f12e16de558dc574bbaea2a5023ec1153cf56f78577d77d480`  
		Last Modified: Tue, 10 Mar 2020 23:20:33 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc2ed38c4f7d6778869d23f80ecf1d265169191c68e0ed151b5610fe0b934d`  
		Last Modified: Tue, 10 Mar 2020 23:20:32 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:4f685723060cfe366068b916eb03cf578c13b580f1d31ce8e081bbcd2212d16e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.5 MB (376519154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee220ddd7668e6b737f0151b642eabb7c53badd0b6c7f79e5ef07945c17b7886`
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
# Wed, 05 Feb 2020 23:46:15 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 05 Feb 2020 23:46:17 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Wed, 05 Feb 2020 23:46:18 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 10 Mar 2020 22:40:22 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.3.tar.gz.asc crate-4.1.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.3.tar.gz.asc     && tar -xf crate-4.1.3.tar.gz -C /crate --strip-components=1     && rm crate-4.1.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 10 Mar 2020 22:40:23 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 22:40:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 22:40:28 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 10 Mar 2020 22:40:29 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Mar 2020 22:40:30 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 10 Mar 2020 22:40:34 GMT
RUN mkdir -p /data/data /data/log
# Tue, 10 Mar 2020 22:40:34 GMT
VOLUME [/data]
# Tue, 10 Mar 2020 22:40:35 GMT
WORKDIR /data
# Tue, 10 Mar 2020 22:40:36 GMT
EXPOSE 4200 4300 5432
# Tue, 10 Mar 2020 22:40:36 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 22:40:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 22:40:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-03-05T16:12:47.636379 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.3
# Tue, 10 Mar 2020 22:40:38 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 10 Mar 2020 22:40:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 10 Mar 2020 22:40:39 GMT
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
	-	`sha256:60d6743359dfaf8645137afd31a4552eb3195971517a48fca57593b25250b015`  
		Last Modified: Tue, 18 Feb 2020 22:42:08 GMT  
		Size: 196.4 MB (196423249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf4a3a653abc3f2a5931326c03e9ef927aec2a7ab30aa4fcc311b69d41fa57c`  
		Last Modified: Tue, 18 Feb 2020 22:41:34 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c025dc6cae10e94b36345eae35e138b3d898339e1fafc5f1aaf04abf387029`  
		Last Modified: Tue, 10 Mar 2020 22:42:36 GMT  
		Size: 75.2 MB (75176628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fd59b598b1afc1dfc052ee06e3ed3a308f9b17f265f45d0ed5418317b45767`  
		Last Modified: Tue, 10 Mar 2020 22:42:22 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a29188fe4b021a4a54bfd4c4eccd656a33c8599c5d626b2a5d64ccb2f69c0ce`  
		Last Modified: Tue, 10 Mar 2020 22:42:23 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4843db5a229fae94ebe225592d1b3fb40d23a38234016a09d611b22f8b0d0e2a`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 1.3 MB (1294047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8640a32f3360eef8222cadc0ff902e6f3790ee8d0fdc5e844ab7ed0ea4dee152`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c1668cf596c3f71fced564351c6301af1ef0bc58ebb1edd70f4e29bd1f5279`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007438d52e9d66e1da7d2546f538ea4a0c333af127388d120d2b1f93384ede40`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f520775899774c3898bd17958f4d73322c8506f45e94be6955092c72eeccb`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1.4`

**does not exist** (yet?)

## `crate:latest`

```console
$ docker pull crate@sha256:844be694aa8e28f3b7d65c4fadfe126cb783ec4dce492bebade75030699ff4bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:d784e271d0ea301617b8ed6ace22e6844db1768ff2faf097075580d3cc1e5c02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (350987275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9864b9a05d3699433e84bb07844d98df3a065435e2dcc1a0b531ef483ef1ac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 12 Nov 2019 02:25:33 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 05 Feb 2020 23:25:54 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 05 Feb 2020 23:25:54 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Wed, 05 Feb 2020 23:25:55 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 10 Mar 2020 23:20:07 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.3.tar.gz.asc crate-4.1.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.3.tar.gz.asc     && tar -xf crate-4.1.3.tar.gz -C /crate --strip-components=1     && rm crate-4.1.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 10 Mar 2020 23:20:07 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 23:20:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 23:20:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 10 Mar 2020 23:20:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Mar 2020 23:20:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 10 Mar 2020 23:20:11 GMT
RUN mkdir -p /data/data /data/log
# Tue, 10 Mar 2020 23:20:11 GMT
VOLUME [/data]
# Tue, 10 Mar 2020 23:20:11 GMT
WORKDIR /data
# Tue, 10 Mar 2020 23:20:12 GMT
EXPOSE 4200 4300 5432
# Tue, 10 Mar 2020 23:20:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 23:20:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 23:20:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-03-05T16:12:47.636379 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.3
# Tue, 10 Mar 2020 23:20:12 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 10 Mar 2020 23:20:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 10 Mar 2020 23:20:13 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82aa4130eb2a175e62f98b2ce60e9b2e0d68d8ae342810b26c821bedc428983`  
		Last Modified: Tue, 12 Nov 2019 02:30:36 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c132278b93b3443fafff8460382be10690caf0702bc22339ea0dd7b81d5cf8b`  
		Last Modified: Wed, 05 Feb 2020 23:31:07 GMT  
		Size: 196.4 MB (196423227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42807ee70d40e75fddd4f32ee923cedd85714cfe1339b0e13e317438a447e721`  
		Last Modified: Wed, 05 Feb 2020 23:28:42 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b71cea01ab267fb926b2d84eb5c2518cc594ecd2dac127122deaa3513d9ba0`  
		Last Modified: Tue, 10 Mar 2020 23:20:41 GMT  
		Size: 77.5 MB (77483750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db39538c033a122467b822270cdf73160fdeb03696fea64030b894cc1c3d54cb`  
		Last Modified: Tue, 10 Mar 2020 23:20:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f1feb5b39f7493ac238b311d4c808c91a91d813883772b37a98ebcc296a5e`  
		Last Modified: Tue, 10 Mar 2020 23:20:33 GMT  
		Size: 954.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddadaabd46bbafeb6d6bba5703faa44fb3f6a0e2d34939b94cc8795c58964dca`  
		Last Modified: Tue, 10 Mar 2020 23:20:33 GMT  
		Size: 1.3 MB (1294056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0e985529e9a537e9ad8a1d8e1c7cb9473cdda26694a0cdc12e910de2c6112f`  
		Last Modified: Tue, 10 Mar 2020 23:20:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e91d88011d6ad457db85dd5ce3968ff72d57f80860b440d5d2d47b080a6faf6`  
		Last Modified: Tue, 10 Mar 2020 23:20:32 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ce60a679cde4f12e16de558dc574bbaea2a5023ec1153cf56f78577d77d480`  
		Last Modified: Tue, 10 Mar 2020 23:20:33 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc2ed38c4f7d6778869d23f80ecf1d265169191c68e0ed151b5610fe0b934d`  
		Last Modified: Tue, 10 Mar 2020 23:20:32 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:4f685723060cfe366068b916eb03cf578c13b580f1d31ce8e081bbcd2212d16e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.5 MB (376519154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee220ddd7668e6b737f0151b642eabb7c53badd0b6c7f79e5ef07945c17b7886`
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
# Wed, 05 Feb 2020 23:46:15 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Wed, 05 Feb 2020 23:46:17 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Wed, 05 Feb 2020 23:46:18 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Tue, 10 Mar 2020 22:40:22 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.3.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.3.tar.gz.asc crate-4.1.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.3.tar.gz.asc     && tar -xf crate-4.1.3.tar.gz -C /crate --strip-components=1     && rm crate-4.1.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Tue, 10 Mar 2020 22:40:23 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 22:40:24 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 22:40:28 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Tue, 10 Mar 2020 22:40:29 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Mar 2020 22:40:30 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 10 Mar 2020 22:40:34 GMT
RUN mkdir -p /data/data /data/log
# Tue, 10 Mar 2020 22:40:34 GMT
VOLUME [/data]
# Tue, 10 Mar 2020 22:40:35 GMT
WORKDIR /data
# Tue, 10 Mar 2020 22:40:36 GMT
EXPOSE 4200 4300 5432
# Tue, 10 Mar 2020 22:40:36 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Tue, 10 Mar 2020 22:40:37 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Tue, 10 Mar 2020 22:40:37 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-03-05T16:12:47.636379 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.3
# Tue, 10 Mar 2020 22:40:38 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Tue, 10 Mar 2020 22:40:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 10 Mar 2020 22:40:39 GMT
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
	-	`sha256:60d6743359dfaf8645137afd31a4552eb3195971517a48fca57593b25250b015`  
		Last Modified: Tue, 18 Feb 2020 22:42:08 GMT  
		Size: 196.4 MB (196423249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf4a3a653abc3f2a5931326c03e9ef927aec2a7ab30aa4fcc311b69d41fa57c`  
		Last Modified: Tue, 18 Feb 2020 22:41:34 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c025dc6cae10e94b36345eae35e138b3d898339e1fafc5f1aaf04abf387029`  
		Last Modified: Tue, 10 Mar 2020 22:42:36 GMT  
		Size: 75.2 MB (75176628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fd59b598b1afc1dfc052ee06e3ed3a308f9b17f265f45d0ed5418317b45767`  
		Last Modified: Tue, 10 Mar 2020 22:42:22 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a29188fe4b021a4a54bfd4c4eccd656a33c8599c5d626b2a5d64ccb2f69c0ce`  
		Last Modified: Tue, 10 Mar 2020 22:42:23 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4843db5a229fae94ebe225592d1b3fb40d23a38234016a09d611b22f8b0d0e2a`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 1.3 MB (1294047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8640a32f3360eef8222cadc0ff902e6f3790ee8d0fdc5e844ab7ed0ea4dee152`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c1668cf596c3f71fced564351c6301af1ef0bc58ebb1edd70f4e29bd1f5279`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007438d52e9d66e1da7d2546f538ea4a0c333af127388d120d2b1f93384ede40`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f520775899774c3898bd17958f4d73322c8506f45e94be6955092c72eeccb`  
		Last Modified: Tue, 10 Mar 2020 22:42:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
