## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:3bc678cff59410673d2e94a8c138d6ad0f7e9b86e05ea7124a7d680c394686a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:3a2e06e62b5baf2f8ecf34012c8e0568a40dd83ad9c6c1c8855bb08fa0ffe55c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317340868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769ae9126b1ee107b675ee5e16d130ba6246c2155d194cf5813e4c1c6f9790a8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:16:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:25:19 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:25:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:25:21 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:25:21 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:25:21 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:25:26 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:25:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:25:26 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:25:44 GMT
RUN boot
# Thu, 23 Mar 2023 06:25:44 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:25:44 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:25:44 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7c7fe7e43e56d1e5e7153ccd41c7b1bf9e8b831af647a69ed9da06d59f2d9b`  
		Last Modified: Thu, 23 Mar 2023 06:34:16 GMT  
		Size: 201.1 MB (201112948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36fd3a8f44222024e49457a4665b13835082498964fafde4fd19033d0b714c0`  
		Last Modified: Thu, 23 Mar 2023 06:34:02 GMT  
		Size: 2.4 MB (2361573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71911946b985a2690af580a40391a90510668be23a9852f6e5bb63da0af26e7`  
		Last Modified: Thu, 23 Mar 2023 06:34:06 GMT  
		Size: 58.8 MB (58820341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdda6129c00b1d55f7045400e92bd3a63a20a97d7698675762108b561c9aa2ec`  
		Last Modified: Thu, 23 Mar 2023 06:34:02 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:75328c46b8285f86617c50f22db247c9a7bc861da9892f476d0eca1b3fc41452
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314730079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:729b1c29e71064ea672fc2570cb0ef9263a6180f3c182c7a8a490a3bcaf47a0a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:59:08 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:59:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:59:13 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:59:13 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:59:13 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:59:18 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:59:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:59:18 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:59:34 GMT
RUN boot
# Thu, 23 Mar 2023 06:59:35 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:59:35 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:59:35 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d0a6a3f6f4458fd84817e257a4ed1795d2fe3740eb80c763937a14d0cf186a`  
		Last Modified: Thu, 23 Mar 2023 07:07:20 GMT  
		Size: 199.9 MB (199855189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d345e4c3a3644e2ccdf22482b735fc7ab3dacb258be6f1043fea6578cc6c7ea`  
		Last Modified: Thu, 23 Mar 2023 07:07:09 GMT  
		Size: 2.4 MB (2350959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd8c3780e0458df4927af2338b9814ce632041356d5de5a560b9a02318014c9`  
		Last Modified: Thu, 23 Mar 2023 07:07:12 GMT  
		Size: 58.8 MB (58820433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec4d0839a55c4fcaa826391b5ee0aa8b76ed712a1fc4de516db3af73d232cd9`  
		Last Modified: Thu, 23 Mar 2023 07:07:09 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
