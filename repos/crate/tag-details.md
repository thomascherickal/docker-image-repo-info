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
-	[`crate:4.5`](#crate45)
-	[`crate:4.5.3`](#crate453)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:27223a3c4cef609a0a3e586bf4677da7ca48c7472278006619b7603c24dad12a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:a5eb267f0447f7ea0ebd39873bb27372b903b0a9c1ed2199ffdd98d766e649e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.5 MB (377488923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d29d50d18a0db06963e53452e5ad3c9841ac7722f47e8c3fc2e603e0b818e86`
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
# Thu, 24 Jun 2021 18:49:06 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Thu, 24 Jun 2021 18:49:06 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Thu, 24 Jun 2021 18:49:07 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Thu, 24 Jun 2021 18:49:52 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 24 Jun 2021 18:49:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:49:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:49:55 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:49:55 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:49:55 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:49:56 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:49:56 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:49:56 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:49:56 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:49:57 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:49:57 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:49:57 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Thu, 24 Jun 2021 18:49:57 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 24 Jun 2021 18:49:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:49:58 GMT
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
	-	`sha256:d286972740923eb98d662ff5b239aec690af7c62958d29f4f1afda54fc5f3b5e`  
		Last Modified: Thu, 24 Jun 2021 18:55:08 GMT  
		Size: 188.1 MB (188101482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ff9e11f6f20bde914b321881338393a8597dd92b13cb46d076c13601fb5044`  
		Last Modified: Thu, 24 Jun 2021 18:54:50 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7538d17ccc998a284d6fb53a3f8b1cd006ebe124580360691c4f254a213282`  
		Last Modified: Thu, 24 Jun 2021 18:54:59 GMT  
		Size: 79.7 MB (79712750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0947683cedd1db520404f554003ace7a671f26e7905fef848d6a4decf39472`  
		Last Modified: Thu, 24 Jun 2021 18:54:50 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e4f1b61f970743d1e9d7104d6f626d83feb490e9a69634ccd21aa64ade4c43`  
		Last Modified: Thu, 24 Jun 2021 18:54:50 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaef173ff55df505ff87f9c18440da8f9d041581b66c3a88dffcbce6450401e`  
		Last Modified: Thu, 24 Jun 2021 18:54:48 GMT  
		Size: 1.3 MB (1294146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0411b3d027e90d9cbb73b4e3729738f9dea50010279d55bee1fe313e0b098613`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae01c989f2a3d375035c1e59906d4f162fc11c27724ccf4521a3a29f92fa01`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cb8863ead537170e498dfed4b4c29ebc6e362cdad73e03298bba48d39b5158`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2987b51c615a945f278cfdd6454f6539fade9efb842ec2d461137cf8eed59f4a`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:3.3.5`

```console
$ docker pull crate@sha256:27223a3c4cef609a0a3e586bf4677da7ca48c7472278006619b7603c24dad12a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:a5eb267f0447f7ea0ebd39873bb27372b903b0a9c1ed2199ffdd98d766e649e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.5 MB (377488923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d29d50d18a0db06963e53452e5ad3c9841ac7722f47e8c3fc2e603e0b818e86`
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
# Thu, 24 Jun 2021 18:49:06 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Thu, 24 Jun 2021 18:49:06 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Thu, 24 Jun 2021 18:49:07 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Thu, 24 Jun 2021 18:49:52 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 24 Jun 2021 18:49:52 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:49:53 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:49:55 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:49:55 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:49:55 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:49:56 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:49:56 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:49:56 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:49:56 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:49:57 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:49:57 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:49:57 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Thu, 24 Jun 2021 18:49:57 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 24 Jun 2021 18:49:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:49:58 GMT
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
	-	`sha256:d286972740923eb98d662ff5b239aec690af7c62958d29f4f1afda54fc5f3b5e`  
		Last Modified: Thu, 24 Jun 2021 18:55:08 GMT  
		Size: 188.1 MB (188101482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ff9e11f6f20bde914b321881338393a8597dd92b13cb46d076c13601fb5044`  
		Last Modified: Thu, 24 Jun 2021 18:54:50 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7538d17ccc998a284d6fb53a3f8b1cd006ebe124580360691c4f254a213282`  
		Last Modified: Thu, 24 Jun 2021 18:54:59 GMT  
		Size: 79.7 MB (79712750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0947683cedd1db520404f554003ace7a671f26e7905fef848d6a4decf39472`  
		Last Modified: Thu, 24 Jun 2021 18:54:50 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e4f1b61f970743d1e9d7104d6f626d83feb490e9a69634ccd21aa64ade4c43`  
		Last Modified: Thu, 24 Jun 2021 18:54:50 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaef173ff55df505ff87f9c18440da8f9d041581b66c3a88dffcbce6450401e`  
		Last Modified: Thu, 24 Jun 2021 18:54:48 GMT  
		Size: 1.3 MB (1294146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0411b3d027e90d9cbb73b4e3729738f9dea50010279d55bee1fe313e0b098613`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae01c989f2a3d375035c1e59906d4f162fc11c27724ccf4521a3a29f92fa01`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cb8863ead537170e498dfed4b4c29ebc6e362cdad73e03298bba48d39b5158`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2987b51c615a945f278cfdd6454f6539fade9efb842ec2d461137cf8eed59f4a`  
		Last Modified: Thu, 24 Jun 2021 18:54:47 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0`

```console
$ docker pull crate@sha256:e2ce6a5b3db47d7f49c11a35e27caa433c4208ce701a4b40b57c862becd5a6e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:f0cd1ce26b5656594b458d7d90b2fc89752c3511020022b423377c91ec1d5490
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.4 MB (371411806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b0a20a824a9ac56872a5b74efb001e8bddbe7915291ddc9423efe9d56bb9f5`
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
# Thu, 24 Jun 2021 18:48:14 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Thu, 24 Jun 2021 18:48:15 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Thu, 24 Jun 2021 18:48:16 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Thu, 24 Jun 2021 18:48:35 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 24 Jun 2021 18:48:36 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:48:36 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:48:43 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:48:43 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:48:44 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:48:44 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:48:45 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:48:45 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:48:45 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:48:45 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:48:45 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:48:46 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Thu, 24 Jun 2021 18:48:46 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 24 Jun 2021 18:48:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:48:46 GMT
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
	-	`sha256:3fa8e3404622e71fe9e571ad11f24eab7ffcf35e725587689ef93bf262958b74`  
		Last Modified: Thu, 24 Jun 2021 18:54:32 GMT  
		Size: 198.1 MB (198127615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576c11b313ed9d8155cf997250488681d8e306809b2bef37d9e62d3c169dd444`  
		Last Modified: Thu, 24 Jun 2021 18:54:12 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffebce686659fdf0b75133c4889a8b6554d73dfb6a34614993bd850ab79a58c`  
		Last Modified: Thu, 24 Jun 2021 18:54:18 GMT  
		Size: 63.6 MB (63609491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9037b8bd7bb073dd104f431fa7c26991963efa39fb225b4e779c76c7548d9456`  
		Last Modified: Thu, 24 Jun 2021 18:54:11 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47dcd9adeff934f26a6fbef373df88e5e37dda7e801eeddff9635e9c839e8033`  
		Last Modified: Thu, 24 Jun 2021 18:54:11 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a06c35e92dc867c00f8f7aac04000907957df6b32b29407a3c66213079f8984`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 1.3 MB (1294160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245c3d26493614706f58eed52f0dc53ac6dd7c202ce8454f1060aa42772fd0ae`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5e5e682cf3a371d6d0e18fa466b9a987dfb7dd7b46a5e82a94a9175202c0f`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e7546da3a2a17333516b3ece74c102e6444b5a04d36f405e4a21cdd1fb8df`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552360798affe780bc89db92fb9f673e8479761f7a5523355af406175ec5c437`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0.12`

```console
$ docker pull crate@sha256:e2ce6a5b3db47d7f49c11a35e27caa433c4208ce701a4b40b57c862becd5a6e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:f0cd1ce26b5656594b458d7d90b2fc89752c3511020022b423377c91ec1d5490
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.4 MB (371411806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b0a20a824a9ac56872a5b74efb001e8bddbe7915291ddc9423efe9d56bb9f5`
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
# Thu, 24 Jun 2021 18:48:14 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Thu, 24 Jun 2021 18:48:15 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Thu, 24 Jun 2021 18:48:16 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Thu, 24 Jun 2021 18:48:35 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 24 Jun 2021 18:48:36 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:48:36 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:48:43 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:48:43 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:48:44 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:48:44 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:48:45 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:48:45 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:48:45 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:48:45 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:48:45 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:48:46 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Thu, 24 Jun 2021 18:48:46 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 24 Jun 2021 18:48:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:48:46 GMT
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
	-	`sha256:3fa8e3404622e71fe9e571ad11f24eab7ffcf35e725587689ef93bf262958b74`  
		Last Modified: Thu, 24 Jun 2021 18:54:32 GMT  
		Size: 198.1 MB (198127615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576c11b313ed9d8155cf997250488681d8e306809b2bef37d9e62d3c169dd444`  
		Last Modified: Thu, 24 Jun 2021 18:54:12 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffebce686659fdf0b75133c4889a8b6554d73dfb6a34614993bd850ab79a58c`  
		Last Modified: Thu, 24 Jun 2021 18:54:18 GMT  
		Size: 63.6 MB (63609491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9037b8bd7bb073dd104f431fa7c26991963efa39fb225b4e779c76c7548d9456`  
		Last Modified: Thu, 24 Jun 2021 18:54:11 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47dcd9adeff934f26a6fbef373df88e5e37dda7e801eeddff9635e9c839e8033`  
		Last Modified: Thu, 24 Jun 2021 18:54:11 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a06c35e92dc867c00f8f7aac04000907957df6b32b29407a3c66213079f8984`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 1.3 MB (1294160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245c3d26493614706f58eed52f0dc53ac6dd7c202ce8454f1060aa42772fd0ae`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5e5e682cf3a371d6d0e18fa466b9a987dfb7dd7b46a5e82a94a9175202c0f`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e7546da3a2a17333516b3ece74c102e6444b5a04d36f405e4a21cdd1fb8df`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552360798affe780bc89db92fb9f673e8479761f7a5523355af406175ec5c437`  
		Last Modified: Thu, 24 Jun 2021 18:54:09 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1`

```console
$ docker pull crate@sha256:f1a0c699cdbc749ed2395a883f672ce043bcd6479e48b39a6f9085b5246e4658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:be0a77f6590687a0a94fd727b6651d7033e6fabedc8b70fc51e36b5bf3fee569
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.1 MB (384066787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960ed0a661edaad943e9d2cc8e0d25d690b68ceec332b4d1fc9a0f25edbe2e0e`
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
# Thu, 24 Jun 2021 18:46:53 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Thu, 24 Jun 2021 18:46:53 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Thu, 24 Jun 2021 18:46:54 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Thu, 24 Jun 2021 18:47:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:47:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:47:48 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:47:48 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:47:49 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:47:49 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:47:49 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:47:49 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:47:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:47:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:47:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Thu, 24 Jun 2021 18:47:50 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 24 Jun 2021 18:47:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:47:50 GMT
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
	-	`sha256:b6b762c37465425c09fb92e72e0c5754aea5495c5a20d05e3aedfc79c8e34ad1`  
		Last Modified: Thu, 24 Jun 2021 18:53:56 GMT  
		Size: 196.4 MB (196423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad7d7166eae6f671f5d28dc07dd295115dbe920befb942ce33cc23d1bd675e0`  
		Last Modified: Thu, 24 Jun 2021 18:53:37 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6670c10af4ab0f0fc25d276edf27eb8df4674c4b52e21ecef4b9288e2784db8`  
		Last Modified: Thu, 24 Jun 2021 18:53:46 GMT  
		Size: 78.0 MB (77970028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed36cb93d0882bc613177ca20fa0a757a1d68e47d7e1f0632cdf6e91e63e74fa`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 1.3 MB (1294153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a5d188dae354761c1858d5c630da7ef4b35f8583d381a8e8a2d2f2e229d628`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9635dd031449214b23a954532e8d90d9faf68f2759a06cf01913b4ba61de2bfd`  
		Last Modified: Thu, 24 Jun 2021 18:53:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea4e6abb6b965d5ef13f33801012c232fd2c508bb596d2105b290a2f78aeba4`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45663360a08e3c983a1621d3046abff2d01f1375b0389ab05a029f472ee20`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1.8`

```console
$ docker pull crate@sha256:f1a0c699cdbc749ed2395a883f672ce043bcd6479e48b39a6f9085b5246e4658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:be0a77f6590687a0a94fd727b6651d7033e6fabedc8b70fc51e36b5bf3fee569
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.1 MB (384066787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960ed0a661edaad943e9d2cc8e0d25d690b68ceec332b4d1fc9a0f25edbe2e0e`
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
# Thu, 24 Jun 2021 18:46:53 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Thu, 24 Jun 2021 18:46:53 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Thu, 24 Jun 2021 18:46:54 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Thu, 24 Jun 2021 18:47:38 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:47:47 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:47:48 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:47:48 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:47:49 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:47:49 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:47:49 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:47:49 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:47:49 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:47:50 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:47:50 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Thu, 24 Jun 2021 18:47:50 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 24 Jun 2021 18:47:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:47:50 GMT
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
	-	`sha256:b6b762c37465425c09fb92e72e0c5754aea5495c5a20d05e3aedfc79c8e34ad1`  
		Last Modified: Thu, 24 Jun 2021 18:53:56 GMT  
		Size: 196.4 MB (196423284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad7d7166eae6f671f5d28dc07dd295115dbe920befb942ce33cc23d1bd675e0`  
		Last Modified: Thu, 24 Jun 2021 18:53:37 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6670c10af4ab0f0fc25d276edf27eb8df4674c4b52e21ecef4b9288e2784db8`  
		Last Modified: Thu, 24 Jun 2021 18:53:46 GMT  
		Size: 78.0 MB (77970028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed36cb93d0882bc613177ca20fa0a757a1d68e47d7e1f0632cdf6e91e63e74fa`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 1.3 MB (1294153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a5d188dae354761c1858d5c630da7ef4b35f8583d381a8e8a2d2f2e229d628`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9635dd031449214b23a954532e8d90d9faf68f2759a06cf01913b4ba61de2bfd`  
		Last Modified: Thu, 24 Jun 2021 18:53:34 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea4e6abb6b965d5ef13f33801012c232fd2c508bb596d2105b290a2f78aeba4`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c45663360a08e3c983a1621d3046abff2d01f1375b0389ab05a029f472ee20`  
		Last Modified: Thu, 24 Jun 2021 18:53:35 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2`

```console
$ docker pull crate@sha256:0e3642394810edbde03b649eb1a69f4332c41a4839904ede90d61a6e1e6b1d4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:efa03f23d006f7580870edf04620de7568f8761ee0619a6a102aaef04d2b7832
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.2 MB (363219130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57f619298e34ef63e030cad262c5d3d62139165b38c7c6e4079912442e3bacb`
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
# Thu, 24 Jun 2021 18:46:15 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:46:18 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:46:19 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:46:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:46:20 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:46:20 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:46:20 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:46:20 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:46:20 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:46:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:46:21 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Thu, 24 Jun 2021 18:46:21 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:46:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:46:21 GMT
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
	-	`sha256:cd0fa4230db9e1e7af42282b334d2611c9a5e5a19c61e0fb808c1360d7af568e`  
		Last Modified: Thu, 24 Jun 2021 18:53:21 GMT  
		Size: 253.3 MB (253272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354ee58ee6f914b72387957a2d3e731ca3921e2bc3ae19fe7a4810e87321eeb`  
		Last Modified: Thu, 24 Jun 2021 18:52:52 GMT  
		Size: 1.6 MB (1567819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88966585801da9c869603e4e4ebd938f426c8757459286b3e706af3b96a78a29`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f9695139f3e37f6e1d5af2e25457ec9ce9aea38ed832bac9d067986b2eb9d2`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b35d0a8f5daee97b064e6398944cf3f8aa74b501ab257b932d48677450d278`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d2eeca9b75be30383763c131991d7f2d1739953eb02f7a03711458bc352cbf`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2.7`

```console
$ docker pull crate@sha256:0e3642394810edbde03b649eb1a69f4332c41a4839904ede90d61a6e1e6b1d4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:efa03f23d006f7580870edf04620de7568f8761ee0619a6a102aaef04d2b7832
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.2 MB (363219130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57f619298e34ef63e030cad262c5d3d62139165b38c7c6e4079912442e3bacb`
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
# Thu, 24 Jun 2021 18:46:15 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.7.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.7.tar.gz.asc crate-4.2.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.7.tar.gz.asc     && tar -xf crate-4.2.7.tar.gz -C /crate --strip-components=1     && rm crate-4.2.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:46:18 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:46:19 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:46:19 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:46:20 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:46:20 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:46:20 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:46:20 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:46:20 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:46:21 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:46:21 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-15T20:03:26.122288 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.7
# Thu, 24 Jun 2021 18:46:21 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:46:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:46:21 GMT
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
	-	`sha256:cd0fa4230db9e1e7af42282b334d2611c9a5e5a19c61e0fb808c1360d7af568e`  
		Last Modified: Thu, 24 Jun 2021 18:53:21 GMT  
		Size: 253.3 MB (253272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354ee58ee6f914b72387957a2d3e731ca3921e2bc3ae19fe7a4810e87321eeb`  
		Last Modified: Thu, 24 Jun 2021 18:52:52 GMT  
		Size: 1.6 MB (1567819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88966585801da9c869603e4e4ebd938f426c8757459286b3e706af3b96a78a29`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f9695139f3e37f6e1d5af2e25457ec9ce9aea38ed832bac9d067986b2eb9d2`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b35d0a8f5daee97b064e6398944cf3f8aa74b501ab257b932d48677450d278`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d2eeca9b75be30383763c131991d7f2d1739953eb02f7a03711458bc352cbf`  
		Last Modified: Thu, 24 Jun 2021 18:52:51 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.3`

```console
$ docker pull crate@sha256:1f12392be7546eab6e710fbf1652c0d271cdc2a4c6c9d13eeff590a983a9d914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:1be76b931c3562e742fdd3b68a1df3c60325b8245ef1d1ddfc99da7adc0604e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362066449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f44ba265d5a71ff994e0f3804173b9aa5189add60241303614b23848e69d79`
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
# Thu, 24 Jun 2021 18:44:54 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.4.tar.gz.asc crate-4.3.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.4.tar.gz.asc     && tar -xf crate-4.3.4.tar.gz -C /crate --strip-components=1     && rm crate-4.3.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:45:04 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:45:05 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:45:05 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:45:06 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:45:06 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:45:06 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:45:06 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:45:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:45:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:45:07 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-19T14:19:50.388804 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.4
# Thu, 24 Jun 2021 18:45:07 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:45:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:45:07 GMT
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
	-	`sha256:e1eb9c1bc41f92bc37fe32d590a0375f199e6a7c486b51565d18cb48d659313d`  
		Last Modified: Thu, 24 Jun 2021 18:52:39 GMT  
		Size: 252.1 MB (252119546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c97a0eee1f23abe4446df337f32403dfd0dc08d588ba5f23ac50fd30adca8c`  
		Last Modified: Thu, 24 Jun 2021 18:52:11 GMT  
		Size: 1.6 MB (1567817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0699164f09ed38e293d37551d6202888528b26ec9aa2ef1794711501443c35ba`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148aa1c86f2c2ff96fe8eca94f65506efa597e8447d8d80b6e476fd5b6beb67f`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dd5e6298955be2d7fabce39258a0d42e30abda3f7588cbadda09a4ad1a20c7`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8760391ad5478675dc1c9bec8e94c9a06ddabba6013e13ccfbaf2dab5052b75`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.3.4`

```console
$ docker pull crate@sha256:1f12392be7546eab6e710fbf1652c0d271cdc2a4c6c9d13eeff590a983a9d914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
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
$ docker pull crate@sha256:1be76b931c3562e742fdd3b68a1df3c60325b8245ef1d1ddfc99da7adc0604e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362066449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f44ba265d5a71ff994e0f3804173b9aa5189add60241303614b23848e69d79`
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
# Thu, 24 Jun 2021 18:44:54 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.3.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.3.4.tar.gz.asc crate-4.3.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.3.4.tar.gz.asc     && tar -xf crate-4.3.4.tar.gz -C /crate --strip-components=1     && rm crate-4.3.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:45:04 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:45:05 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:45:05 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:45:06 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:45:06 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:45:06 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:45:06 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:45:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:45:07 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:45:07 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-01-19T14:19:50.388804 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.3.4
# Thu, 24 Jun 2021 18:45:07 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:45:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:45:07 GMT
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
	-	`sha256:e1eb9c1bc41f92bc37fe32d590a0375f199e6a7c486b51565d18cb48d659313d`  
		Last Modified: Thu, 24 Jun 2021 18:52:39 GMT  
		Size: 252.1 MB (252119546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c97a0eee1f23abe4446df337f32403dfd0dc08d588ba5f23ac50fd30adca8c`  
		Last Modified: Thu, 24 Jun 2021 18:52:11 GMT  
		Size: 1.6 MB (1567817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0699164f09ed38e293d37551d6202888528b26ec9aa2ef1794711501443c35ba`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148aa1c86f2c2ff96fe8eca94f65506efa597e8447d8d80b6e476fd5b6beb67f`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dd5e6298955be2d7fabce39258a0d42e30abda3f7588cbadda09a4ad1a20c7`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8760391ad5478675dc1c9bec8e94c9a06ddabba6013e13ccfbaf2dab5052b75`  
		Last Modified: Thu, 24 Jun 2021 18:52:10 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.4`

```console
$ docker pull crate@sha256:3687eaec8c56cfbcb17683db572aeb661272292c933ff25c177dfc133eb5a595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.4` - linux; amd64

```console
$ docker pull crate@sha256:e5c7c66846879db517445b5ae91163cc8ccf984844ef99e4d46387f464abe1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.4 MB (333363940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c0490cd3fc0aa657a091e571fbdcefd68b1d3937ba33489ba13a0e9a6bbfae`
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
# Fri, 26 Mar 2021 16:42:22 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Fri, 26 Mar 2021 16:42:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 26 Mar 2021 16:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 16:42:27 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 26 Mar 2021 16:42:28 GMT
RUN mkdir -p /data/data /data/log
# Fri, 26 Mar 2021 16:42:28 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 16:42:28 GMT
WORKDIR /data
# Fri, 26 Mar 2021 16:42:28 GMT
EXPOSE 4200 4300 5432
# Fri, 26 Mar 2021 16:42:28 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 26 Mar 2021 16:42:29 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 26 Mar 2021 16:42:29 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Fri, 26 Mar 2021 16:42:29 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 26 Mar 2021 16:42:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:42:29 GMT
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
	-	`sha256:192fde085303967f8184ff694a42aee9d771de382d71fa0ae7b7b215324e778a`  
		Last Modified: Fri, 26 Mar 2021 16:43:33 GMT  
		Size: 255.7 MB (255680460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c4cb2212ef8f76beee1e8cc14d9c71cff195d97585103fc81d320b1095a7ad`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 1.6 MB (1582186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8922bb6026f33be643febc56ab217d22420ee0832a2270edf0d8e725403240d`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c86996fd9159b78653d683069deacf3c842227768516febc1c0f0e569cc83f4`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4892b14b9585bb6574e4117cf9a1fbca12730008798e0800cd5cd8efb33f6`  
		Last Modified: Fri, 26 Mar 2021 16:43:06 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1020439fee87fa9d119cbd3d0f58a2d5133e43b095ef7c153b841c8af3074a`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.4` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:707b4b361b8898224bd129d7e8673d8effb54c884bad249ae4c722d4174762ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362399476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf88615c6eda6d65af59ec6e42b353ab521b430e19a76e3c5ecf4e8719774c6`
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
# Thu, 24 Jun 2021 18:43:31 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:43:39 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:43:40 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:43:40 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:43:41 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:43:41 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:43:41 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:43:41 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:43:41 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:43:42 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:43:42 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Thu, 24 Jun 2021 18:43:42 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:43:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:43:42 GMT
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
	-	`sha256:87d29c316bc60246513cd3ba5553ff7bac0d81cfcf9c584f04a13f93e5edb7ed`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 252.4 MB (252438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6e969da30e8fe21b1559f21d1d343df84b1aaff2f044d2ff0233d8e08a2ea2`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 1.6 MB (1582200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e4c2fd918ebb2ca2332fa693a3f8fa479039e7ee0314b1faf24088e101fb7`  
		Last Modified: Thu, 24 Jun 2021 18:51:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844a93af20ccf899cd4cc1233cbedbf762447306fac4a9422d9de02e55398f3b`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bde49b8e8d9acdfead359fd497f5e1f21b84b81a507d9ad45acbc3dd5543f9`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ec6ec26ad250b6d7807b18863526642cbc7520007f5f98f7f88112f295b5`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.4.3`

```console
$ docker pull crate@sha256:3687eaec8c56cfbcb17683db572aeb661272292c933ff25c177dfc133eb5a595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.4.3` - linux; amd64

```console
$ docker pull crate@sha256:e5c7c66846879db517445b5ae91163cc8ccf984844ef99e4d46387f464abe1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.4 MB (333363940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c0490cd3fc0aa657a091e571fbdcefd68b1d3937ba33489ba13a0e9a6bbfae`
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
# Fri, 26 Mar 2021 16:42:22 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Fri, 26 Mar 2021 16:42:26 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Fri, 26 Mar 2021 16:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 16:42:27 GMT
ENV CRATE_HEAP_SIZE=512M
# Fri, 26 Mar 2021 16:42:28 GMT
RUN mkdir -p /data/data /data/log
# Fri, 26 Mar 2021 16:42:28 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 16:42:28 GMT
WORKDIR /data
# Fri, 26 Mar 2021 16:42:28 GMT
EXPOSE 4200 4300 5432
# Fri, 26 Mar 2021 16:42:28 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Fri, 26 Mar 2021 16:42:29 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Fri, 26 Mar 2021 16:42:29 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Fri, 26 Mar 2021 16:42:29 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Fri, 26 Mar 2021 16:42:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:42:29 GMT
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
	-	`sha256:192fde085303967f8184ff694a42aee9d771de382d71fa0ae7b7b215324e778a`  
		Last Modified: Fri, 26 Mar 2021 16:43:33 GMT  
		Size: 255.7 MB (255680460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c4cb2212ef8f76beee1e8cc14d9c71cff195d97585103fc81d320b1095a7ad`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 1.6 MB (1582186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8922bb6026f33be643febc56ab217d22420ee0832a2270edf0d8e725403240d`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c86996fd9159b78653d683069deacf3c842227768516febc1c0f0e569cc83f4`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4892b14b9585bb6574e4117cf9a1fbca12730008798e0800cd5cd8efb33f6`  
		Last Modified: Fri, 26 Mar 2021 16:43:06 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1020439fee87fa9d119cbd3d0f58a2d5133e43b095ef7c153b841c8af3074a`  
		Last Modified: Fri, 26 Mar 2021 16:43:07 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.4.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:707b4b361b8898224bd129d7e8673d8effb54c884bad249ae4c722d4174762ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362399476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf88615c6eda6d65af59ec6e42b353ab521b430e19a76e3c5ecf4e8719774c6`
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
# Thu, 24 Jun 2021 18:43:31 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.4.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.4.3.tar.gz.asc crate-4.4.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.4.3.tar.gz.asc     && tar -xf crate-4.4.3.tar.gz -C /crate --strip-components=1     && rm crate-4.4.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:43:39 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:43:40 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:43:40 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:43:41 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:43:41 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:43:41 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:43:41 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:43:41 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:43:42 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:43:42 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-03-23T11:20:23.363006 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.4.3
# Thu, 24 Jun 2021 18:43:42 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:43:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:43:42 GMT
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
	-	`sha256:87d29c316bc60246513cd3ba5553ff7bac0d81cfcf9c584f04a13f93e5edb7ed`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 252.4 MB (252438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6e969da30e8fe21b1559f21d1d343df84b1aaff2f044d2ff0233d8e08a2ea2`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 1.6 MB (1582200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e4c2fd918ebb2ca2332fa693a3f8fa479039e7ee0314b1faf24088e101fb7`  
		Last Modified: Thu, 24 Jun 2021 18:51:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844a93af20ccf899cd4cc1233cbedbf762447306fac4a9422d9de02e55398f3b`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bde49b8e8d9acdfead359fd497f5e1f21b84b81a507d9ad45acbc3dd5543f9`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a55ec6ec26ad250b6d7807b18863526642cbc7520007f5f98f7f88112f295b5`  
		Last Modified: Thu, 24 Jun 2021 18:51:28 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.5`

```console
$ docker pull crate@sha256:53d50bdcf4f55759a128627c7074e73138e14cc80d2d5d6267d627de7b829129
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.5` - linux; amd64

```console
$ docker pull crate@sha256:2cb4def2c40399572ce2751b362e7ac3d66fd5339f988c0a65e594e424291ed1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331650641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972fb234916d4466032fcd1b10fde8f4e7f4a8715bfcdf1997064e474b505038`
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
# Thu, 24 Jun 2021 19:21:19 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 19:21:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 19:21:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 19:21:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 19:21:33 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 19:21:33 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:21:33 GMT
WORKDIR /data
# Thu, 24 Jun 2021 19:21:34 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 19:21:34 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 19:21:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 19:21:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 19:21:35 GMT
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
	-	`sha256:ecc329942bda5a423587272a404accf60dbcb9ebcf0a7897cec067c73ed731d8`  
		Last Modified: Thu, 24 Jun 2021 19:22:36 GMT  
		Size: 254.0 MB (253967169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61053c3bf2c4ead0f73027e3524c34c9ae49f6861535c40bd8ad0a9e1c485730`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 1.6 MB (1582181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bab11a61bd1c7c2af14234136b0e58ff3641267df0b1461cd6e50d46ebc29a4`  
		Last Modified: Thu, 24 Jun 2021 19:22:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a238762f62ecad53037cc6ee1a8502d76e147222c5ef3c8294e9bf026a17a`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d6ff6f0a4903bd888409121f33fee3fc04a8bc25898ad1d7f99f457edece8`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c3c7b0444faf6034ad134fca95717b32fe02c9a275e42cf4b048b6455ed03`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:d177532e186aba61de4d54b1f437fa5d8e0f8dd33e1a499be039ba8a157800a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360685324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ed7d10f8d644721cbb42a72bd1765a6c66201b64a5131eb936272e45cc9d00`
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
# Thu, 24 Jun 2021 18:42:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:42:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:42:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:42:26 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:42:27 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:42:27 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:42:27 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:42:28 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 18:42:28 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:42:28 GMT
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
	-	`sha256:2913fc3db3db14b5c5965fa8bf1a4238cec1ad88a51953cee6879c9640e68600`  
		Last Modified: Thu, 24 Jun 2021 18:51:10 GMT  
		Size: 250.7 MB (250724036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd85191a67d5c23f76cf0af887841989f7824958426183ccb44826242a3c2d8a`  
		Last Modified: Thu, 24 Jun 2021 18:50:42 GMT  
		Size: 1.6 MB (1582201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f3c3711dd535b2a2b89ad7447fd1b7e48cb7bbc64b294e2b34b8f93318915`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ccf937bdf10288d078d2e76a470533844833d3e1be62283d14a7f0ac84fbdf`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1fbc52778409789c05f322f4fc484613b2b36aee708b48f6c27452a28cde9e`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b48081fa4b69263a82d3f6c260050f4596c08cfa730d2fae5eca13105459dd`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.5.3`

```console
$ docker pull crate@sha256:53d50bdcf4f55759a128627c7074e73138e14cc80d2d5d6267d627de7b829129
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.5.3` - linux; amd64

```console
$ docker pull crate@sha256:2cb4def2c40399572ce2751b362e7ac3d66fd5339f988c0a65e594e424291ed1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331650641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972fb234916d4466032fcd1b10fde8f4e7f4a8715bfcdf1997064e474b505038`
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
# Thu, 24 Jun 2021 19:21:19 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 19:21:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 19:21:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 19:21:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 19:21:33 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 19:21:33 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:21:33 GMT
WORKDIR /data
# Thu, 24 Jun 2021 19:21:34 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 19:21:34 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 19:21:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 19:21:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 19:21:35 GMT
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
	-	`sha256:ecc329942bda5a423587272a404accf60dbcb9ebcf0a7897cec067c73ed731d8`  
		Last Modified: Thu, 24 Jun 2021 19:22:36 GMT  
		Size: 254.0 MB (253967169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61053c3bf2c4ead0f73027e3524c34c9ae49f6861535c40bd8ad0a9e1c485730`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 1.6 MB (1582181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bab11a61bd1c7c2af14234136b0e58ff3641267df0b1461cd6e50d46ebc29a4`  
		Last Modified: Thu, 24 Jun 2021 19:22:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a238762f62ecad53037cc6ee1a8502d76e147222c5ef3c8294e9bf026a17a`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d6ff6f0a4903bd888409121f33fee3fc04a8bc25898ad1d7f99f457edece8`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c3c7b0444faf6034ad134fca95717b32fe02c9a275e42cf4b048b6455ed03`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.5.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:d177532e186aba61de4d54b1f437fa5d8e0f8dd33e1a499be039ba8a157800a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360685324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ed7d10f8d644721cbb42a72bd1765a6c66201b64a5131eb936272e45cc9d00`
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
# Thu, 24 Jun 2021 18:42:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:42:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:42:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:42:26 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:42:27 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:42:27 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:42:27 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:42:28 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 18:42:28 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:42:28 GMT
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
	-	`sha256:2913fc3db3db14b5c5965fa8bf1a4238cec1ad88a51953cee6879c9640e68600`  
		Last Modified: Thu, 24 Jun 2021 18:51:10 GMT  
		Size: 250.7 MB (250724036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd85191a67d5c23f76cf0af887841989f7824958426183ccb44826242a3c2d8a`  
		Last Modified: Thu, 24 Jun 2021 18:50:42 GMT  
		Size: 1.6 MB (1582201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f3c3711dd535b2a2b89ad7447fd1b7e48cb7bbc64b294e2b34b8f93318915`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ccf937bdf10288d078d2e76a470533844833d3e1be62283d14a7f0ac84fbdf`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1fbc52778409789c05f322f4fc484613b2b36aee708b48f6c27452a28cde9e`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b48081fa4b69263a82d3f6c260050f4596c08cfa730d2fae5eca13105459dd`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:53d50bdcf4f55759a128627c7074e73138e14cc80d2d5d6267d627de7b829129
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:2cb4def2c40399572ce2751b362e7ac3d66fd5339f988c0a65e594e424291ed1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331650641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972fb234916d4466032fcd1b10fde8f4e7f4a8715bfcdf1997064e474b505038`
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
# Thu, 24 Jun 2021 19:21:19 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 19:21:32 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 19:21:32 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 19:21:32 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 19:21:33 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 19:21:33 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:21:33 GMT
WORKDIR /data
# Thu, 24 Jun 2021 19:21:34 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 19:21:34 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 19:21:34 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 19:21:35 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 19:21:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 19:21:35 GMT
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
	-	`sha256:ecc329942bda5a423587272a404accf60dbcb9ebcf0a7897cec067c73ed731d8`  
		Last Modified: Thu, 24 Jun 2021 19:22:36 GMT  
		Size: 254.0 MB (253967169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61053c3bf2c4ead0f73027e3524c34c9ae49f6861535c40bd8ad0a9e1c485730`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 1.6 MB (1582181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bab11a61bd1c7c2af14234136b0e58ff3641267df0b1461cd6e50d46ebc29a4`  
		Last Modified: Thu, 24 Jun 2021 19:22:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a238762f62ecad53037cc6ee1a8502d76e147222c5ef3c8294e9bf026a17a`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d6ff6f0a4903bd888409121f33fee3fc04a8bc25898ad1d7f99f457edece8`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c3c7b0444faf6034ad134fca95717b32fe02c9a275e42cf4b048b6455ed03`  
		Last Modified: Thu, 24 Jun 2021 19:22:12 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:d177532e186aba61de4d54b1f437fa5d8e0f8dd33e1a499be039ba8a157800a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360685324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ed7d10f8d644721cbb42a72bd1765a6c66201b64a5131eb936272e45cc9d00`
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
# Thu, 24 Jun 2021 18:42:17 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.5.3.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.5.3.tar.gz.asc crate-4.5.3.tar.gz     && rm -rf "$GNUPGHOME" crate-4.5.3.tar.gz.asc     && tar -xf crate-4.5.3.tar.gz -C /crate --strip-components=1     && rm crate-4.5.3.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Thu, 24 Jun 2021 18:42:25 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.27.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.27.0.asc crash_standalone_0.27.0     && rm -rf "$GNUPGHOME" crash_standalone_0.27.0.asc     && mv crash_standalone_0.27.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 24 Jun 2021 18:42:26 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 18:42:26 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 24 Jun 2021 18:42:26 GMT
RUN mkdir -p /data/data /data/log
# Thu, 24 Jun 2021 18:42:27 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:42:27 GMT
WORKDIR /data
# Thu, 24 Jun 2021 18:42:27 GMT
EXPOSE 4200 4300 5432
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 24 Jun 2021 18:42:27 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 24 Jun 2021 18:42:28 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2021-06-22T09:46:38.924581 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.5.3
# Thu, 24 Jun 2021 18:42:28 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Thu, 24 Jun 2021 18:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Jun 2021 18:42:28 GMT
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
	-	`sha256:2913fc3db3db14b5c5965fa8bf1a4238cec1ad88a51953cee6879c9640e68600`  
		Last Modified: Thu, 24 Jun 2021 18:51:10 GMT  
		Size: 250.7 MB (250724036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd85191a67d5c23f76cf0af887841989f7824958426183ccb44826242a3c2d8a`  
		Last Modified: Thu, 24 Jun 2021 18:50:42 GMT  
		Size: 1.6 MB (1582201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817f3c3711dd535b2a2b89ad7447fd1b7e48cb7bbc64b294e2b34b8f93318915`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ccf937bdf10288d078d2e76a470533844833d3e1be62283d14a7f0ac84fbdf`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1fbc52778409789c05f322f4fc484613b2b36aee708b48f6c27452a28cde9e`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b48081fa4b69263a82d3f6c260050f4596c08cfa730d2fae5eca13105459dd`  
		Last Modified: Thu, 24 Jun 2021 18:50:41 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
