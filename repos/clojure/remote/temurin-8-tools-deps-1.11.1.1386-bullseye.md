## `clojure:temurin-8-tools-deps-1.11.1.1386-bullseye`

```console
$ docker pull clojure@sha256:509dc0c70ac925c603628c6d1611f0ba0ed068db61857740c8d2428dfc12a649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-tools-deps-1.11.1.1386-bullseye` - linux; amd64

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
