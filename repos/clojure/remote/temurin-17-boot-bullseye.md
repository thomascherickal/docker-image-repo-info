## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:37d7b3822ade2fe58c85ac538d71aebb6923606cb84860bb9b23b61a9fd44c8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:84534afbbf118219020de12fe3434bd7ea3b1a23a5e65df1a60eaff2a1911b9b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261013462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4786271a976c63ebfcf0ad7c36ba21f434e33fb7574244bdd5e44df96c0f9a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:32:30 GMT
COPY dir:8ea3eea47bd8b9d37ce2403b2d64b2cdc0fec836a119c10ec3e4ff0bcca8bb4d in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:32:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 01:32:31 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 01:32:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 01:32:32 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 01:32:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 01:32:38 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 01:32:56 GMT
RUN boot
# Wed, 16 Aug 2023 01:32:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 16 Aug 2023 01:32:56 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 16 Aug 2023 01:32:57 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc7280fdeaffb4052a634fa388f698b684cf1d81982342365cecfdca4b0946`  
		Last Modified: Wed, 16 Aug 2023 01:42:29 GMT  
		Size: 144.8 MB (144773775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c12c2d610e59e459804a0d8fd93c103088ab27d311200e9da3b1ddd90216a7`  
		Last Modified: Wed, 16 Aug 2023 01:42:18 GMT  
		Size: 2.4 MB (2362162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ab42af830a5408fd646d7738c441c32ba2ab2d356ef954873281facdaf8d87`  
		Last Modified: Wed, 16 Aug 2023 01:42:21 GMT  
		Size: 58.8 MB (58820504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83d5bc529e86107646c8d7b8516bb35122b38e5267d32994357e2fff8a8b993`  
		Last Modified: Wed, 16 Aug 2023 01:42:17 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0bfe62c6c52706867c6a0e46fc98c682736e409634b60f27f2937be2c6f7de15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258415268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a048a7b183f0aaf952d98c76ac24b6d706f8d7ce3e947e8eb3286d8e97a8a1db`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:20 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:25:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:25:24 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 17:25:24 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 17:25:24 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 17:25:29 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 17:25:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 17:25:29 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 17:25:46 GMT
RUN boot
# Wed, 16 Aug 2023 17:25:46 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 16 Aug 2023 17:25:47 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 16 Aug 2023 17:25:47 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407f1b0394be128a63af2359d89c3282164b67cd2fac29716c6f2f5e348ec07a`  
		Last Modified: Wed, 16 Aug 2023 17:34:01 GMT  
		Size: 143.5 MB (143538089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34182b71af18636282320505be3e3a3c8c1c354c995613212e4c8ed93f2b5c28`  
		Last Modified: Wed, 16 Aug 2023 17:33:51 GMT  
		Size: 2.4 MB (2351416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5548432b5120e8d40e85d209d5cd022dfa3af54d333b41e6470a87c8558b1c1`  
		Last Modified: Wed, 16 Aug 2023 17:33:54 GMT  
		Size: 58.8 MB (58820583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80fe62f299714184c58674ec1c97dd892bef68413b7792bb93fcac6b3460c0`  
		Last Modified: Wed, 16 Aug 2023 17:33:51 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
