## `clojure:temurin-17-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:7f4d3db2fd4ec69ee1b39bc497cc81cb885a7c3b4d804d7814adba55de76749a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:9e5fb70e64ee90eb4e77026f5fb0dbbc06389e70faa1cf8fa088d727f8c87bed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285340095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a540f8e30d772e841fde7b0940ab031d0d3332476443d6fa759f3bffc94721`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:41:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 07:08:38 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 16 Mar 2023 07:39:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 20:25:10 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 16 Mar 2023 20:25:10 GMT
WORKDIR /tmp
# Thu, 16 Mar 2023 20:25:26 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 16 Mar 2023 20:25:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 16 Mar 2023 20:25:27 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 16 Mar 2023 20:25:27 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 16 Mar 2023 20:25:27 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6987daa2231f63e24673f500cc33290b31087d360a4da1759adea5436c5f3100`  
		Last Modified: Thu, 16 Mar 2023 07:10:38 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649070e54b44fe81b6f0562aa579df201ff0e43d8d49e944fe58e4d3f5df9e3a`  
		Last Modified: Thu, 16 Mar 2023 20:35:37 GMT  
		Size: 61.5 MB (61489410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a48c7931c1eb6209283f1f6430b077273f4f57bdf14018824d382da899c0bc`  
		Last Modified: Thu, 16 Mar 2023 20:35:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea793f3b38632e42709ee9540bd3c1946b3e7b7b8bbba417784f7b5545ac99`  
		Last Modified: Thu, 16 Mar 2023 20:35:29 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:01b2c961affb2c8ea2fe26a4b670bccc162703def8e64261a2ef70724bba1c32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282928955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8131ff57a71a9a95bc1bcfbefc5fb0620ed3c9390ef3f0130f64bde24705d28e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 04:54:34 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 16 Mar 2023 04:54:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 19:44:05 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 16 Mar 2023 19:44:05 GMT
WORKDIR /tmp
# Thu, 16 Mar 2023 19:44:19 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 16 Mar 2023 19:44:19 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 16 Mar 2023 19:44:19 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 16 Mar 2023 19:44:19 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 16 Mar 2023 19:44:19 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fd3d2fa5647f50c6abfaf315449074732a3ae4821d578ce315c4827bc6417a`  
		Last Modified: Thu, 16 Mar 2023 05:08:08 GMT  
		Size: 191.3 MB (191260401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78163b38552664c6a80b62647ac06ace7665ef5346057c0b493b87f95ef1c25a`  
		Last Modified: Thu, 16 Mar 2023 19:52:20 GMT  
		Size: 61.6 MB (61604722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6cd5f700a4b18722ea10f1865661e07391cc8a3142147bd25de7fcbbdfe2fc`  
		Last Modified: Thu, 16 Mar 2023 19:52:14 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b07d5d53db3bf80fe0eea4268f87bd5c121bc2e445a3df6a4b1cf922e4e40f1`  
		Last Modified: Thu, 16 Mar 2023 19:52:14 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
