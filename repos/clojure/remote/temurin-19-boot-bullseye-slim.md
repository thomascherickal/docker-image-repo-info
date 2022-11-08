## `clojure:temurin-19-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:746d934b7fc0f0017f0e98b83ff72d47dd0fec8c82ba40eb4ff4f2c428a9f088
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:897ae5abcaf0331497e02f70fffc6eb80e8ba2ee05ddc0ac51030b1b04c87abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292423352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14de5744a5c3e0fe42c4025b6c5962a060d6a8ca6d147eb071e9240951f50d7a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 19:51:27 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 08 Nov 2022 19:51:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 19:51:29 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Nov 2022 19:51:29 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Nov 2022 19:51:29 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 19:51:35 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Nov 2022 19:51:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Nov 2022 19:51:35 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Nov 2022 19:51:54 GMT
RUN boot
# Tue, 08 Nov 2022 19:51:55 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 19:51:55 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 19:51:55 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10a8a6939ae868ebbacdafba32bb072252658a353d99bfac452b469d292956a`  
		Last Modified: Tue, 08 Nov 2022 20:01:13 GMT  
		Size: 201.1 MB (201103390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d50d4b09c9b03c0185a3a4ee50c7fb5d2fac9aae43d1a33a8a33433a9d6789`  
		Last Modified: Tue, 08 Nov 2022 20:00:58 GMT  
		Size: 1.1 MB (1078995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb1940368efa86defb95e9fe4e828e61659cd7b40d4a70ccc0d7484b38acd3a`  
		Last Modified: Tue, 08 Nov 2022 20:01:01 GMT  
		Size: 58.8 MB (58820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6b12b88280a01e6462e8e2b4e7b204027c51c2ea281926ed573ec2b81dd85d`  
		Last Modified: Tue, 08 Nov 2022 20:00:58 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0c731fb51243acd80bd79b0f1103468db5b32948622c45a723990397802b2e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289815568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bbe676e7afff5b1fc81d1375529e0dc1d455dc06f30ec6c7419090acdd0da07`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 22:41:45 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 08 Nov 2022 22:41:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 22:41:49 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Nov 2022 22:41:49 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Nov 2022 22:41:49 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 22:41:54 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Nov 2022 22:41:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Nov 2022 22:41:54 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Nov 2022 22:42:10 GMT
RUN boot
# Tue, 08 Nov 2022 22:42:11 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 22:42:11 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 22:42:11 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87dade7855f65c2325e4aad477888abaabf5a2aa0888be9bbb8d5e0445df5ec`  
		Last Modified: Tue, 08 Nov 2022 22:50:12 GMT  
		Size: 199.9 MB (199864415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ba0cfe43250c096938811c4964b5d9c3ef2bca6f7d86506cef02cdbc029fd3`  
		Last Modified: Tue, 08 Nov 2022 22:50:00 GMT  
		Size: 1.1 MB (1066346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb02d790826298b209c9f2fcf334f7dac4126b125edbe8058320ffbcc49fe55`  
		Last Modified: Tue, 08 Nov 2022 22:50:03 GMT  
		Size: 58.8 MB (58820496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018d588bef3280fd7681157f36a96f78a2d66e56017e6c493c737ec05085e16`  
		Last Modified: Tue, 08 Nov 2022 22:49:59 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
