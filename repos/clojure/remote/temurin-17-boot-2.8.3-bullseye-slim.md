## `clojure:temurin-17-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:017045cee6bd2507350faec95f721dff75f0a3163234897cd49fb2d0b8beaeb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a345ab29166a5c5add76fb216111415ed86821186c177cf26bb6be45d2592a57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283748130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b66b0a921368732e0981678e1ea88430d91bf163e56bd35998a623051d26daf`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:28:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:28:41 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:28:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:28:41 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:28:46 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:28:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:28:46 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:29:04 GMT
RUN boot
# Thu, 09 Feb 2023 09:29:04 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:29:04 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:29:04 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b05bab1b9ba30681ad47120bffd01bb1d2b56b4564173f929a1b09b1530f9b6`  
		Last Modified: Thu, 09 Feb 2023 09:40:26 GMT  
		Size: 1.1 MB (1077346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b743d0fa3de07875198f7a3a0b0e14403920c356a4971f83ff5c8271e504d1`  
		Last Modified: Thu, 09 Feb 2023 09:40:29 GMT  
		Size: 58.8 MB (58820384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832a62b8bad23e713d2a654a7ad60be209722563b8a0386cbfeb89a476d2127b`  
		Last Modified: Thu, 09 Feb 2023 09:40:26 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:99802056893697924700398685956bd1d922a14b8a0e4a43de7e59c9f4c2d8fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281208429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb8b738d858918c3e0fced807c79ed6e0cca3030e90fdc1c1cf698fd826b21c9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:24:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:24:03 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:24:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:24:03 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:24:08 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:24:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:24:08 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:24:23 GMT
RUN boot
# Thu, 09 Feb 2023 09:24:24 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:24:24 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:24:24 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83305f4fffe415f1db210ab50c8b2d940aeca9a6b9a2b46d63c3034fd8369cb3`  
		Last Modified: Thu, 09 Feb 2023 09:34:14 GMT  
		Size: 1.1 MB (1064590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46620065f3268310d26460d8f060c4f1fe4c49d10f3084ccb6898d68cac5cf9b`  
		Last Modified: Thu, 09 Feb 2023 09:34:17 GMT  
		Size: 58.8 MB (58820502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195b0d5f7693484afacc3521398c704afa8ab5e80c64f315523234eef01b7afd`  
		Last Modified: Thu, 09 Feb 2023 09:34:14 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
