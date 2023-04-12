## `clojure:temurin-8-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:1653d7db8949ef51d6628079148e4b8e9228340fc7767ac91e764ef0b9414640
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0f435ef3e7133d4b80a5e6924bdb0926ff1f5c1c463018fd3fe1a6e4267984f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.0 MB (145951913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5062deee2ea9bfa61ed98e81c668fba78ce22c0a3f04072696cbb60320f74448`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:11:18 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:11:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:11:19 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 08:11:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:11:19 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:11:25 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 08:11:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:11:25 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 08:11:43 GMT
RUN boot
# Wed, 12 Apr 2023 08:11:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f4a27a9e344c488df290d18697fb80bdb4bc2f7e4f2e7cb55c5f8b8c5b416b`  
		Last Modified: Wed, 12 Apr 2023 08:21:40 GMT  
		Size: 54.6 MB (54635556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad219b7bdb4f482d4d87f154d268737df393922bc1e8f54809b59bab6f0d3c3`  
		Last Modified: Wed, 12 Apr 2023 08:21:34 GMT  
		Size: 1.1 MB (1077518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e1697196bb44933bf715e9eb101c8d3573086c571658847a8b7a09463a760d`  
		Last Modified: Wed, 12 Apr 2023 08:21:38 GMT  
		Size: 58.8 MB (58820611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1a1bf737367813f1d9f9f5baeef5c66fadde262a8d2aa459a6fe03aa83ed5423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143677037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d68ac35f45fcbfda9ccc455703fc0bc1e26a065d58752da3b7d1fb9099255`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:18:46 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:18:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:18:47 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 01:18:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:18:47 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:18:52 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 01:18:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:18:52 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 01:19:10 GMT
RUN boot
# Wed, 12 Apr 2023 01:19:10 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beeaea1bb320b3b40a83a6b31783cdc7af5081dd6683ffd28ef3a3b39f888ff`  
		Last Modified: Wed, 12 Apr 2023 01:28:11 GMT  
		Size: 53.7 MB (53727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57a2837a2cc9f72adbfdb72e848b55988e5f4380c77ceeba4af44829069d826`  
		Last Modified: Wed, 12 Apr 2023 01:28:06 GMT  
		Size: 1.1 MB (1064821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d84987be50e9054eb5252b00f4316d0920448752d31acd03040424ca40f000`  
		Last Modified: Wed, 12 Apr 2023 01:28:08 GMT  
		Size: 58.8 MB (58820453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
