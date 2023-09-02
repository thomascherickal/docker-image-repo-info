## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:86701b6911cf0d831b0b00895ab3d7231bca3216f7461df0ef25fb057f7da6d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:bd133cfa377a0791411c7dff8535ad5143c796f7cc93e9242f9ea3355f01f12f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261015590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d889591ce85256fdcb7f8f8e9dad4838bfa7a3625da381d5a36ab50ab45904`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 23:31:16 GMT
COPY dir:6777d1f77166c2ecdd8f4eb23f5fd82574aa8a90fd65d6dff981fbb31778a3d1 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:31:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:31:17 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 31 Aug 2023 23:31:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 31 Aug 2023 23:31:17 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:31:23 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 31 Aug 2023 23:31:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 31 Aug 2023 23:31:23 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 31 Aug 2023 23:31:41 GMT
RUN boot
# Thu, 31 Aug 2023 23:31:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 31 Aug 2023 23:31:41 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 31 Aug 2023 23:31:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a114598ad33aed6a505f38365243af34f1e10fad82e78b36362b08851483a7`  
		Last Modified: Thu, 31 Aug 2023 23:44:21 GMT  
		Size: 144.8 MB (144775748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715cb421444410c31f0c42e3cf21fd92c3381c09ec1afa2790bf63faf3b1cd`  
		Last Modified: Thu, 31 Aug 2023 23:44:10 GMT  
		Size: 2.4 MB (2362207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4331089cab2914766b2430cf8f07bd611197057be1c863a3ba421e81680a1ff6`  
		Last Modified: Thu, 31 Aug 2023 23:44:14 GMT  
		Size: 58.8 MB (58820614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa81219bfb57035f4fc6eef00a1ea786241c4d544a8b242fdfb974bb38d69221`  
		Last Modified: Thu, 31 Aug 2023 23:44:09 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:395d27762fff1dbac7296025de49316e47b00fef1ab7951aaa982f70deb631c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258420749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d043e872f4994ec1339f1e9f8578ee8b8a582c96069c49b3cc82d41102aad67d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:47:28 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:47:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:47:31 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Sep 2023 01:47:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Sep 2023 01:47:31 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:47:36 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Sep 2023 01:47:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Sep 2023 01:47:36 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Sep 2023 01:47:52 GMT
RUN boot
# Sat, 02 Sep 2023 01:47:53 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 02 Sep 2023 01:47:53 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Sep 2023 01:47:53 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c782a1c2165dbdac384abd088ebc99d9f013b55fa39e22661861b6b10083b60`  
		Last Modified: Sat, 02 Sep 2023 01:55:28 GMT  
		Size: 143.5 MB (143543490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48927940444fbc331a2f2d983631e5a7e0711e10cf083e07a5a5586539b2609b`  
		Last Modified: Sat, 02 Sep 2023 01:55:19 GMT  
		Size: 2.4 MB (2351444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e483f1cf05ff1e280ec4615803f92f6654889dc21b06f35ce9efdce0c2302098`  
		Last Modified: Sat, 02 Sep 2023 01:55:22 GMT  
		Size: 58.8 MB (58820637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e553780940c0c73ac4e2c1ea1e108193ffa056d918ae285f3c28288464f188`  
		Last Modified: Sat, 02 Sep 2023 01:55:19 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
