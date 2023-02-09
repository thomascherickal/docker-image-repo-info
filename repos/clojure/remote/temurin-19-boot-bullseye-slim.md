## `clojure:temurin-19-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:e8a2f3b4115a85807fdd58695464330a39d024cccee97e372235d283ee2cc25d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:c735e3419d0388e8040308a1a9adfde2ae0c37f2a3462463fea21d9cacd6659d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292423015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcbbfde44a246ac5da9d47aeeac4e00093597e4e01b258af1d1350859c4bea49`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:31:41 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:31:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:31:43 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:31:43 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:31:43 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:31:49 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:31:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:31:49 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:32:06 GMT
RUN boot
# Thu, 09 Feb 2023 09:32:07 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:32:07 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:32:07 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4864f8db9c8a9f2cc75ddf386c4ed7fdb7fd8a6d6a8e917a1fefd0d654a89ada`  
		Last Modified: Thu, 09 Feb 2023 09:42:47 GMT  
		Size: 201.1 MB (201112993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9ed75144e162603904a4db6fa6e661f6ee84616bc66ab86bd06c51072eaced`  
		Last Modified: Thu, 09 Feb 2023 09:42:32 GMT  
		Size: 1.1 MB (1077357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69457bdc975b28256668cfb062646c8c3168fd290684b5a239ebc0639239a3a`  
		Last Modified: Thu, 09 Feb 2023 09:42:35 GMT  
		Size: 58.8 MB (58820454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae893ac2a26a444a1d41f85d96277add09779b62df0a361b6b438210f8d75ee6`  
		Last Modified: Thu, 09 Feb 2023 09:42:31 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:bec86f4cac329453082f8b36d9f7e0b87a25cdc35a5a5862a57bc2190aece1ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289802968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0390c3c1eb1a4fbfbd761003504f13cb91e8f4444bc5946548d1e0afd52c68`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:26:28 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:26:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:26:32 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:26:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:26:32 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:26:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:26:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:26:37 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:26:52 GMT
RUN boot
# Thu, 09 Feb 2023 09:26:52 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:26:52 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:26:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88b0545c043fbdf4b8f9e944c5439147e4d7ceb092637c3f142d7ec06d0749`  
		Last Modified: Thu, 09 Feb 2023 09:36:23 GMT  
		Size: 199.9 MB (199855198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f71aa2c6f1852220a6c46cf451c556eeabdbd6d32809823bc944e05a2be92d4`  
		Last Modified: Thu, 09 Feb 2023 09:36:09 GMT  
		Size: 1.1 MB (1064588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746c37ad39cf88ff319f678d5c800193aefcd1bc0697556e9b9d89ec50ae349d`  
		Last Modified: Thu, 09 Feb 2023 09:36:12 GMT  
		Size: 58.8 MB (58820273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cabddedd0a374af725ba42f3d68fd02d6934e69e55635c44607f5c7338654cd`  
		Last Modified: Thu, 09 Feb 2023 09:36:09 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
