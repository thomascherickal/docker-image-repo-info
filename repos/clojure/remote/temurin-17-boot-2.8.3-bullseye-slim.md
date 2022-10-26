## `clojure:temurin-17-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:89c9afc2436bf59f98b2b76490a41904c2225b763ad04cb5c32428cb1f4dea14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:12e16c1aa77bc4a3df1daec11305139cc32a03f498092a970d8cd70e71f2447f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.5 MB (283457324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c73edc58684b47fc09f9edbb89b27cd6cd0e92bd87cc0705830245cf658a9d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:40:02 GMT
COPY dir:09afbf947759009c57336c17f70cd71239c5d8b0170793151aec66483cdd0976 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:40:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:40:03 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:40:04 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:40:04 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:40:09 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:40:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:40:09 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:40:28 GMT
RUN boot
# Tue, 25 Oct 2022 02:40:28 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 25 Oct 2022 02:40:28 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 25 Oct 2022 02:40:28 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83abe3e31fb9e53a1a1e4ee0c8ea2375695563d8ad661be27c808d990fc0da74`  
		Last Modified: Tue, 25 Oct 2022 02:52:28 GMT  
		Size: 192.1 MB (192137443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2c4f70ac16efd5b7dc63dfb05a068f3b2b0d94d0a50ba110408e6b10fabaa`  
		Last Modified: Tue, 25 Oct 2022 02:52:14 GMT  
		Size: 1.1 MB (1078978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbe433518c091e402e17ccde349c77996ba0ba685863b7b57956054d66ffd3b`  
		Last Modified: Tue, 25 Oct 2022 02:52:17 GMT  
		Size: 58.8 MB (58820464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bb29444913c08d12170e7e2145a4f8d62a4f9b95d791c516222e426d551d6b`  
		Last Modified: Tue, 25 Oct 2022 02:52:13 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:21a3be2b144bf61f7585c88cd0c8d71da0c4bf6ae08a51dda40872a4df30b01a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.9 MB (280855152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2fbc73234a0d5c015b45cacf23d9bab218a8957944c3c90d71476902dfbcbfd`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:45:22 GMT
COPY dir:580c509aa131da1d31de9db8eed968c1f0ef93ad270f258b0b43d9d7d72bba84 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:45:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:45:27 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:45:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:45:27 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:45:31 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:45:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:45:32 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:45:48 GMT
RUN boot
# Wed, 26 Oct 2022 15:45:49 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 15:45:49 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 15:45:49 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227b5452ba825facdc158312391c195512969f1ab7a485e56b2a432c2fcf433`  
		Last Modified: Wed, 26 Oct 2022 16:01:26 GMT  
		Size: 190.9 MB (190904076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afeb01f03f79cba2182a0ba0171a49e74856f06fa748f6189f985cbf6320d0d`  
		Last Modified: Wed, 26 Oct 2022 16:01:13 GMT  
		Size: 1.1 MB (1066327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf5db60693257df14b8da660eaec26b7ce78671057bcff86a0f792c663f860f`  
		Last Modified: Wed, 26 Oct 2022 16:01:16 GMT  
		Size: 58.8 MB (58820440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4281ef008ca27e429064da5a5c36da1729ddd7923577022525c612175fcbc8e`  
		Last Modified: Wed, 26 Oct 2022 16:01:13 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
