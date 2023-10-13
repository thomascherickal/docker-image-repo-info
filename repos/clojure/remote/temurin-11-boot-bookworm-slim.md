## `clojure:temurin-11-boot-bookworm-slim`

```console
$ docker pull clojure@sha256:2a70567feac1cd8579b7b9e730c1cbe0f1032d9050fb156fcebbbbf668285768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:13c9f86e56b74cd44559a83989b839d3bf5c1dd2e9cd913f5a717d0145fd1aa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.3 MB (236298017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b94647f95304d4cfba280bb04ca0c1069a5b776b15e2e9bfd7e3f351e4b6ffee`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:28:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:44:27 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:44:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:44:28 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 13 Oct 2023 12:44:28 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 12:44:28 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:44:34 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 12:44:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 12:44:35 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 13 Oct 2023 12:44:53 GMT
RUN boot
# Fri, 13 Oct 2023 12:44:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58d686df0429bc899b9ad25527714341a548bd057ccf4c6c39ca10ffcf2b6a5`  
		Last Modified: Fri, 13 Oct 2023 13:05:13 GMT  
		Size: 144.8 MB (144826195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659abc8766417ac16174fff89ac5abf6ed42a25b8dda006b05ecf39398c1424a`  
		Last Modified: Fri, 13 Oct 2023 13:05:01 GMT  
		Size: 3.5 MB (3501439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85f967c4e80870ac20e5d1e759ec680017b8b333f8e12095c4ef39017eb0d10`  
		Last Modified: Fri, 13 Oct 2023 13:05:07 GMT  
		Size: 58.8 MB (58820509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c176a162994140cc3aea3a775118a2249b6acc6bcca980b3daebca2b1a9ff74d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232895425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79c094a6b2e81694d94493baf56d3f7528a1d0decf007e7361164385149729e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 00:59:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:12:35 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:12:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:12:38 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 13 Oct 2023 10:12:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 10:12:38 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:12:44 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 10:12:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 10:12:44 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 13 Oct 2023 10:13:00 GMT
RUN boot
# Fri, 13 Oct 2023 10:13:00 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7aa7d3902d954c470f86fe2b38acaf6172ca287d14a276c679a36a75e4824`  
		Last Modified: Fri, 13 Oct 2023 10:29:43 GMT  
		Size: 141.6 MB (141570614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef433121823e89ce82a0c156e8cfdf6614332d432f7e506af977e6e8252b0ec`  
		Last Modified: Fri, 13 Oct 2023 10:29:34 GMT  
		Size: 3.3 MB (3325234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2495e3abb88294236d2f859cbc190fd25636b2458b7471714ab20a81fcc581f4`  
		Last Modified: Fri, 13 Oct 2023 10:29:38 GMT  
		Size: 58.8 MB (58820293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
