## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:cec0ffc8f5f3845e52f2efceb6b32da9c1a2a2d5a9fb54731dd901e2769b2706
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:08d46fd54c8fb485acee2d1ffd959455881c24da681c6e85fac43e38b0c6bf76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308655531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976c20891c0409dd5311433522741ad38d0913447a8c9e821348c71913789f2b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:54:43 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:54:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:54:45 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:54:45 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:54:45 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:54:51 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:54:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:54:51 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:55:10 GMT
RUN boot
# Tue, 06 Dec 2022 01:55:10 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:55:10 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:55:10 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c44c11d030ccad72929755f22eeb76adeb4e273253c295bb22aa0cd941361f3`  
		Last Modified: Tue, 06 Dec 2022 02:06:58 GMT  
		Size: 192.4 MB (192431239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d7d1bced7b293214c349bbb1971d08549a0eb653466dab9b4434567179235`  
		Last Modified: Tue, 06 Dec 2022 02:06:44 GMT  
		Size: 2.4 MB (2361961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3398294e7e9e4f3a24fa784024530cf0e5ea35229eebb093d85bf2d61be22f7`  
		Last Modified: Tue, 06 Dec 2022 02:06:48 GMT  
		Size: 58.8 MB (58820590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05982ee7f945a411ff307c36caadfcfe9957b5ca68e30ef26afbd28e1fa4997a`  
		Last Modified: Tue, 06 Dec 2022 02:06:43 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cc1e08844008faceea6cd83ca9f344d7ceb370c1a174d991a5481b46f88a5538
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306088222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6d900da21e3d9af2ec4b0f9b11428a7706e9ce1eaab1f7a2e938ca9c8e3100`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:48:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 15 Nov 2022 05:54:01 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Tue, 15 Nov 2022 05:54:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 05:54:05 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 15 Nov 2022 05:54:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 15 Nov 2022 05:54:05 GMT
WORKDIR /tmp
# Tue, 15 Nov 2022 05:54:10 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 15 Nov 2022 05:54:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 15 Nov 2022 05:54:10 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 15 Nov 2022 05:54:27 GMT
RUN boot
# Tue, 15 Nov 2022 05:54:28 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 15 Nov 2022 05:54:28 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 15 Nov 2022 05:54:28 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee604ee1c814449c1e8223fcbca2cf78c6ba906a0de869dc5ae852d237e22604`  
		Last Modified: Tue, 15 Nov 2022 06:04:50 GMT  
		Size: 191.2 MB (191215218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039f1d577246462e461a235787c393f1c378a61f37f505632ce33cb8c612f982`  
		Last Modified: Tue, 15 Nov 2022 06:04:39 GMT  
		Size: 2.4 MB (2352200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eba7a89179cb7f9c0684af2e2c130e0f32262253510e1fe193574d2e81190e`  
		Last Modified: Tue, 15 Nov 2022 06:04:42 GMT  
		Size: 58.8 MB (58820542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb11aed458b4d88cbb9eb5cc01b9331794d7dfc45d7c91e672b8701b1c9fa9b`  
		Last Modified: Tue, 15 Nov 2022 06:04:38 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
