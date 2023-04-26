## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:6c7e74294ee3b17f8ac078b759ae88318be73e655ccad8135251621799fe9ab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:1d255638195f196d7b29e2eb622c1ee96ad649fb10302592b332c635ffb916b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289865584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8fcde7671c693215e0418429efd3e7d8c2d3ce9ebc230c780f6026d383c0e79`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:04:09 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:04:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:04:11 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:04:11 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:04:11 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:04:16 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:04:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:04:16 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:04:34 GMT
RUN boot
# Wed, 26 Apr 2023 20:04:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4732512befd268374b48fb0d71e1d7b92ee077512c8190c2a7378323351f7fb`  
		Last Modified: Wed, 26 Apr 2023 20:21:00 GMT  
		Size: 198.5 MB (198549520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26673e206eb87dd67eb7d812af2c81d99b21f112a00c9da789b3a38de139ff`  
		Last Modified: Wed, 26 Apr 2023 20:20:46 GMT  
		Size: 1.1 MB (1077496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14711f38ba35c2366bcd02c934d3d8fd7ea2eb41df9c3a358c2a67a6bc9e106c`  
		Last Modified: Wed, 26 Apr 2023 20:20:49 GMT  
		Size: 58.8 MB (58820340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d5762a36e5c191a3a7ec646e5bf0c686039bb8d3d71bde9328b35fe76023e17d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285273376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82db29012dafa7ddc1d3ac0433608f4d541ed2f49e48f71c32061405a8152b0e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:39:21 GMT
COPY dir:8d5d0106b2c3fe64c4905be44080473b7828ffb48e0e107739a7ba7a3cb627cf in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:39:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:39:25 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:39:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:39:25 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:39:30 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:39:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:39:31 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:39:47 GMT
RUN boot
# Wed, 26 Apr 2023 20:39:47 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0ff727a2ea86bf959fae7a3ea2e76bbb235388265f92315f2f24de6816a635`  
		Last Modified: Wed, 26 Apr 2023 20:53:03 GMT  
		Size: 195.3 MB (195324205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9254492d9551954076023e7db763a2fb669c981004825fb4460274a32b38c605`  
		Last Modified: Wed, 26 Apr 2023 20:52:52 GMT  
		Size: 1.1 MB (1064799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36750e09e52abbe5fcd31817f65b0f7346007c9c962b0e6ac64e67956165479a`  
		Last Modified: Wed, 26 Apr 2023 20:52:55 GMT  
		Size: 58.8 MB (58820546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
