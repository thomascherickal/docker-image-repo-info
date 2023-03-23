## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:0d10137924745b16ab9101585ddf563f1ac0bd9d31717d01039699663ca1f8d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:2107e266fafb06223a9f5beaae095d19dc6c3b28c76d966b373453886ee7295d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145944695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2602fbf90b8c163e52c5adb0121bb452feff0d8d329852d82bf2ed20e61110`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:17:47 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:17:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:17:48 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:17:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:17:48 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:17:53 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:17:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:17:53 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:18:10 GMT
RUN boot
# Thu, 23 Mar 2023 06:18:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977e261c2ece5904696fe62d44f44495568e580f96e10c2adb6f00ef7e609c9`  
		Last Modified: Thu, 23 Mar 2023 06:29:27 GMT  
		Size: 54.6 MB (54635545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e622ad49c17f249d06a9110797d6470803f637fa8202665cc61e330e8f4b94`  
		Last Modified: Thu, 23 Mar 2023 06:29:21 GMT  
		Size: 1.1 MB (1077364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4716835939df2da63cc2dbad9d3c507584040df9606d1fbb7eb806f78d5a9b4d`  
		Last Modified: Thu, 23 Mar 2023 06:29:24 GMT  
		Size: 58.8 MB (58820381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4065ff2c38e4f94226f5ba4a20a0f32ec119fae888ab7d5fc6b66b9352b4ffb9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143675568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2d83b589307c706148059fd61f651a476ff11d785f44d433fe619b88bd102d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:52:40 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:52:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:52:41 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:52:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:52:41 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:52:46 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:52:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:52:46 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:53:02 GMT
RUN boot
# Thu, 23 Mar 2023 06:53:02 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f48d2f27de7b5e53c0560c7b25baf6904fad54afeb5ea0f8dc5d66dd42d6ee`  
		Last Modified: Thu, 23 Mar 2023 07:02:45 GMT  
		Size: 53.7 MB (53727901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62e27847341e65bb4706a03a761649956f22245327aa981c068532c5e9940d`  
		Last Modified: Thu, 23 Mar 2023 07:02:40 GMT  
		Size: 1.1 MB (1064632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73743c06b9c3733dedf79b3966cc656e73d3334982b852cbce4dce33d6b9071d`  
		Last Modified: Thu, 23 Mar 2023 07:02:42 GMT  
		Size: 58.8 MB (58820335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
