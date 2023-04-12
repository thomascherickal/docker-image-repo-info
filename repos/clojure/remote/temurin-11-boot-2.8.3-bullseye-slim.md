## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:4f13e5311a295c9e186438beb19f3815af9057509191c5e89be2c4c08d9d2bdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:36e8c44174fc1f86fe96d161a51f8233386fbd061d2c84f439ac230d8f6afa69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289792196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f41c408a3c842fec4c4d176162f8489c58a8320370d67300441873cf31fabf`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:14:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:14:02 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 08:14:02 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:14:02 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:14:08 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 08:14:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:14:08 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 08:14:26 GMT
RUN boot
# Wed, 12 Apr 2023 08:14:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda96c7b8aa69385b19c520aa06ff5d57c687e857e5255da300163c0826a78d4`  
		Last Modified: Wed, 12 Apr 2023 08:23:05 GMT  
		Size: 1.1 MB (1077527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69944937ada57ce29378904fae7caa0b7ad900e8b3397c7f83e279809c7d24c`  
		Last Modified: Wed, 12 Apr 2023 08:23:08 GMT  
		Size: 58.8 MB (58820450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ed525d4fbfe75682c0ddcd0a1849f76ab73efae6117f05f5b3a892fd9db67a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285191745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5fe87a4c9e8adfc7929e2000a98fd292f804f6a71053db52c884de38e0c274`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:21:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:21:14 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 01:21:14 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:21:14 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:21:19 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 01:21:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:21:19 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 01:21:37 GMT
RUN boot
# Wed, 12 Apr 2023 01:21:37 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36f04a3569f1f016be4996ed9b22512641ca30eaa96a16673a3f1d957af9155`  
		Last Modified: Wed, 12 Apr 2023 01:29:32 GMT  
		Size: 1.1 MB (1064795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ddc8af85a3487a9d5b02a56c8596560a0c568fd0beacc6d1c6d69d7b7495fd`  
		Last Modified: Wed, 12 Apr 2023 01:29:35 GMT  
		Size: 58.8 MB (58820590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
