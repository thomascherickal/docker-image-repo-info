## `clojure:temurin-11-tools-deps-1.11.1.1386-bullseye`

```console
$ docker pull clojure@sha256:e02d1045a71f034561ade2474ed292554ace0c5cb517c3127539c37fcc2dfb05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-tools-deps-1.11.1.1386-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b9ed21f6d696d547e2e7378f35594addac8d21f422a78715e37ffaa9c4e4f400
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271782478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d275e5f8e54043250a2f83b42ca6712f2e27cc28b0c8d4ccee9d37b7957daa`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 22:29:36 GMT
COPY dir:071e7267c24117f41caea93a03f9d7c7d8dc1c681571e9b8f2b8b433c86f9778 in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:29:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:22:41 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:22:41 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:22:57 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:22:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:22:58 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a4eb0585d7c0fad1a2cb76388ee1ecc94aa2230b3e8084d56c17968d0ef2f`  
		Last Modified: Tue, 08 Aug 2023 22:46:07 GMT  
		Size: 144.8 MB (144831528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabc9b4bbd18d8ae40bed5b9f1a70f2c03b7e9c8775b91a338ee43fb149bbb3f`  
		Last Modified: Mon, 14 Aug 2023 23:30:49 GMT  
		Size: 71.9 MB (71894761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c41c1336cce2fd86521acf15d1f32144b17768d6e035ba05c401b81cd8a2665`  
		Last Modified: Mon, 14 Aug 2023 23:30:42 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
