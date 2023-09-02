## `clojure:temurin-17-bullseye-slim`

```console
$ docker pull clojure@sha256:24ffe5727e617b12ea396d7213bbb1f852049c37205bec8235267c5d95c8ba44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:6b65758812cd90db237349d06832725a5048812119548cf6fdc862779a29a271
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237688074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d3321ddb2dba2948effdc11a726359b6d9dad7b8ec3f0f7e1b2d1fa5a9c70b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 20:48:51 GMT
COPY dir:6777d1f77166c2ecdd8f4eb23f5fd82574aa8a90fd65d6dff981fbb31778a3d1 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:31:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:38:04 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Thu, 31 Aug 2023 23:38:04 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:38:20 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 31 Aug 2023 23:38:20 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 31 Aug 2023 23:38:20 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 31 Aug 2023 23:38:20 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 31 Aug 2023 23:38:20 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65006a4851e206ccc53a9bf891b081e6fefbdbe0fcb897d670970fc7f2eff9ea`  
		Last Modified: Thu, 31 Aug 2023 20:51:41 GMT  
		Size: 144.8 MB (144775820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5044695fd17bf3f973e31581a2e8b9aba6ffae8a40434ff241ac30305d9e0b`  
		Last Modified: Thu, 31 Aug 2023 23:47:09 GMT  
		Size: 61.5 MB (61493559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9da5e7b90344baa0cd3afe316d7e7b261298d41c2aebe2fbec7e1042aa158`  
		Last Modified: Thu, 31 Aug 2023 23:47:01 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0083784da58fdcbd300f81a2c9976afde929e5ba9ea112091cc13d29b46ff0`  
		Last Modified: Thu, 31 Aug 2023 23:47:01 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d56bc6c3d4ad7f6e3790dbd86e3e42193fa0aab734bf5346ce29c400f88fe91d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235218789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37cab92b74782bb354220d9e5b08fbcea5cea482841a24936afe768f750d33e1`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:48:00 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:48:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:49:57 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Sat, 02 Sep 2023 01:49:57 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:50:10 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 02 Sep 2023 01:50:11 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 02 Sep 2023 01:50:11 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Sat, 02 Sep 2023 01:50:11 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Sep 2023 01:50:11 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75390d7bc4a96162e240272aeff28881955f7af498179aa85faecd879748f913`  
		Last Modified: Sat, 02 Sep 2023 01:55:46 GMT  
		Size: 143.5 MB (143543515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d03dc17b915978012134be2e29b4f89c5c9c01664b8080862a16428e4a86fe9`  
		Last Modified: Sat, 02 Sep 2023 01:57:18 GMT  
		Size: 61.6 MB (61611440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0bbf82a7d999c46f1a91774ae920d7673309443101cd2ddc5881870482cf82`  
		Last Modified: Sat, 02 Sep 2023 01:57:12 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e06cacbc944d5277917665a2eb9b7d65adc620b49e435dc3cdac269231a8a`  
		Last Modified: Sat, 02 Sep 2023 01:57:12 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
