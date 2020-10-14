<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:3.3`](#crate33)
-	[`crate:3.3.5`](#crate335)
-	[`crate:4.0`](#crate40)
-	[`crate:4.0.12`](#crate4012)
-	[`crate:4.1`](#crate41)
-	[`crate:4.1.8`](#crate418)
-	[`crate:4.2`](#crate42)
-	[`crate:4.2.6`](#crate426)
-	[`crate:latest`](#cratelatest)

## `crate:3.3`

```console
$ docker pull crate@sha256:79610eb88276d8434e58e7b456204fc796384cd4ecbc8efbd9d3c9fa2044faae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:3.3` - linux; amd64

```console
$ docker pull crate@sha256:287172d41a24589341527ae0de0698a8f93440a1ff19ccec021707afa150ec21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.5 MB (344547171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1959b9eb72576ad284b23e2a260f58278f2d5eb9229ed08335afe80f6cde9b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 18:51:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 18:51:48 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Mon, 10 Aug 2020 18:51:49 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Thu, 20 Aug 2020 19:22:17 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 20 Aug 2020 19:22:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:22:18 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:22:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 20 Aug 2020 19:22:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 19:22:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 20 Aug 2020 19:22:21 GMT
RUN mkdir -p /data/data /data/log
# Thu, 20 Aug 2020 19:22:21 GMT
VOLUME [/data]
# Thu, 20 Aug 2020 19:22:22 GMT
WORKDIR /data
# Thu, 20 Aug 2020 19:22:22 GMT
EXPOSE 4200 4300 5432
# Thu, 20 Aug 2020 19:22:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:22:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:22:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Thu, 20 Aug 2020 19:22:23 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 20 Aug 2020 19:22:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 19:22:23 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832e32314d6a05afed643636a2c1baad10515efbb71b1f01cfec46b085fbea14`  
		Last Modified: Mon, 10 Aug 2020 18:54:02 GMT  
		Size: 188.1 MB (188101329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fb76bc1732c60a3d3ddb00ea6d42ba52972c957dfa485b6d73bad734666b52`  
		Last Modified: Mon, 10 Aug 2020 18:53:45 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5b74ef97223994935b2e50f1e1a4536d1a29f2b164022cfc6a6236f96947dc`  
		Last Modified: Thu, 20 Aug 2020 19:22:50 GMT  
		Size: 79.3 MB (79283067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35c54368add1bc9b334fedadcff0bb8cd3eb1a33e8a8005cbde959534890f2`  
		Last Modified: Thu, 20 Aug 2020 19:22:42 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93357dd2cc916bd9e0e0865d8a9a0372e368e1367eeeb22e9d15de21c90596`  
		Last Modified: Thu, 20 Aug 2020 19:22:42 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab951df1d5d8e97a8338853f78355052237ee7c9a9f15597d4be681ec0ddced`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 1.3 MB (1294045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c06b480c0705fadb1ca66e86ad1dcfb125f0040b5c6b474b4d83d2471bd26c5`  
		Last Modified: Thu, 20 Aug 2020 19:22:42 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ece4d755805376a98bc9fc943536eb3543704dde5a5b5e1e95eb8b070d41c1`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4f1d6844aa2883e4a64693e98d8e5244cd83c0222b7525a89f8e157cf05b28`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c9bed45d4a36fc96b7f1672558f423cc8accc2219919ef94c4e98ed655fd26`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:3.3` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8de4eae4f224918279809bf279aae34e9f0c6e3c511a7b5d4b5d8d4098a56da3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.4 MB (375382197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c366797e4cfecafb86b468d01058cd326f765d6f8ebad7139dbeb1267fd74503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 19:03:13 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 19:03:14 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Mon, 10 Aug 2020 19:03:16 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Thu, 20 Aug 2020 19:43:27 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 20 Aug 2020 19:43:29 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:43:29 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:43:38 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 20 Aug 2020 19:43:38 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 19:43:39 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 20 Aug 2020 19:43:42 GMT
RUN mkdir -p /data/data /data/log
# Thu, 20 Aug 2020 19:43:43 GMT
VOLUME [/data]
# Thu, 20 Aug 2020 19:43:44 GMT
WORKDIR /data
# Thu, 20 Aug 2020 19:43:44 GMT
EXPOSE 4200 4300 5432
# Thu, 20 Aug 2020 19:43:45 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:43:45 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:43:46 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Thu, 20 Aug 2020 19:43:47 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 20 Aug 2020 19:43:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 19:43:48 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc4cf93e8037e4331888af64b2b357c893fad0ed8d78e1f3bc5fb195ac48210`  
		Last Modified: Mon, 10 Aug 2020 19:07:04 GMT  
		Size: 188.1 MB (188101411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa35411cdfc52e542e09354b26c7e0825ec1e298dea568e6e3b155e0d49776ad`  
		Last Modified: Mon, 10 Aug 2020 19:06:32 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933f86b390387a562c369674c43ccb0f5084b31bc670ad7adccf63e096d2380`  
		Last Modified: Thu, 20 Aug 2020 19:44:18 GMT  
		Size: 78.6 MB (78649806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080ea246110d4646eb27a035a5de791086786ae80245118798e5d815a3b2923f`  
		Last Modified: Thu, 20 Aug 2020 19:44:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a797717c2ce517c850d275f9bac6fe0d879d7bf7c06f746a3d205efb4173aa`  
		Last Modified: Thu, 20 Aug 2020 19:44:05 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0424997bc203f1bb866f4f9a15a51c82ba1310cf91d555ace39f57c100f71d9`  
		Last Modified: Thu, 20 Aug 2020 19:44:02 GMT  
		Size: 1.3 MB (1294046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b03f1552dce8d7356f65bd8799cf93700f2606eaf7299a6a9a6497df21cbdee`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb839d0f81abab88b6e4d7faba4ee2c91db0a2e625eaee0ffa59e56a768da36`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3119b24e75e1c2d67dccddc46394b99a7e5e7c27eadb0434206352418ba61fe`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45f279e7ecdd2663d1ac1a57c6e6cb18f730ff0856ce7b4a005b540a95b6f6`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:3.3.5`

```console
$ docker pull crate@sha256:79610eb88276d8434e58e7b456204fc796384cd4ecbc8efbd9d3c9fa2044faae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:3.3.5` - linux; amd64

```console
$ docker pull crate@sha256:287172d41a24589341527ae0de0698a8f93440a1ff19ccec021707afa150ec21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.5 MB (344547171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1959b9eb72576ad284b23e2a260f58278f2d5eb9229ed08335afe80f6cde9b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 18:51:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 18:51:48 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Mon, 10 Aug 2020 18:51:49 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Thu, 20 Aug 2020 19:22:17 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 20 Aug 2020 19:22:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:22:18 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:22:20 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 20 Aug 2020 19:22:20 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 19:22:20 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 20 Aug 2020 19:22:21 GMT
RUN mkdir -p /data/data /data/log
# Thu, 20 Aug 2020 19:22:21 GMT
VOLUME [/data]
# Thu, 20 Aug 2020 19:22:22 GMT
WORKDIR /data
# Thu, 20 Aug 2020 19:22:22 GMT
EXPOSE 4200 4300 5432
# Thu, 20 Aug 2020 19:22:22 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:22:22 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:22:22 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Thu, 20 Aug 2020 19:22:23 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 20 Aug 2020 19:22:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 19:22:23 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832e32314d6a05afed643636a2c1baad10515efbb71b1f01cfec46b085fbea14`  
		Last Modified: Mon, 10 Aug 2020 18:54:02 GMT  
		Size: 188.1 MB (188101329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fb76bc1732c60a3d3ddb00ea6d42ba52972c957dfa485b6d73bad734666b52`  
		Last Modified: Mon, 10 Aug 2020 18:53:45 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5b74ef97223994935b2e50f1e1a4536d1a29f2b164022cfc6a6236f96947dc`  
		Last Modified: Thu, 20 Aug 2020 19:22:50 GMT  
		Size: 79.3 MB (79283067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35c54368add1bc9b334fedadcff0bb8cd3eb1a33e8a8005cbde959534890f2`  
		Last Modified: Thu, 20 Aug 2020 19:22:42 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93357dd2cc916bd9e0e0865d8a9a0372e368e1367eeeb22e9d15de21c90596`  
		Last Modified: Thu, 20 Aug 2020 19:22:42 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab951df1d5d8e97a8338853f78355052237ee7c9a9f15597d4be681ec0ddced`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 1.3 MB (1294045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c06b480c0705fadb1ca66e86ad1dcfb125f0040b5c6b474b4d83d2471bd26c5`  
		Last Modified: Thu, 20 Aug 2020 19:22:42 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ece4d755805376a98bc9fc943536eb3543704dde5a5b5e1e95eb8b070d41c1`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4f1d6844aa2883e4a64693e98d8e5244cd83c0222b7525a89f8e157cf05b28`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c9bed45d4a36fc96b7f1672558f423cc8accc2219919ef94c4e98ed655fd26`  
		Last Modified: Thu, 20 Aug 2020 19:22:41 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:3.3.5` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:8de4eae4f224918279809bf279aae34e9f0c6e3c511a7b5d4b5d8d4098a56da3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.4 MB (375382197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c366797e4cfecafb86b468d01058cd326f765d6f8ebad7139dbeb1267fd74503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 19:03:13 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_linux-x64_bin.tar.gz     && echo "7a6bb980b9c91c478421f865087ad2d69086a0583aeeb9e69204785e8e97dcfd */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 19:03:14 GMT
ENV JAVA_HOME=/opt/jdk-11.0.1
# Mon, 10 Aug 2020 19:03:16 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-11.0.1/lib/security/cacerts
# Thu, 20 Aug 2020 19:43:27 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-3.3.5.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-3.3.5.tar.gz.asc crate-3.3.5.tar.gz     && rm -rf "$GNUPGHOME" crate-3.3.5.tar.gz.asc     && tar -xf crate-3.3.5.tar.gz -C /crate --strip-components=1     && rm crate-3.3.5.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Thu, 20 Aug 2020 19:43:29 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:43:29 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:43:38 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Thu, 20 Aug 2020 19:43:38 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 19:43:39 GMT
ENV CRATE_HEAP_SIZE=512M
# Thu, 20 Aug 2020 19:43:42 GMT
RUN mkdir -p /data/data /data/log
# Thu, 20 Aug 2020 19:43:43 GMT
VOLUME [/data]
# Thu, 20 Aug 2020 19:43:44 GMT
WORKDIR /data
# Thu, 20 Aug 2020 19:43:44 GMT
EXPOSE 4200 4300 5432
# Thu, 20 Aug 2020 19:43:45 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Thu, 20 Aug 2020 19:43:45 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Thu, 20 Aug 2020 19:43:46 GMT
LABEL maintainer=Crate.io <office@crate.io> org.label-schema.schema-version=1.0 org.label-schema.build-date=2020-08-20T09:47:47.048235 org.label-schema.name=crate org.label-schema.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.label-schema.url=https://crate.io/products/cratedb/ org.label-schema.vcs-url=https://github.com/crate/docker-crate org.label-schema.vendor=Crate.io org.label-schema.version=3.3.5
# Thu, 20 Aug 2020 19:43:47 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Thu, 20 Aug 2020 19:43:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 19:43:48 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc4cf93e8037e4331888af64b2b357c893fad0ed8d78e1f3bc5fb195ac48210`  
		Last Modified: Mon, 10 Aug 2020 19:07:04 GMT  
		Size: 188.1 MB (188101411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa35411cdfc52e542e09354b26c7e0825ec1e298dea568e6e3b155e0d49776ad`  
		Last Modified: Mon, 10 Aug 2020 19:06:32 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933f86b390387a562c369674c43ccb0f5084b31bc670ad7adccf63e096d2380`  
		Last Modified: Thu, 20 Aug 2020 19:44:18 GMT  
		Size: 78.6 MB (78649806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080ea246110d4646eb27a035a5de791086786ae80245118798e5d815a3b2923f`  
		Last Modified: Thu, 20 Aug 2020 19:44:05 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a797717c2ce517c850d275f9bac6fe0d879d7bf7c06f746a3d205efb4173aa`  
		Last Modified: Thu, 20 Aug 2020 19:44:05 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0424997bc203f1bb866f4f9a15a51c82ba1310cf91d555ace39f57c100f71d9`  
		Last Modified: Thu, 20 Aug 2020 19:44:02 GMT  
		Size: 1.3 MB (1294046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b03f1552dce8d7356f65bd8799cf93700f2606eaf7299a6a9a6497df21cbdee`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb839d0f81abab88b6e4d7faba4ee2c91db0a2e625eaee0ffa59e56a768da36`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3119b24e75e1c2d67dccddc46394b99a7e5e7c27eadb0434206352418ba61fe`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45f279e7ecdd2663d1ac1a57c6e6cb18f730ff0856ce7b4a005b540a95b6f6`  
		Last Modified: Thu, 20 Aug 2020 19:44:03 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0`

```console
$ docker pull crate@sha256:a98e06234fe3a8d388287230910d0c193f69f7cc53c8d481845d853eed4dedbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0` - linux; amd64

```console
$ docker pull crate@sha256:e00bff2dd39782d36457cd891d46bd9b37fdeb3895f7d18444addd15b5e05653
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337907214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2b1bc8bbc475017594be1e5d0bcadb3d3361c03f77fb0ebbcffd7dd496aa7f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 18:50:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 18:50:48 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Mon, 10 Aug 2020 18:50:49 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 18:51:05 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Mon, 10 Aug 2020 18:51:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 18:51:06 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 18:51:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 18:51:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 18:51:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 18:51:08 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 18:51:08 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 18:51:08 GMT
WORKDIR /data
# Mon, 10 Aug 2020 18:51:09 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 18:51:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 18:51:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 18:51:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Mon, 10 Aug 2020 18:51:09 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 18:51:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:51:10 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf855105041e7ee04646324ee09c0c50ec5eddc904d07931b10f0052dbac38`  
		Last Modified: Mon, 10 Aug 2020 18:53:39 GMT  
		Size: 198.1 MB (198127763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a503e291bd46b1caf2e7357ab1cff6effa07f5fef8f4e9910f97a425a5a166d`  
		Last Modified: Mon, 10 Aug 2020 18:53:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca76067f5f939c58ae8f6f57527eb0dc460c4ec8606127cfd7a89aca3aa1c2d`  
		Last Modified: Mon, 10 Aug 2020 18:53:27 GMT  
		Size: 62.6 MB (62616694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e426be22d7c01b008d2a79725ed3e1afebd5a9bfafc36bb4579f57f89c0ef916`  
		Last Modified: Mon, 10 Aug 2020 18:53:21 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34683dd9f0646e650f90777ac08e12e7440577f555d764ee82b60c3848060c04`  
		Last Modified: Mon, 10 Aug 2020 18:53:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a037e6345eee6a6e4d90831257e28beab2da94c3f48cae4c1b86e2077b7fbd`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 1.3 MB (1294034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c48d10fd9cc73428969505b88fc6e62732e3390d38e16e1c874228a8a6296`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9db80c36a2b0ae358913d6b355add49b7b47a394b79161bd07a729ef2955c1c`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f708fabfd006f199060fbf5b617136b510389684f5d31b9c6b954aed954ce`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaadbdb48e6fd0abb4df942a48d59108051177f6799ec8da92e1da3c0d1347e6`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.0` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:bc61d4431e0c6ed138f15deea1cf60389b493d12b6b6f5401be41e450bb94504
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.1 MB (369097087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c05303b33905ab922f62e833b54efe03775e0a6a86ff9c5fa4f84c81067b9d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 19:02:03 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 19:02:06 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Mon, 10 Aug 2020 19:02:08 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 19:02:30 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Mon, 10 Aug 2020 19:02:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 19:02:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 19:02:34 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 19:02:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 19:02:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 19:02:38 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 19:02:38 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 19:02:39 GMT
WORKDIR /data
# Mon, 10 Aug 2020 19:02:40 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 19:02:40 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 19:02:41 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 19:02:42 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Mon, 10 Aug 2020 19:02:42 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 19:02:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 19:02:44 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791e150dadc7478ca2a4921b4d9f2992c6094829853e90ff6a481a2c8ec4159e`  
		Last Modified: Mon, 10 Aug 2020 19:06:20 GMT  
		Size: 198.1 MB (198127553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea6fa262ab37c57c07b6f6a1bc06fd84d572929e4ed9ba9567ac3dd2a6600fa`  
		Last Modified: Mon, 10 Aug 2020 19:05:47 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9506c1a7d5aa9ab0048995897771f536fc39052e5abedc87e983164db94c5a`  
		Last Modified: Mon, 10 Aug 2020 19:05:56 GMT  
		Size: 62.3 MB (62338571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f667545a63024599829ee233db845fddcb82245a126892d3a27b221be83bf`  
		Last Modified: Mon, 10 Aug 2020 19:05:46 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b79a01b9aa3b61b3db365ac9f1d32411586fd4d885371a6d63c6f259b4b22f`  
		Last Modified: Mon, 10 Aug 2020 19:05:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6931e014cab492a84a1a1996cd68f045e1cd540ad124e400556f7e72147b486f`  
		Last Modified: Mon, 10 Aug 2020 19:05:45 GMT  
		Size: 1.3 MB (1294036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5924aa5e44462c8fe0b1462fbe4d75c7f5acabec7fb5a3fcd13e539569561`  
		Last Modified: Mon, 10 Aug 2020 19:05:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b008233369f3d9e2c2da6c0191dff5e05d2e1308b39c4a9150e2c7457e9fb7`  
		Last Modified: Mon, 10 Aug 2020 19:05:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200bca33a8981c51a69311ae589a4e236142ebc78918341721d0f5a31fd34631`  
		Last Modified: Mon, 10 Aug 2020 19:05:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ef6891f4af51401aa185f30137fa71fe8a4b776f2854363e143dc2cf065dd`  
		Last Modified: Mon, 10 Aug 2020 19:05:45 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.0.12`

```console
$ docker pull crate@sha256:a98e06234fe3a8d388287230910d0c193f69f7cc53c8d481845d853eed4dedbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.0.12` - linux; amd64

```console
$ docker pull crate@sha256:e00bff2dd39782d36457cd891d46bd9b37fdeb3895f7d18444addd15b5e05653
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.9 MB (337907214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2b1bc8bbc475017594be1e5d0bcadb3d3361c03f77fb0ebbcffd7dd496aa7f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 18:50:48 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 18:50:48 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Mon, 10 Aug 2020 18:50:49 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 18:51:05 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Mon, 10 Aug 2020 18:51:06 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 18:51:06 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 18:51:07 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 18:51:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 18:51:07 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 18:51:08 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 18:51:08 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 18:51:08 GMT
WORKDIR /data
# Mon, 10 Aug 2020 18:51:09 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 18:51:09 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 18:51:09 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 18:51:09 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Mon, 10 Aug 2020 18:51:09 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 18:51:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:51:10 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf855105041e7ee04646324ee09c0c50ec5eddc904d07931b10f0052dbac38`  
		Last Modified: Mon, 10 Aug 2020 18:53:39 GMT  
		Size: 198.1 MB (198127763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a503e291bd46b1caf2e7357ab1cff6effa07f5fef8f4e9910f97a425a5a166d`  
		Last Modified: Mon, 10 Aug 2020 18:53:21 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca76067f5f939c58ae8f6f57527eb0dc460c4ec8606127cfd7a89aca3aa1c2d`  
		Last Modified: Mon, 10 Aug 2020 18:53:27 GMT  
		Size: 62.6 MB (62616694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e426be22d7c01b008d2a79725ed3e1afebd5a9bfafc36bb4579f57f89c0ef916`  
		Last Modified: Mon, 10 Aug 2020 18:53:21 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34683dd9f0646e650f90777ac08e12e7440577f555d764ee82b60c3848060c04`  
		Last Modified: Mon, 10 Aug 2020 18:53:21 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a037e6345eee6a6e4d90831257e28beab2da94c3f48cae4c1b86e2077b7fbd`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 1.3 MB (1294034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c48d10fd9cc73428969505b88fc6e62732e3390d38e16e1c874228a8a6296`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9db80c36a2b0ae358913d6b355add49b7b47a394b79161bd07a729ef2955c1c`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f708fabfd006f199060fbf5b617136b510389684f5d31b9c6b954aed954ce`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaadbdb48e6fd0abb4df942a48d59108051177f6799ec8da92e1da3c0d1347e6`  
		Last Modified: Mon, 10 Aug 2020 18:53:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.0.12` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:bc61d4431e0c6ed138f15deea1cf60389b493d12b6b6f5401be41e450bb94504
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.1 MB (369097087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c05303b33905ab922f62e833b54efe03775e0a6a86ff9c5fa4f84c81067b9d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 19:02:03 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk12.0.1/69cfe15208a647278a19ef0990eea691/12/GPL/openjdk-12.0.1_linux-x64_bin.tar.gz     && echo "151eb4ec00f82e5e951126f572dc9116104c884d97f91be14ec11e85fc2dd626 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 19:02:06 GMT
ENV JAVA_HOME=/opt/jdk-12.0.1
# Mon, 10 Aug 2020 19:02:08 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-12.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 19:02:30 GMT
RUN yum install -y yum-utils https://centos7.iuscommunity.org/ius-release.rpm     && yum makecache     && yum install -y python36u openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.0.12.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.0.12.tar.gz.asc crate-4.0.12.tar.gz     && rm -rf "$GNUPGHOME" crate-4.0.12.tar.gz.asc     && tar -xf crate-4.0.12.tar.gz -C /crate --strip-components=1     && rm crate-4.0.12.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3     && ln -sf /usr/bin/python3.6 /usr/bin/python
# Mon, 10 Aug 2020 19:02:31 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 19:02:32 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 19:02:34 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 19:02:35 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 19:02:36 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 19:02:38 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 19:02:38 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 19:02:39 GMT
WORKDIR /data
# Mon, 10 Aug 2020 19:02:40 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 19:02:40 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 19:02:41 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 19:02:42 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-01-30T15:00:47.948355 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.0.12
# Mon, 10 Aug 2020 19:02:42 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 19:02:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 19:02:44 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791e150dadc7478ca2a4921b4d9f2992c6094829853e90ff6a481a2c8ec4159e`  
		Last Modified: Mon, 10 Aug 2020 19:06:20 GMT  
		Size: 198.1 MB (198127553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea6fa262ab37c57c07b6f6a1bc06fd84d572929e4ed9ba9567ac3dd2a6600fa`  
		Last Modified: Mon, 10 Aug 2020 19:05:47 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9506c1a7d5aa9ab0048995897771f536fc39052e5abedc87e983164db94c5a`  
		Last Modified: Mon, 10 Aug 2020 19:05:56 GMT  
		Size: 62.3 MB (62338571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f667545a63024599829ee233db845fddcb82245a126892d3a27b221be83bf`  
		Last Modified: Mon, 10 Aug 2020 19:05:46 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b79a01b9aa3b61b3db365ac9f1d32411586fd4d885371a6d63c6f259b4b22f`  
		Last Modified: Mon, 10 Aug 2020 19:05:46 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6931e014cab492a84a1a1996cd68f045e1cd540ad124e400556f7e72147b486f`  
		Last Modified: Mon, 10 Aug 2020 19:05:45 GMT  
		Size: 1.3 MB (1294036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5924aa5e44462c8fe0b1462fbe4d75c7f5acabec7fb5a3fcd13e539569561`  
		Last Modified: Mon, 10 Aug 2020 19:05:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b008233369f3d9e2c2da6c0191dff5e05d2e1308b39c4a9150e2c7457e9fb7`  
		Last Modified: Mon, 10 Aug 2020 19:05:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200bca33a8981c51a69311ae589a4e236142ebc78918341721d0f5a31fd34631`  
		Last Modified: Mon, 10 Aug 2020 19:05:44 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ef6891f4af51401aa185f30137fa71fe8a4b776f2854363e143dc2cf065dd`  
		Last Modified: Mon, 10 Aug 2020 19:05:45 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1`

```console
$ docker pull crate@sha256:ac98f4d55be041f26dfc6bccd7cf0b71a2775432a7d3343375ac808a89ce08f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1` - linux; amd64

```console
$ docker pull crate@sha256:91abf36bcb0b2b67a7e368320f908f7d81d42bb99db1d04cd6be50f581239bb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.1 MB (351127011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e69711de04e30f34f22afd16de9598e8e50e1baa112f240f333df55ada45b79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 18:49:46 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 18:49:47 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Mon, 10 Aug 2020 18:49:47 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 18:50:09 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 10 Aug 2020 18:50:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 18:50:12 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 18:50:12 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 18:50:12 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 18:50:13 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 18:50:13 GMT
WORKDIR /data
# Mon, 10 Aug 2020 18:50:13 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 18:50:13 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 18:50:13 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 18:50:14 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Mon, 10 Aug 2020 18:50:14 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 18:50:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:50:14 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174735e6a88b4c00fc6876074ee4b72d9c43bc43828af20b24df7bdf37a245a5`  
		Last Modified: Mon, 10 Aug 2020 18:53:15 GMT  
		Size: 196.4 MB (196423186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840a92b3414f60885212b02602cb7c8a154e62ceace7a0cd88a9779e7c24bbd`  
		Last Modified: Mon, 10 Aug 2020 18:52:57 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97c259dcae986157aae48b544f4a7d3f6379fa729e71cb4abd45ac72183f0c1`  
		Last Modified: Mon, 10 Aug 2020 18:53:05 GMT  
		Size: 77.5 MB (77542286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a1f4ce2fa02ffa6eefe39ade522ea2adc4a75ca1de9235f40c7b915850cf14`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 1.3 MB (1294035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954e67c484e4ee3ca38f5896f9241e3c0a1c25b0b7a30554ff46d979bac2c0fd`  
		Last Modified: Mon, 10 Aug 2020 18:52:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29843cc1cb726194acc2c9b3cf07af677327b9babb7dd7c58b9b861d9d3f634`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1aa7c40a86247d7aeca6655d4d7c8e2d2f6166f6b207f94b509ab31396821c`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8448a2cf71b38e6ee03edce56609c6e8d7b06cf852bfda1ee514d1a47e431c`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:823ad3752e3f870232f3f4d7a48d0312a38db8d4c192492093de3d6295ff4604
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.0 MB (381957375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f305fbe108cfadc60b2d91d96565b4e312b709c509fa8e9c1aff5e184e66530`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 19:00:19 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 19:00:21 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Mon, 10 Aug 2020 19:00:30 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 19:01:04 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 10 Aug 2020 19:01:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 19:01:12 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 19:01:13 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 19:01:14 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 19:01:15 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 19:01:16 GMT
WORKDIR /data
# Mon, 10 Aug 2020 19:01:17 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 19:01:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 19:01:19 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 19:01:19 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Mon, 10 Aug 2020 19:01:20 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 19:01:21 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ecf4fab6155ed8aeb124eeaf3042d4388fc85144b7e2f45cda3cbaa26acd5d`  
		Last Modified: Mon, 10 Aug 2020 19:05:36 GMT  
		Size: 196.4 MB (196423144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4396024f400eee15ad74f8349784c2b1e50dd7c2c5166eb5d4652ce9fd2d39e9`  
		Last Modified: Mon, 10 Aug 2020 19:05:04 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37e53a6f66bd51cce95116743baaa0399e26920e3b3e6a7243392a5528bc63`  
		Last Modified: Mon, 10 Aug 2020 19:05:18 GMT  
		Size: 76.9 MB (76904486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940dacf68d5a8ccda9782ae5a5072d6e05cc2750376ba02cfe692b904c0eccd3`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 1.3 MB (1294036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c0b2e4a3b26f907fd309aa6cc6012e56c4e7ca913e3acb0d2101f3b957180`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491ab978f141d5bec09320bfdf47020b0a1ceb9bfbeb4b86c11ae367859a19a`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf7e2455f8e1761dee0c9b6d9941e4456424a024b2c9ed044a3ea8a8ebed6d6`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690cfb6bef232e8dfb42a22857e4fbb63afcc4790aa5335015624695d04db802`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.1.8`

```console
$ docker pull crate@sha256:ac98f4d55be041f26dfc6bccd7cf0b71a2775432a7d3343375ac808a89ce08f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.1.8` - linux; amd64

```console
$ docker pull crate@sha256:91abf36bcb0b2b67a7e368320f908f7d81d42bb99db1d04cd6be50f581239bb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.1 MB (351127011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e69711de04e30f34f22afd16de9598e8e50e1baa112f240f333df55ada45b79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 18:49:46 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 18:49:47 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Mon, 10 Aug 2020 18:49:47 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 18:50:09 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 10 Aug 2020 18:50:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 18:50:12 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 18:50:12 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 18:50:12 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 18:50:13 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 18:50:13 GMT
WORKDIR /data
# Mon, 10 Aug 2020 18:50:13 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 18:50:13 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 18:50:13 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 18:50:14 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Mon, 10 Aug 2020 18:50:14 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 18:50:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:50:14 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174735e6a88b4c00fc6876074ee4b72d9c43bc43828af20b24df7bdf37a245a5`  
		Last Modified: Mon, 10 Aug 2020 18:53:15 GMT  
		Size: 196.4 MB (196423186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8840a92b3414f60885212b02602cb7c8a154e62ceace7a0cd88a9779e7c24bbd`  
		Last Modified: Mon, 10 Aug 2020 18:52:57 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97c259dcae986157aae48b544f4a7d3f6379fa729e71cb4abd45ac72183f0c1`  
		Last Modified: Mon, 10 Aug 2020 18:53:05 GMT  
		Size: 77.5 MB (77542286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a1f4ce2fa02ffa6eefe39ade522ea2adc4a75ca1de9235f40c7b915850cf14`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 1.3 MB (1294035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954e67c484e4ee3ca38f5896f9241e3c0a1c25b0b7a30554ff46d979bac2c0fd`  
		Last Modified: Mon, 10 Aug 2020 18:52:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29843cc1cb726194acc2c9b3cf07af677327b9babb7dd7c58b9b861d9d3f634`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1aa7c40a86247d7aeca6655d4d7c8e2d2f6166f6b207f94b509ab31396821c`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8448a2cf71b38e6ee03edce56609c6e8d7b06cf852bfda1ee514d1a47e431c`  
		Last Modified: Mon, 10 Aug 2020 18:52:56 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.1.8` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:823ad3752e3f870232f3f4d7a48d0312a38db8d4c192492093de3d6295ff4604
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.0 MB (381957375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f305fbe108cfadc60b2d91d96565b4e312b709c509fa8e9c1aff5e184e66530`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Mon, 10 Aug 2020 19:00:19 GMT
RUN curl --retry 8 -o /openjdk.tar.gz https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz     && echo "2e01716546395694d3fad54c9b36d1cd46c5894c06f72d156772efbcf4b41335 */openjdk.tar.gz" | sha256sum -c -     && tar -C /opt -zxf /openjdk.tar.gz     && rm /openjdk.tar.gz
# Mon, 10 Aug 2020 19:00:21 GMT
ENV JAVA_HOME=/opt/jdk-13.0.1
# Mon, 10 Aug 2020 19:00:30 GMT
RUN ln -sf /etc/pki/ca-trust/extracted/java/cacerts /opt/jdk-13.0.1/lib/security/cacerts
# Mon, 10 Aug 2020 19:01:04 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.8.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.8.tar.gz.asc crate-4.1.8.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.8.tar.gz.asc     && tar -xf crate-4.1.8.tar.gz -C /crate --strip-components=1     && rm crate-4.1.8.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 10 Aug 2020 19:01:11 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 10 Aug 2020 19:01:12 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 Aug 2020 19:01:13 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 10 Aug 2020 19:01:14 GMT
RUN mkdir -p /data/data /data/log
# Mon, 10 Aug 2020 19:01:15 GMT
VOLUME [/data]
# Mon, 10 Aug 2020 19:01:16 GMT
WORKDIR /data
# Mon, 10 Aug 2020 19:01:17 GMT
EXPOSE 4200 4300 5432
# Mon, 10 Aug 2020 19:01:18 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 10 Aug 2020 19:01:19 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 10 Aug 2020 19:01:19 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-07-07T09:24:31.760994 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.8
# Mon, 10 Aug 2020 19:01:20 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 10 Aug 2020 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 19:01:21 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ecf4fab6155ed8aeb124eeaf3042d4388fc85144b7e2f45cda3cbaa26acd5d`  
		Last Modified: Mon, 10 Aug 2020 19:05:36 GMT  
		Size: 196.4 MB (196423144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4396024f400eee15ad74f8349784c2b1e50dd7c2c5166eb5d4652ce9fd2d39e9`  
		Last Modified: Mon, 10 Aug 2020 19:05:04 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37e53a6f66bd51cce95116743baaa0399e26920e3b3e6a7243392a5528bc63`  
		Last Modified: Mon, 10 Aug 2020 19:05:18 GMT  
		Size: 76.9 MB (76904486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940dacf68d5a8ccda9782ae5a5072d6e05cc2750376ba02cfe692b904c0eccd3`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 1.3 MB (1294036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c0b2e4a3b26f907fd309aa6cc6012e56c4e7ca913e3acb0d2101f3b957180`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491ab978f141d5bec09320bfdf47020b0a1ceb9bfbeb4b86c11ae367859a19a`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf7e2455f8e1761dee0c9b6d9941e4456424a024b2c9ed044a3ea8a8ebed6d6`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690cfb6bef232e8dfb42a22857e4fbb63afcc4790aa5335015624695d04db802`  
		Last Modified: Mon, 10 Aug 2020 19:05:01 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2`

```console
$ docker pull crate@sha256:f2e2c6bd17fa47d621f54b356e61ddca7fe290435f0014887bd7c7daee61dcf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:4.2` - linux; amd64

```console
$ docker pull crate@sha256:7c606555b4ec7203e007995b238a58696bbc02af02384c6edb19a6520f9a1935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332854845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5aa357548464054ee254193b9b7f21d4ae359cb0af1342eb3d7cdb08b8370e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 14 Oct 2020 10:11:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.6.tar.gz.asc crate-4.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.6.tar.gz.asc     && tar -xf crate-4.2.6.tar.gz -C /crate --strip-components=1     && rm crate-4.2.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 14 Oct 2020 10:11:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 14 Oct 2020 10:11:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Oct 2020 10:11:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 14 Oct 2020 10:11:11 GMT
RUN mkdir -p /data/data /data/log
# Wed, 14 Oct 2020 10:11:11 GMT
VOLUME [/data]
# Wed, 14 Oct 2020 10:11:11 GMT
WORKDIR /data
# Wed, 14 Oct 2020 10:11:12 GMT
EXPOSE 4200 4300 5432
# Wed, 14 Oct 2020 10:11:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 14 Oct 2020 10:11:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 14 Oct 2020 10:11:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-08T13:14:47.102454 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.6
# Wed, 14 Oct 2020 10:11:12 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 14 Oct 2020 10:11:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Oct 2020 10:11:13 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805c434feea4480105e814f46b3662c7ff967bd75b7d8d82324a2d9f2786e537`  
		Last Modified: Wed, 14 Oct 2020 10:12:02 GMT  
		Size: 255.4 MB (255419872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db202556aacbd602456f1a304d6184daacfda3c188fc014b5d35dae47cb4e0`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 1.6 MB (1567708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9a325dea6c3edf2fc05c18c78f5faaa861cda13ffec68f96f431f481c4364e`  
		Last Modified: Wed, 14 Oct 2020 10:11:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400729202a0eebe4fd1bdd623a878d72b34eccb95d1b4248c1023521c92e06f`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938404ac8bd1f5ae2a39dfe246f9a2d05643ca40b064686b352ede8ad9090a59`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd42d0538a68fdedf67fcee3ce620bb59b5f5cdd74e95545bb965106f4144a7`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:4.2` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:b9b41d6eb51aa90abc38799ec9d602f857fa3537c1bbf6684c4ca9ce18566ef6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (361036387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744f3fe46d259b43f28baef802b19abaf42c56e4ba83c3a259429732a5162f41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 02 Sep 2020 18:40:51 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.4.tar.gz.asc crate-4.2.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.4.tar.gz.asc     && tar -xf crate-4.2.4.tar.gz -C /crate --strip-components=1     && rm crate-4.2.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 02 Sep 2020 18:40:57 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 02 Sep 2020 18:40:57 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Sep 2020 18:40:58 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 02 Sep 2020 18:41:00 GMT
RUN mkdir -p /data/data /data/log
# Wed, 02 Sep 2020 18:41:00 GMT
VOLUME [/data]
# Wed, 02 Sep 2020 18:41:01 GMT
WORKDIR /data
# Wed, 02 Sep 2020 18:41:02 GMT
EXPOSE 4200 4300 5432
# Wed, 02 Sep 2020 18:41:02 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 02 Sep 2020 18:41:03 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 02 Sep 2020 18:41:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-08-27T15:44:44.777677 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.4
# Wed, 02 Sep 2020 18:41:04 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 02 Sep 2020 18:41:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Sep 2020 18:41:06 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cc9a394ae3340100e02b45fdb6abc4da5e20136701666e63096693c16fc4c2`  
		Last Modified: Wed, 02 Sep 2020 18:42:25 GMT  
		Size: 252.2 MB (252197643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8a7a7df4642c6625ff498623afed02ccc9bcec27e9b1c6816426f9e5be657e`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 1.5 MB (1503275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9891523b7359ff8a6248439af975bc6a6707a8579076f81d0eb6650de234cb`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3559386b545630be735be11d2ba2dc9ef5b99eecee4b6cc3a6eb310cb297c832`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9788278e294fb0cce7814bc9590e05d3905733360fd3ce4c954d00c056e5cbf`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfd6df58d93dde5a02b62b4206f9b539c843121d4d6d228dcfcf282dd898e1b`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:4.2.6`

```console
$ docker pull crate@sha256:5ce9d06d088516d02674d9d125d48adf8bd0e2701e46cd2bb8da515220e215ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:4.2.6` - linux; amd64

```console
$ docker pull crate@sha256:7c606555b4ec7203e007995b238a58696bbc02af02384c6edb19a6520f9a1935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332854845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5aa357548464054ee254193b9b7f21d4ae359cb0af1342eb3d7cdb08b8370e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 14 Oct 2020 10:11:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.6.tar.gz.asc crate-4.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.6.tar.gz.asc     && tar -xf crate-4.2.6.tar.gz -C /crate --strip-components=1     && rm crate-4.2.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 14 Oct 2020 10:11:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 14 Oct 2020 10:11:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Oct 2020 10:11:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 14 Oct 2020 10:11:11 GMT
RUN mkdir -p /data/data /data/log
# Wed, 14 Oct 2020 10:11:11 GMT
VOLUME [/data]
# Wed, 14 Oct 2020 10:11:11 GMT
WORKDIR /data
# Wed, 14 Oct 2020 10:11:12 GMT
EXPOSE 4200 4300 5432
# Wed, 14 Oct 2020 10:11:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 14 Oct 2020 10:11:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 14 Oct 2020 10:11:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-08T13:14:47.102454 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.6
# Wed, 14 Oct 2020 10:11:12 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 14 Oct 2020 10:11:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Oct 2020 10:11:13 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805c434feea4480105e814f46b3662c7ff967bd75b7d8d82324a2d9f2786e537`  
		Last Modified: Wed, 14 Oct 2020 10:12:02 GMT  
		Size: 255.4 MB (255419872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db202556aacbd602456f1a304d6184daacfda3c188fc014b5d35dae47cb4e0`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 1.6 MB (1567708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9a325dea6c3edf2fc05c18c78f5faaa861cda13ffec68f96f431f481c4364e`  
		Last Modified: Wed, 14 Oct 2020 10:11:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400729202a0eebe4fd1bdd623a878d72b34eccb95d1b4248c1023521c92e06f`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938404ac8bd1f5ae2a39dfe246f9a2d05643ca40b064686b352ede8ad9090a59`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd42d0538a68fdedf67fcee3ce620bb59b5f5cdd74e95545bb965106f4144a7`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:f2e2c6bd17fa47d621f54b356e61ddca7fe290435f0014887bd7c7daee61dcf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:7c606555b4ec7203e007995b238a58696bbc02af02384c6edb19a6520f9a1935
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332854845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5aa357548464054ee254193b9b7f21d4ae359cb0af1342eb3d7cdb08b8370e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:48:08 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 14 Oct 2020 10:11:08 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.6.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.6.tar.gz.asc crate-4.2.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.6.tar.gz.asc     && tar -xf crate-4.2.6.tar.gz -C /crate --strip-components=1     && rm crate-4.2.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 14 Oct 2020 10:11:10 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.26.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.26.0.asc crash_standalone_0.26.0     && rm -rf "$GNUPGHOME" crash_standalone_0.26.0.asc     && mv crash_standalone_0.26.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 14 Oct 2020 10:11:10 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Oct 2020 10:11:10 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 14 Oct 2020 10:11:11 GMT
RUN mkdir -p /data/data /data/log
# Wed, 14 Oct 2020 10:11:11 GMT
VOLUME [/data]
# Wed, 14 Oct 2020 10:11:11 GMT
WORKDIR /data
# Wed, 14 Oct 2020 10:11:12 GMT
EXPOSE 4200 4300 5432
# Wed, 14 Oct 2020 10:11:12 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 14 Oct 2020 10:11:12 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 14 Oct 2020 10:11:12 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-10-08T13:14:47.102454 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.6
# Wed, 14 Oct 2020 10:11:12 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 14 Oct 2020 10:11:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Oct 2020 10:11:13 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d441d1d9ac83b78fd083af4a0582951c2f9626f76ae45c164970f5cfc1a6c0`  
		Last Modified: Mon, 10 Aug 2020 18:52:27 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805c434feea4480105e814f46b3662c7ff967bd75b7d8d82324a2d9f2786e537`  
		Last Modified: Wed, 14 Oct 2020 10:12:02 GMT  
		Size: 255.4 MB (255419872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db202556aacbd602456f1a304d6184daacfda3c188fc014b5d35dae47cb4e0`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 1.6 MB (1567708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9a325dea6c3edf2fc05c18c78f5faaa861cda13ffec68f96f431f481c4364e`  
		Last Modified: Wed, 14 Oct 2020 10:11:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3400729202a0eebe4fd1bdd623a878d72b34eccb95d1b4248c1023521c92e06f`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938404ac8bd1f5ae2a39dfe246f9a2d05643ca40b064686b352ede8ad9090a59`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd42d0538a68fdedf67fcee3ce620bb59b5f5cdd74e95545bb965106f4144a7`  
		Last Modified: Wed, 14 Oct 2020 10:11:36 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:b9b41d6eb51aa90abc38799ec9d602f857fa3537c1bbf6684c4ca9ce18566ef6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (361036387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744f3fe46d259b43f28baef802b19abaf42c56e4ba83c3a259429732a5162f41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Mon, 10 Aug 2020 18:40:15 GMT
ADD file:bd33d5894d5b88d0234cb910fde969eb9864ff572b5f9c61d7e847e0d25eab07 in / 
# Mon, 10 Aug 2020 18:40:21 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:40:21 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:57:45 GMT
RUN groupadd crate && useradd -u 1000 -g crate -d /crate crate
# Wed, 02 Sep 2020 18:40:51 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && export PLATFORM="$(         case $(uname --m) in             x86_64)  echo x64_linux ;;             aarch64) echo aarch64_linux ;;         esac)"     && export CRATE_URL=https://cdn.crate.io/downloads/releases/cratedb/${PLATFORM}/crate-4.2.4.tar.gz     && curl -fSL -O ${CRATE_URL}     && curl -fSL -O ${CRATE_URL}.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.2.4.tar.gz.asc crate-4.2.4.tar.gz     && rm -rf "$GNUPGHOME" crate-4.2.4.tar.gz.asc     && tar -xf crate-4.2.4.tar.gz -C /crate --strip-components=1     && rm crate-4.2.4.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 02 Sep 2020 18:40:57 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.25.0.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.25.0.asc crash_standalone_0.25.0     && rm -rf "$GNUPGHOME" crash_standalone_0.25.0.asc     && mv crash_standalone_0.25.0 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 02 Sep 2020 18:40:57 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Sep 2020 18:40:58 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 02 Sep 2020 18:41:00 GMT
RUN mkdir -p /data/data /data/log
# Wed, 02 Sep 2020 18:41:00 GMT
VOLUME [/data]
# Wed, 02 Sep 2020 18:41:01 GMT
WORKDIR /data
# Wed, 02 Sep 2020 18:41:02 GMT
EXPOSE 4200 4300 5432
# Wed, 02 Sep 2020 18:41:02 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 02 Sep 2020 18:41:03 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 02 Sep 2020 18:41:04 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-08-27T15:44:44.777677 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.2.4
# Wed, 02 Sep 2020 18:41:04 GMT
COPY file:2e0f9e8c9006d6d56e9be42bd5646f68ec854481fcfbe51bafbf8695dc44b38a in / 
# Wed, 02 Sep 2020 18:41:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Sep 2020 18:41:06 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:9f74aa7d9ab9b412a3fcf68bb81925361c12040976f82e40aec2a10d83fb0ec6`  
		Last Modified: Mon, 10 Aug 2020 18:41:57 GMT  
		Size: 107.3 MB (107331333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d842dc7b645168ea409e9ba5027fb863651b5c2d56bde60d64a87c7867f5c988`  
		Last Modified: Mon, 10 Aug 2020 19:04:09 GMT  
		Size: 2.3 KB (2253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cc9a394ae3340100e02b45fdb6abc4da5e20136701666e63096693c16fc4c2`  
		Last Modified: Wed, 02 Sep 2020 18:42:25 GMT  
		Size: 252.2 MB (252197643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8a7a7df4642c6625ff498623afed02ccc9bcec27e9b1c6816426f9e5be657e`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 1.5 MB (1503275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9891523b7359ff8a6248439af975bc6a6707a8579076f81d0eb6650de234cb`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3559386b545630be735be11d2ba2dc9ef5b99eecee4b6cc3a6eb310cb297c832`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9788278e294fb0cce7814bc9590e05d3905733360fd3ce4c954d00c056e5cbf`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfd6df58d93dde5a02b62b4206f9b539c843121d4d6d228dcfcf282dd898e1b`  
		Last Modified: Wed, 02 Sep 2020 18:41:41 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
