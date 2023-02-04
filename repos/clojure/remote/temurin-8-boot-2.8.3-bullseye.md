## `clojure:temurin-8-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:1281eced2204d987dd3b127e8e5ea5e895a79154a4a491ba164c137ccca8cfaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b42ff8272495efa6d060c5005109a4a3b123e65f49ef3a05d82eaea4691aed95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170842270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39bf758eb8981b25d13d43f88b3a17475e9e1bc96e6ef0f32cbe89c9d226fd96`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:05:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:05:28 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:05:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:05:29 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 04 Feb 2023 14:05:29 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 04 Feb 2023 14:05:29 GMT
WORKDIR /tmp
# Sat, 04 Feb 2023 14:05:35 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 04 Feb 2023 14:05:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Feb 2023 14:05:35 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 04 Feb 2023 14:06:03 GMT
RUN boot
# Sat, 04 Feb 2023 14:06:03 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed6af97ccf16f95286359a7baad8fc2394e5c5fdeb6b0e3d4faa3a9509aa270`  
		Last Modified: Sat, 04 Feb 2023 14:20:01 GMT  
		Size: 54.6 MB (54635589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e5356942665d9527802bac3fb85d706fc46268d209808b068c39a8b0066ef9`  
		Last Modified: Sat, 04 Feb 2023 14:19:55 GMT  
		Size: 2.4 MB (2360701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0589837ebbe5faab215cbcfcaaa7ff2340ac36cc31cb6c960af126af861a32b`  
		Last Modified: Sat, 04 Feb 2023 14:19:58 GMT  
		Size: 58.8 MB (58820668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:48c4580bf9f8c0f5444c5cf6f4e7417d6d061e215feb28bd41a592c4c6f2f0d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168580680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f02e148190be48258a1feb1e37cc1fa6c416a8ea902f02f036b6d815705e7f4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 20:00:30 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Wed, 25 Jan 2023 20:00:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 20:00:32 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 20:00:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 20:00:32 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 20:00:37 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 20:00:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 20:00:37 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 20:00:53 GMT
RUN boot
# Wed, 25 Jan 2023 20:00:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e357c132a845a5b6431eb56a9c21fe41d8d90eb03c92e2ff21aed32387f927e2`  
		Last Modified: Wed, 25 Jan 2023 20:12:49 GMT  
		Size: 53.7 MB (53727905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbbccbb5e10f8d0d5ea64a387eb18e0b185a1656f210e32f8882506ffbe6549`  
		Last Modified: Wed, 25 Jan 2023 20:12:44 GMT  
		Size: 2.4 MB (2350654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368299cde10e90f0245f3b4261f368ad7be19271021bbbbb07ff50835cbef057`  
		Last Modified: Wed, 25 Jan 2023 20:12:47 GMT  
		Size: 58.8 MB (58820262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
