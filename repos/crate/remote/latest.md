## `crate:latest`

```console
$ docker pull crate@sha256:ff26a7403c7177fb9ce0916e0a32dbfe202b9825d00a7758a668806d47302c57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:4e13e6c35d1ecf00fff386999c85bf3f8c8468ae748c3b82b9fb4851066121dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.2 MB (351229492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0715a8cf24d45e87392bd7530ea1dc1e304ff5640f8e84991fbbe2c3c39975fd`
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
# Mon, 29 Jun 2020 20:24:26 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.7.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.7.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.7.tar.gz.asc crate-4.1.7.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.7.tar.gz.asc     && tar -xf crate-4.1.7.tar.gz -C /crate --strip-components=1     && rm crate-4.1.7.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Mon, 29 Jun 2020 20:24:28 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Mon, 29 Jun 2020 20:24:28 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Jun 2020 20:24:28 GMT
ENV CRATE_HEAP_SIZE=512M
# Mon, 29 Jun 2020 20:24:29 GMT
RUN mkdir -p /data/data /data/log
# Mon, 29 Jun 2020 20:24:29 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:24:29 GMT
WORKDIR /data
# Mon, 29 Jun 2020 20:24:30 GMT
EXPOSE 4200 4300 5432
# Mon, 29 Jun 2020 20:24:30 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Mon, 29 Jun 2020 20:24:30 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Mon, 29 Jun 2020 20:24:30 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-06-24T16:41:26.302384 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.7
# Mon, 29 Jun 2020 20:24:30 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Mon, 29 Jun 2020 20:24:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 29 Jun 2020 20:24:31 GMT
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
	-	`sha256:53b86e21c03b3479ee0d3b69bcdbe6da5b7a583dcf45b26226581926767d608a`  
		Last Modified: Mon, 29 Jun 2020 20:24:56 GMT  
		Size: 77.6 MB (77627847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2654c5ec64512003432abfcff4f21d50a3108caa9181d10666ae0db3ef141e3`  
		Last Modified: Mon, 29 Jun 2020 20:24:47 GMT  
		Size: 1.3 MB (1294053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5560f870ec036764f4dfda88c620387df819174ecfbfc0a1b85995f4617f9e`  
		Last Modified: Mon, 29 Jun 2020 20:24:47 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa1ddbfae1d2de7064f86b15a59fe8c99817bdf876337ad10ef210c1ff0d05c`  
		Last Modified: Mon, 29 Jun 2020 20:24:47 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5614427c6ffa4dbe11861c2c02c13cb1b15a77b31ca5c59263afcabb3f416bf0`  
		Last Modified: Mon, 29 Jun 2020 20:24:47 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb795252b44b12c30a901000e82e7a6f220de30d0caaa1dff60d71ac2e62bd6b`  
		Last Modified: Mon, 29 Jun 2020 20:24:47 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crate:latest` - linux; arm64 variant v8

```console
$ docker pull crate@sha256:dc245f85de4c5e54a81ed29e45082bf5bb705e1f04d86fb792bcee3b400ff5fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.4 MB (378373960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fdf0d8f0aa57a5973f11a995a0472bdaf14153110f8832400a7fa29d1f870c9`
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
# Wed, 10 Jun 2020 18:42:03 GMT
RUN yum install -y yum-utils     && yum makecache     && yum install -y python36 openssl     && yum clean all     && rm -rf /var/cache/yum     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.6.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-4.1.6.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-4.1.6.tar.gz.asc crate-4.1.6.tar.gz     && rm -rf "$GNUPGHOME" crate-4.1.6.tar.gz.asc     && tar -xf crate-4.1.6.tar.gz -C /crate --strip-components=1     && rm crate-4.1.6.tar.gz     && ln -sf /usr/bin/python3.6 /usr/bin/python3
# Wed, 10 Jun 2020 18:42:08 GMT
RUN curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2     && curl -fSL -O https://cdn.crate.io/downloads/releases/crash_standalone_0.24.2.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crash_standalone_0.24.2.asc crash_standalone_0.24.2     && rm -rf "$GNUPGHOME" crash_standalone_0.24.2.asc     && mv crash_standalone_0.24.2 /usr/local/bin/crash     && chmod +x /usr/local/bin/crash
# Wed, 10 Jun 2020 18:42:08 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Jun 2020 18:42:09 GMT
ENV CRATE_HEAP_SIZE=512M
# Wed, 10 Jun 2020 18:42:11 GMT
RUN mkdir -p /data/data /data/log
# Wed, 10 Jun 2020 18:42:11 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 18:42:13 GMT
WORKDIR /data
# Wed, 10 Jun 2020 18:42:13 GMT
EXPOSE 4200 4300 5432
# Wed, 10 Jun 2020 18:42:14 GMT
COPY --chown=1000:0file:bff8d2f33b7a44d36fcd66fc7e7d92b0ee463d0eb0df2a56e42511d4f1b3e9b2 in /crate/config/crate.yml 
# Wed, 10 Jun 2020 18:42:14 GMT
COPY --chown=1000:0file:5f0d1b776d3a6517508a00a88f8053bd0933a642599374c9dff00dc3b632fd09 in /crate/config/log4j2.properties 
# Wed, 10 Jun 2020 18:42:15 GMT
LABEL maintainer=Crate.io <office@crate.io> org.opencontainers.image.created=2020-06-08T09:38:55.376569 org.opencontainers.image.title=crate org.opencontainers.image.description=CrateDB is a distributed SQL database handles massive amounts of machine data in real-time. org.opencontainers.image.url=https://crate.io/products/cratedb/ org.opencontainers.image.source=https://github.com/crate/docker-crate org.opencontainers.image.vendor=Crate.io org.opencontainers.image.version=4.1.6
# Wed, 10 Jun 2020 18:42:15 GMT
COPY file:9830363b41b8063591887d9dc9ce2767bf0e91dc4cb05efcb6ea622a60ec15e3 in / 
# Wed, 10 Jun 2020 18:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 18:42:17 GMT
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
	-	`sha256:45a795756f03ab83dd6c6d62190914abf2695536c70b757cd1c5b38f7cd69c07`  
		Last Modified: Wed, 10 Jun 2020 18:50:47 GMT  
		Size: 76.1 MB (76096900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccc1d5a0e6b6b33a56931a22d7ad51f3f8e511313a9cd72cabca38ecd48baed`  
		Last Modified: Wed, 10 Jun 2020 18:50:27 GMT  
		Size: 1.3 MB (1294036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b72dd3df5e051cc529b6a43641ff71c8f11791efdc1e58acaeb6e4e1a6c20a`  
		Last Modified: Wed, 10 Jun 2020 18:50:27 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f85610c334ef57396c874f4c4b8ac2b6161781936a26b5f32edb11d25565212`  
		Last Modified: Wed, 10 Jun 2020 18:50:26 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c07dbd00e07253f7249eed2812d6088a4a0fdd22b1b00fc3c657b2e1b189c58`  
		Last Modified: Wed, 10 Jun 2020 18:50:27 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6487781b0b6a5757997b2a8f307b16b8f57dc6b437f62602972d183b807975c`  
		Last Modified: Wed, 10 Jun 2020 18:50:26 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
