## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:dadf849ff70e8336a1e41a44519b534891e11368961a64ec2cb1acd4b09f50bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:c1fb3f23969286268d7c91975ee1d8e20cf06624282950c993d7437531f38b4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317332691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8427a0034f31b954f3faf7da97df03b0e356c69b0d8ab7da34af255ca5309293`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 19:50:54 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 08 Nov 2022 19:50:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 19:50:56 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Nov 2022 19:50:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Nov 2022 19:50:56 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 19:51:03 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Nov 2022 19:51:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Nov 2022 19:51:03 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Nov 2022 19:51:22 GMT
RUN boot
# Tue, 08 Nov 2022 19:51:22 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 19:51:22 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 19:51:22 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234d89610b4a16d903abead0c04715b2957b47183fec8ab6f88c4f3538cff68`  
		Last Modified: Tue, 08 Nov 2022 20:00:47 GMT  
		Size: 201.1 MB (201103429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cb5ee206fc26eb73b815485806e272b29b1b9c67c3dff04bfc21558c62db0f`  
		Last Modified: Tue, 08 Nov 2022 20:00:33 GMT  
		Size: 2.4 MB (2362129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e786c61c21663b908ebf3b24a542c516cddc83d8ad2d3659a915545424499a1d`  
		Last Modified: Tue, 08 Nov 2022 20:00:35 GMT  
		Size: 58.8 MB (58820402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1e3b79f3e2356d8787e32aff9f85ecbd24748481302925ff9856423d72686`  
		Last Modified: Tue, 08 Nov 2022 20:00:31 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:34b0822a078c51c1ced7188d232f73a6c1df92af44f3f8a3ae2d86cf55fe7a21
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314739607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7264601d6f5c6e5d289ccccebece408f24aceaa2ca561e7a99f2a9dc4cca64c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 22:41:06 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 08 Nov 2022 22:41:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 22:41:10 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Nov 2022 22:41:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Nov 2022 22:41:11 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 22:41:15 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Nov 2022 22:41:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Nov 2022 22:41:16 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Nov 2022 22:41:37 GMT
RUN boot
# Tue, 08 Nov 2022 22:41:37 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 22:41:37 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 22:41:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92032ad253d7bb165f3b1ac644f2177d86d0bf0dd878bdd484c4c281ba1a1b0a`  
		Last Modified: Tue, 08 Nov 2022 22:49:49 GMT  
		Size: 199.9 MB (199864415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc47dbbbbae7d3e5b4a5db370acd84f8c59a542f7eae6d53a3a8f9daf1adcdf`  
		Last Modified: Tue, 08 Nov 2022 22:49:37 GMT  
		Size: 2.4 MB (2352290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b4ff19660474edbe11b04e22ff3736c6020c93f3425e0bcb00d4c1711176b`  
		Last Modified: Tue, 08 Nov 2022 22:49:40 GMT  
		Size: 58.8 MB (58820534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b165c3c024dc3ce070217f475791cb983a39ee9e40884e3e8af2294167a0b3`  
		Last Modified: Tue, 08 Nov 2022 22:49:37 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
