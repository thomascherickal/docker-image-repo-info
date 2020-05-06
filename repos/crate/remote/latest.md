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
