## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:9c16385003fc69bf38e1f06b2a05c16dc7d284ed5283442f4fdfe5eeb23bd223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:c502554ec0a328077499efb519b2ed1743ad516b37f49d2e5edbebeb4da6fa4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317310283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bc4dd35efe224fd438de2dcbbc9750a44e4256e70866387e899c2b92fbaad2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:28:45 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:28:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:28:47 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:28:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:28:47 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:28:53 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:28:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:28:53 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:29:14 GMT
RUN boot
# Wed, 11 Jan 2023 03:29:15 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:29:15 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:29:15 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4098b1c8c484b772797e0f47e372b00d98eca8d709362a704bbcfe078971a4`  
		Last Modified: Wed, 11 Jan 2023 03:40:21 GMT  
		Size: 201.1 MB (201103372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a0c579aa257123426656ed07a9d9ef3e9f472663cdcbed07cd0f22b58bcf7`  
		Last Modified: Wed, 11 Jan 2023 03:40:06 GMT  
		Size: 2.4 MB (2360761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec949344c2cae609c495ea79692806339d731247c745a41a69d37030fc53c73`  
		Last Modified: Wed, 11 Jan 2023 03:40:10 GMT  
		Size: 58.8 MB (58820544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e0a0d756422122de6fe4fa0151fddb80bb3d56c783d9de5144c075b66f15c6`  
		Last Modified: Wed, 11 Jan 2023 03:40:06 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:138956b90d9c62be59f790d1401795d27fb8cc7ef27d5bd724b03ca9da899723
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314717713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc90d73fca26d7810e669f2b2eb1477d4b9b5014b1df3d4cb45dc5197253f8cf`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:45:54 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:45:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:45:59 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:45:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:45:59 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:46:04 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:46:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:46:04 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:46:20 GMT
RUN boot
# Wed, 11 Jan 2023 03:46:21 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:46:21 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:46:21 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772f0e37f556b3ef1a18a30aff7106c88d94b6e9d9a1ac12a245942bb7995b5`  
		Last Modified: Wed, 11 Jan 2023 03:56:03 GMT  
		Size: 199.9 MB (199864459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9be1c00689cc1102bc962469dc9cd58c2c18765434c23e899c5e179189dc4e`  
		Last Modified: Wed, 11 Jan 2023 03:55:51 GMT  
		Size: 2.4 MB (2350633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43366f9ffc9929404f220e570a86b138cf9ee5049462336742315f36149c412`  
		Last Modified: Wed, 11 Jan 2023 03:55:54 GMT  
		Size: 58.8 MB (58820362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ccb9b184f0e50aa79a1843247b8b2ee0b2d8de0c34d920f51cc58e11c2514`  
		Last Modified: Wed, 11 Jan 2023 03:55:51 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
