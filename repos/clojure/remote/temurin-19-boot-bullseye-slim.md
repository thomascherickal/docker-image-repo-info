## `clojure:temurin-19-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:6913fa0eb2f07f29066ac423e4b087b5341c90095241933aab76dad325cb5d8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:62cbd3225efce139845c8321b5ef9d56f50c30d254ae0cb6d1da00550a47c8d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292398592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ab397b1b88865d8dbb208077931d75c7deaf4fc036654c2ff55a0df979da5e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:00:06 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:00:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:00:08 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:00:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:00:08 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:00:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:00:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:00:14 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:00:34 GMT
RUN boot
# Wed, 21 Dec 2022 02:00:34 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:00:34 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:00:34 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0058afebbfddb0f61fd316c5a4af96e40c10e846cefe669fe9f41c096818b001`  
		Last Modified: Wed, 21 Dec 2022 02:11:21 GMT  
		Size: 201.1 MB (201103405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d011d879c26ea2bfc634dc2a55ef0216cb97d7d1c4cf36dafee7bc53a4a41cc2`  
		Last Modified: Wed, 21 Dec 2022 02:11:05 GMT  
		Size: 1.1 MB (1077344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b466b5a1f3d4d0709c2115af83385d13da52d4b0beffade500665a9dbf36408d`  
		Last Modified: Wed, 21 Dec 2022 02:11:09 GMT  
		Size: 58.8 MB (58820499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f081ce02955588390c781c59da158f59d1a105b96aaf669058b536ba21ac9f31`  
		Last Modified: Wed, 21 Dec 2022 02:11:05 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c40a93cca9e800233d299637bb292b42741925fe56618a83faea343811a1e1e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289794750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad4366e52c489aba8711cfb2d046694215a26fd1082211db7e5d8aa018f17a5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:26:17 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:26:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:26:21 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:26:21 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:26:21 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:26:26 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:26:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:26:26 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:26:43 GMT
RUN boot
# Wed, 21 Dec 2022 02:26:44 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:26:44 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:26:44 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60207e0d770d0504fd11f154cc640f5bd985f35f0e8a2678ed586914b052fe2`  
		Last Modified: Wed, 21 Dec 2022 02:36:04 GMT  
		Size: 199.9 MB (199864411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20def319271307d8aaab3aedd519f9b4cc764758a74672cf4a82abd197fe46e1`  
		Last Modified: Wed, 21 Dec 2022 02:35:52 GMT  
		Size: 1.1 MB (1064625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70861b0abefda16b283e9b8fff4c3f80417ad0b0482438ca609f1c07e0babf07`  
		Last Modified: Wed, 21 Dec 2022 02:35:54 GMT  
		Size: 58.8 MB (58820542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed6b835705c7c400cb5ebbf59505705b386515aa1f1b46b29d4de3141dfba96`  
		Last Modified: Wed, 21 Dec 2022 02:35:51 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
