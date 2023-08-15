## `clojure:temurin-8-bullseye`

```console
$ docker pull clojure@sha256:a078f5cd03fa4ea589cc92cb3834eef22f0eeb6b11be0beca04a066847517985
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:0872eb6d87c3d5c7f7edbcc71790d98c854e43ca307dfb934907b0df426f1903
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230535630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05463ef2247ea25d557f55e19576ebe2a3cfb463f9ed6c2c56e7c9fb8ae7884`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 01 Aug 2023 22:04:20 GMT
COPY dir:66cfc1773e07dead4d108eefca05e38bbe528aec6797deefc0559c5a4d41e721 in /opt/java/openjdk 
# Tue, 01 Aug 2023 22:04:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:20:42 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:20:42 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:21:03 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:21:03 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:21:03 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5994baf91037b8621fd988336f98795e08c9c32f2a733406596f429bf2ee92`  
		Last Modified: Tue, 01 Aug 2023 22:15:16 GMT  
		Size: 103.6 MB (103585038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3ae8406ef8d80708d63ac45b61196ca223e12fd3222008daa5d825309495d2`  
		Last Modified: Mon, 14 Aug 2023 23:29:15 GMT  
		Size: 71.9 MB (71894404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7109777b8ffb7c343b82a121534b6eb2d1dbd1b3e6b6953cef923e9fba6d3b1`  
		Last Modified: Mon, 14 Aug 2023 23:29:08 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7b056da836a610716231ee52e269f026e4a68f5fc6939728952868c9b7290981
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.4 MB (228397027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d4d35a221895bf51a7be043fcc2eb5ff9fb745be35f83a85f4db374a0a147ef`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 01 Aug 2023 22:10:28 GMT
COPY dir:b83f0a0f236c1f97de459c8ae266f437d3630abb3700f3b868301c8fe017c49a in /opt/java/openjdk 
# Tue, 01 Aug 2023 22:10:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Aug 2023 22:14:14 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 01 Aug 2023 22:14:14 GMT
WORKDIR /tmp
# Tue, 01 Aug 2023 22:14:30 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 01 Aug 2023 22:14:30 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 01 Aug 2023 22:14:30 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c068dad8acfadc68ead3eb00398372dcec29fed6a09eca2f88f82eca8ecd10`  
		Last Modified: Tue, 01 Aug 2023 22:18:11 GMT  
		Size: 102.7 MB (102690458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4396d5048ec390404bd6a0a391e52bc5b7387f483a104e222167e66c814d9f5f`  
		Last Modified: Tue, 01 Aug 2023 22:19:48 GMT  
		Size: 72.0 MB (72001161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d4456a4d5de143da4b8524f738123940b2cef40e868411a726b9ffd3ec00e8`  
		Last Modified: Tue, 01 Aug 2023 22:19:42 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
