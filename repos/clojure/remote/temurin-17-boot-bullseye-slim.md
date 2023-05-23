## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:0ba40de820a04b0ed84b3c08b851667a5b3a7ca1b20454701aa2d5b8391cfc9a
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
$ docker pull clojure@sha256:170b6200ca2d8f7dd39e81636aacfedaecffd5f85a0db97bcc736d696ec7cd35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281326065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06c9aaed3ffee9598232918416793b5d270b1dfb7ce29c19fcac99533e781e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:29:51 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Tue, 23 May 2023 01:29:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:29:55 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:29:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:29:55 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:29:59 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:30:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:30:00 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:30:16 GMT
RUN boot
# Tue, 23 May 2023 01:30:17 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:30:17 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:30:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04300dd851e66af00281d635f3fa075517249f6b42bf7ebe21fbbe2828ef53bd`  
		Last Modified: Tue, 23 May 2023 01:37:21 GMT  
		Size: 191.4 MB (191387691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26a475f0bd1bc0d41f2e019efe3a7311e5d5b55010eb4121c1d274954899aba`  
		Last Modified: Tue, 23 May 2023 01:37:11 GMT  
		Size: 1.1 MB (1064807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f990a11fd0c5edb68b93f59ea42ed1698d8b08cfd912682a03c54f6f4f30e`  
		Last Modified: Tue, 23 May 2023 01:37:13 GMT  
		Size: 58.8 MB (58820421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c2e108839e3c55feba645877dd055c2864615866ba32bb200efa518b4f25de`  
		Last Modified: Tue, 23 May 2023 01:37:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
