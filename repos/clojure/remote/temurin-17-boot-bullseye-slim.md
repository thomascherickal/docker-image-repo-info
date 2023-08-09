## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:1503959c357a9f881beed6f286c49604e0d3c564f8c008055ff9ee79dbd1b58e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:5428121eeabb154bf2c08fb95ef69b84eaca1f606d103977db137001c4788267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236089758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97faaba34e3a7dfb4380b7c80ee47d521b3c152ece77f62a2146d1727e459323`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:17:57 GMT
COPY dir:8ea3eea47bd8b9d37ce2403b2d64b2cdc0fec836a119c10ec3e4ff0bcca8bb4d in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:37:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:37:32 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Aug 2023 22:37:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 22:37:32 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 22:37:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Aug 2023 22:37:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 22:37:37 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Aug 2023 22:37:55 GMT
RUN boot
# Tue, 08 Aug 2023 22:37:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 08 Aug 2023 22:37:56 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Aug 2023 22:37:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8050892377b9a47e9c3a9ef290967338da628f34d31341e0efc181a16a685401`  
		Last Modified: Tue, 08 Aug 2023 20:20:46 GMT  
		Size: 144.8 MB (144773775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4a65c014599ca01d38c645c3f1720ad59fa081eef74712fcbc4bef1e8422a0`  
		Last Modified: Tue, 08 Aug 2023 22:49:41 GMT  
		Size: 1.1 MB (1077534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6d34301b28999ecbeb6968149d67d3b4d6cdb3d97d1b4640868985bfa9d274`  
		Last Modified: Tue, 08 Aug 2023 22:49:45 GMT  
		Size: 58.8 MB (58820447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308fdd146246a792c294fbfdce3d3b893ba45e7d6c940dcd764529cf473233e`  
		Last Modified: Tue, 08 Aug 2023 22:49:40 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:fa8ea5dcc771d0960e0f51902177fca400c777d985a251ea52c07ecb0a2e9eb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.5 MB (233486698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69563954d885bf6feee30e2330b253784ac91e05d37aae1f1681795fab0bbcc0`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:25:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 14:25:26 GMT
COPY dir:ea833e6c6c81bc32cfded5d05d30b781acc802f6c770c2720afc9a9f14f4a7d5 in /opt/java/openjdk 
# Fri, 28 Jul 2023 14:35:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:35:35 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 28 Jul 2023 14:35:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 28 Jul 2023 14:35:35 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 14:35:40 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 28 Jul 2023 14:35:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 28 Jul 2023 14:35:40 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 28 Jul 2023 14:35:59 GMT
RUN boot
# Fri, 28 Jul 2023 14:35:59 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 28 Jul 2023 14:35:59 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Jul 2023 14:35:59 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc8dfc50ad1a93c8652ce31df19291350dca86cc2b7462fbd67c78d39e53aca`  
		Last Modified: Fri, 28 Jul 2023 14:27:39 GMT  
		Size: 143.5 MB (143538104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c46ce4b0b545db2a2d1e4fbab8d22ca721f1b69515cc5ef57b30101e6e0254`  
		Last Modified: Fri, 28 Jul 2023 14:43:20 GMT  
		Size: 1.1 MB (1064842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97c695a299359994c84af5e6e5bbcdcec584db37fb703b30e6a4acd1c0cbf5`  
		Last Modified: Fri, 28 Jul 2023 14:43:23 GMT  
		Size: 58.8 MB (58820521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f5cda9bee94254c7133f24b91598a7e694f182808e58f32adeb4d343518d34`  
		Last Modified: Fri, 28 Jul 2023 14:43:20 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
