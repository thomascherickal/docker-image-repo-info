## `clojure:temurin-8-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:bd4cd4e0e12aa3898bdb042bf0899e820a816da9b0d08a9967b8f6618baddba9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:83096f2e619b9b233627e1bf4c8ce17e2116cb9f6f4756690c999589c6b1db45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.0 MB (145958136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c49de0a9dc91a88342cd973a6510a25185e3477142a0d4c69856d74687697e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 19:58:51 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Wed, 26 Apr 2023 19:58:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 19:58:51 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 19:58:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 19:58:52 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 19:58:57 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 19:58:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 19:58:57 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 19:59:15 GMT
RUN boot
# Wed, 26 Apr 2023 19:59:15 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773126247f89efdc56db7f90c92282e6c501ad8da6e738413eb8294ca8f168d`  
		Last Modified: Wed, 26 Apr 2023 20:17:34 GMT  
		Size: 54.6 MB (54642132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767d43556fb1915c3295794a4aeab3b5fd5642dbbbc0657159bbfdc80e120205`  
		Last Modified: Wed, 26 Apr 2023 20:17:28 GMT  
		Size: 1.1 MB (1077511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941cab73c0cb601fe020e20f894f1924c7cf0f26b5596773531bd8db1580e27c`  
		Last Modified: Wed, 26 Apr 2023 20:17:31 GMT  
		Size: 58.8 MB (58820265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:60600117cefeec1f8e107b8ec7df9cec5e9887f68e69130c6954d875573e2a6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143691896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cfacfc46c76b2e7a2a3a00267c6fb0fefcc56b5fb12522bfb2d34dff30a4dc0`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:34:51 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:34:53 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:34:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:34:53 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:34:58 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:34:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:34:58 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:35:16 GMT
RUN boot
# Wed, 26 Apr 2023 20:35:16 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db5665283ff0e51d56564a018fb3ca2c344adab4894fcf4b3be9579890aa03`  
		Last Modified: Wed, 26 Apr 2023 20:50:17 GMT  
		Size: 53.7 MB (53742682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489506d5ce76d1ca4d40f63c5f98fb8158cf71c9920c818fd5fb374f74ccfa40`  
		Last Modified: Wed, 26 Apr 2023 20:50:12 GMT  
		Size: 1.1 MB (1064834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2ab1e15d409f2b6a36e74972e10c74a14cfdb19ea2d2810ad18a3b7403e05a`  
		Last Modified: Wed, 26 Apr 2023 20:50:15 GMT  
		Size: 58.8 MB (58820554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
