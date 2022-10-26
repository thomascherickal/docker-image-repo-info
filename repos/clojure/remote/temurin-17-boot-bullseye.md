## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:519020114b9e7eb6cc4b7df09e12b86b0928cd0a0609672212698723707494c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:206ab170afc3bcbedc9b09f33b1f0cbbdf548869731f455400c7932cb4084619
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.4 MB (308366852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6eb5e84ebdb0ed003fa50029eb2153595154af4efce2e807bf1215ca591a0ac`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:39:23 GMT
COPY dir:09afbf947759009c57336c17f70cd71239c5d8b0170793151aec66483cdd0976 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:39:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:39:24 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:39:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:39:25 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:39:31 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:39:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:39:31 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:39:51 GMT
RUN boot
# Tue, 25 Oct 2022 02:39:51 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 25 Oct 2022 02:39:51 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 25 Oct 2022 02:39:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac76dde2c2f13d28db088f654035acb0c8244b4c9447b8e9b0cfdb280fee3c55`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 192.1 MB (192137591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b634bbf12e96ba68daf84945435fe526a086f43553876baf48e5af3c163acaf6`  
		Last Modified: Tue, 25 Oct 2022 02:51:50 GMT  
		Size: 2.4 MB (2362126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbdd9bb7939290f1b09a202ddc545ea2725af3f38293de94c3a0e947a2502eb`  
		Last Modified: Tue, 25 Oct 2022 02:51:53 GMT  
		Size: 58.8 MB (58820405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bf53b921ad1cc4e71562568ffb4b60e902379b64cf95a468d5fd1c2f917c56`  
		Last Modified: Tue, 25 Oct 2022 02:51:49 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9e2b2311f4a735215c383b24a7a0de15f188f33b740a02514864bb169dc7541f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305779099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24a243950ac617fee291ddd3477247974cc78b7dadcb5907092ec96b2cf141b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:44:50 GMT
COPY dir:580c509aa131da1d31de9db8eed968c1f0ef93ad270f258b0b43d9d7d72bba84 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:44:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:44:54 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:44:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:44:54 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:44:59 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:44:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:44:59 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:45:18 GMT
RUN boot
# Wed, 26 Oct 2022 15:45:18 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 15:45:18 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 15:45:18 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28dae7f1170ef9a47cb310629f09131dfb5a10ce4efd89d8f7e2a1aad189bb61`  
		Last Modified: Wed, 26 Oct 2022 16:01:02 GMT  
		Size: 190.9 MB (190904077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ae30d2c5c9ba379f554152ba155d14a84c249adcef44ea0954c525e69378db`  
		Last Modified: Wed, 26 Oct 2022 16:00:51 GMT  
		Size: 2.4 MB (2352229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5240b2a070d295da9399ff8cf4d00d7a8bbef12835cc3201ac1f86c85d22a4`  
		Last Modified: Wed, 26 Oct 2022 16:00:54 GMT  
		Size: 58.8 MB (58820425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0757cb5d1ebf6793ac5ec1c98315687b4493933103ceb2a68bebb9ffa0035ef`  
		Last Modified: Wed, 26 Oct 2022 16:00:50 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
