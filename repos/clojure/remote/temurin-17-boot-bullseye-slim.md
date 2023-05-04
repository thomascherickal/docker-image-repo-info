## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:a235d9f6b6f5e6aeaaf39741f8928344059a7b3cdba6eed45ea6bb4bb721684a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a1e1b3fce74ec4447fbbba93ac4731635f3daa582b8ab51d16ed1322586fb003
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.9 MB (283882226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62b72b9bf1a405bad6714709bd7f1a315766d5edbc9a9dc4202cd0b8686c19df`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:59:25 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Thu, 04 May 2023 14:59:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 14:59:27 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 May 2023 14:59:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 14:59:27 GMT
WORKDIR /tmp
# Thu, 04 May 2023 14:59:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 04 May 2023 14:59:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 May 2023 14:59:32 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 May 2023 14:59:49 GMT
RUN boot
# Thu, 04 May 2023 14:59:50 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 04 May 2023 14:59:50 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 04 May 2023 14:59:50 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fd2caa057611d1671449088801d8f3e11973cc523e65f79f2b73f9189938c0`  
		Last Modified: Thu, 04 May 2023 15:09:34 GMT  
		Size: 192.6 MB (192580382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3e76af224bf8e79cc3ac46bc3b03b3e70b41bc2ff18a00837f2fb9b6d40d41`  
		Last Modified: Thu, 04 May 2023 15:09:20 GMT  
		Size: 1.1 MB (1077506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4211d10ce0663d4fe2d030ac1e1c3667f911ab45a11a158f9404ec5a94e558`  
		Last Modified: Thu, 04 May 2023 15:09:23 GMT  
		Size: 58.8 MB (58820425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314acda8720dbb04fe6cfcec9a4de61f7126aa368736eb8772c955f3c06a382a`  
		Last Modified: Thu, 04 May 2023 15:09:20 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:94fb21dbddba7f3cbfe9a9cbb03862d9fe5cc998309b61a3cd89c2ef21456f4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281326107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec8a367b0f1fe1712d24ab69c084d290fedd1509b63c18ae76d7cbcc1934525`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:14:13 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 10:14:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 10:14:17 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 May 2023 10:14:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 10:14:17 GMT
WORKDIR /tmp
# Thu, 04 May 2023 10:14:22 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 04 May 2023 10:14:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 May 2023 10:14:22 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 May 2023 10:14:37 GMT
RUN boot
# Thu, 04 May 2023 10:14:38 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 04 May 2023 10:14:38 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 04 May 2023 10:14:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575b486fb24233a04314b561ec4eeae43d749cd55a8b6194087d505365366b7`  
		Last Modified: Thu, 04 May 2023 10:22:21 GMT  
		Size: 191.4 MB (191387643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82118e695e2ab6932cb4423f866adba98bd75ce916f87e33dc30d18c0fd8b98`  
		Last Modified: Thu, 04 May 2023 10:22:10 GMT  
		Size: 1.1 MB (1064802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc4cbd52fca806ce172019c885da13e571dacddb10cf43987da346deaa7a048`  
		Last Modified: Thu, 04 May 2023 10:22:12 GMT  
		Size: 58.8 MB (58820529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84bf923a1ba2538adab4a06f54bf7acc445fe1aa375b3eef99ddbff35822a9f`  
		Last Modified: Thu, 04 May 2023 10:22:10 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
