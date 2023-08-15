## `clojure:temurin-20-tools-deps-1.11.1.1386-bullseye`

```console
$ docker pull clojure@sha256:b4a321737df9562d7113594d4cade35c480c8619ed31a75144df10308f704938
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-20-tools-deps-1.11.1.1386-bullseye` - linux; amd64

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
