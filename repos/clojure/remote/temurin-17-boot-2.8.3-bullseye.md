## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:4280bbd75c398ae5b17c85f83776480f5c00e8bf7bd2b9ba34bf999fe77edac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:850921243aa21b7c6f1d4414b56044d14f35486a1386d1c6b31d86e9f5b8b791
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308638018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:045715de39d3850f8502f510b554471ab7b0c374ec0ec5a36441e1df4c6a7b6a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:56:26 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:56:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:56:28 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:56:28 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:56:28 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:56:34 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:56:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:56:35 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:56:55 GMT
RUN boot
# Wed, 21 Dec 2022 01:56:55 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 01:56:55 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 01:56:55 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85d928f7af45063c8909fd71ef1d2934126eb27a444735b74dc4b9d177542d7`  
		Last Modified: Wed, 21 Dec 2022 02:08:49 GMT  
		Size: 192.4 MB (192431250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f588b942635790516bd71b4d70fad15a0281ad179b86d7289b70116ce039c98`  
		Last Modified: Wed, 21 Dec 2022 02:08:35 GMT  
		Size: 2.4 MB (2360813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc82e4bf9ed1eca1266953e4aa6af02d1e5f4c908412eac66ae5d7cbd431d1e2`  
		Last Modified: Wed, 21 Dec 2022 02:08:38 GMT  
		Size: 58.8 MB (58820389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73299d24d23eecb6218afbacc4d47c350443be9853e9f2e8d9b0f2866307e8cc`  
		Last Modified: Wed, 21 Dec 2022 02:08:34 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:94ce736bec47e989cc026ea6711b749c08eddbdb6f898ac6e315f08e4668bce0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306068510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0939996af11ad0240633375016cf87e7138c6bcd82e79782cccf6f4d417444a8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:23:13 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:23:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:23:17 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:23:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:23:17 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:23:22 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:23:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:23:22 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:23:41 GMT
RUN boot
# Wed, 21 Dec 2022 02:23:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:23:41 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:23:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7590a9cfd73d6147f6887d3e0a5cb84fcb61c48a400fb999741e356bc525b005`  
		Last Modified: Wed, 21 Dec 2022 02:33:56 GMT  
		Size: 191.2 MB (191215202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdea1aea0c772e66f672b8e13e5038beb63c9914943fafad7a6c5d73a5fc753`  
		Last Modified: Wed, 21 Dec 2022 02:33:44 GMT  
		Size: 2.4 MB (2350669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bd9ba9ac1f0cf9f12e187ae1be7d1068c67e992655ee813d21132bc320d2`  
		Last Modified: Wed, 21 Dec 2022 02:33:47 GMT  
		Size: 58.8 MB (58820443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2387f304c62227d29333b32d6bff1010fefe927cad6268755aed051cf8a9e2e4`  
		Last Modified: Wed, 21 Dec 2022 02:33:44 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
