## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:2b61a14211116417232cbc6901a0191db12c38f9adfd70afb350523667b97caf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:211d804b1fd6e0012aeb02b874d7fc37d4a706508e4afaa90ff9093533557dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314661084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bafbb639ea140f2cde8135d9d023cd8025c634dcda210fa17b887e0e95b75d7e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:22:38 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:22:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:22:39 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:22:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:22:40 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:22:46 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:22:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:22:46 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:23:05 GMT
RUN boot
# Wed, 11 Jan 2023 03:23:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9daf555cc2f9363f3a229a8f5a0778aae1c7578c5542c0b8ebda1e59c00a1f`  
		Last Modified: Wed, 11 Jan 2023 03:36:19 GMT  
		Size: 198.5 MB (198454554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556d1be0e8c21111ab60b8becf8835833f780b8fcebf282ca882862d97eb6ca7`  
		Last Modified: Wed, 11 Jan 2023 03:36:04 GMT  
		Size: 2.4 MB (2360719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50991a3e1abc4fe4aab8f36d11363656c9e15ca6ace4f9a2f95ba214eb13d52e`  
		Last Modified: Wed, 11 Jan 2023 03:36:08 GMT  
		Size: 58.8 MB (58820605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1ee5eb1a83d568ede37090f04acc44d30db0b9fced92763eb78813a3ee591799
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310056321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa59739304136f0fac6944dd1133b973e5af4c1e1401c7e583562870881835`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:40:51 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:40:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:40:55 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:40:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:40:55 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:41:00 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:41:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:41:00 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:41:17 GMT
RUN boot
# Wed, 11 Jan 2023 03:41:17 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a71e3b5137ea8b3bc97426de9f949895ebbaf94245a4f79078021dc428df68`  
		Last Modified: Wed, 11 Jan 2023 03:52:32 GMT  
		Size: 195.2 MB (195203370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad3e64da8a74d4405c7f1d88e1fec788a432d4b722f2cedeb296a9b8bf59a91`  
		Last Modified: Wed, 11 Jan 2023 03:52:21 GMT  
		Size: 2.4 MB (2350665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca18951811406f071b8268c29bc4fe856709fd00db3c0c9681546dcf2181ff1c`  
		Last Modified: Wed, 11 Jan 2023 03:52:23 GMT  
		Size: 58.8 MB (58820427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
