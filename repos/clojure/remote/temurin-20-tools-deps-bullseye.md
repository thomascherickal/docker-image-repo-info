## `clojure:temurin-20-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:a8fac93f7dfb4c9cade38904bd23467f55bc2c02371177be07d9ed04b7c4f919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:26db38ff91cbf949c6aa2f627204807fb431aef90a55203eea10a11a4415f3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.7 MB (280742898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32f696e9dd5ed5b260427f9f1eedc878c9f72dcbb7294f00dcdf327462ece91`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 03:24:49 GMT
COPY dir:6a540db71f2a37db361084aee8addd6817cd7c4f18237e6f852a38e98bdb4182 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:24:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:26:03 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:26:03 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:26:19 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:26:20 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:26:20 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 14 Aug 2023 23:26:20 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 14 Aug 2023 23:26:20 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7b3791075e937ca44303722209d883595c7671dd2a19c46338ac19c38a452`  
		Last Modified: Fri, 28 Jul 2023 03:33:09 GMT  
		Size: 153.8 MB (153791746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6a2f4e31dfe6d5de25935b9d8a2f045830f99a019faea60367290d6bbd8526`  
		Last Modified: Mon, 14 Aug 2023 23:34:17 GMT  
		Size: 71.9 MB (71894563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01c69b046b0cbfacad55a4556bea1b8b1266016065753175eb59220891f4113`  
		Last Modified: Mon, 14 Aug 2023 23:34:10 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894ea0b8feda388ca283fd33ba3aeafac76f7557f1bf58af91064df6179386be`  
		Last Modified: Mon, 14 Aug 2023 23:34:10 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:66e644341a50150f8312f1b9b443657ce119acad50ed110c1c0112fb97c616d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277827666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b85050e39ad549e06a88f800bb0506d513fae9caa25427cffa8d568419f7fb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 14:37:27 GMT
COPY dir:d35c6357dd030960bb6081f48b2bc10afb3da11efc1525ff916214b03be70ddf in /opt/java/openjdk 
# Fri, 28 Jul 2023 14:37:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:38:17 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Fri, 28 Jul 2023 14:38:17 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 14:38:31 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Jul 2023 14:38:32 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Jul 2023 14:38:32 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Jul 2023 14:38:32 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Jul 2023 14:38:32 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785f9c63aa786ee3ab03231f07e1160261941272ad745ade935aa994d34f0dc9`  
		Last Modified: Fri, 28 Jul 2023 14:44:47 GMT  
		Size: 152.1 MB (152120124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d630dc7f0257f86dafe6a52d22a7e6fe63e8d9588fda21201b3af6b4755188ab`  
		Last Modified: Fri, 28 Jul 2023 14:45:23 GMT  
		Size: 72.0 MB (72001735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab1f1d0d68d6d2ba692c27317197b33cf0f924bbb5c855258f2b80ea21b72e4`  
		Last Modified: Fri, 28 Jul 2023 14:45:16 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d25271df5583791cdb302339c60dc94ffff0f3ca1300742c21ae0e4a28a609`  
		Last Modified: Fri, 28 Jul 2023 14:45:16 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
