## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:a7573e0c35078437b15275f7877e03d00bb385e12f55801a5d1515fa474231ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4c7d79c1a4ddccc433acc699d8ee007c0f66b6f4e190e51aac9ba356f39757b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317073031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d893f7e063437e883f10288804a270b6b0a399053b8ca47d3dd2592cc4b8a76`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:42:31 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:42:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:42:33 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:42:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:42:33 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:42:40 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:42:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:42:40 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:42:57 GMT
RUN boot
# Tue, 25 Oct 2022 02:42:58 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 25 Oct 2022 02:42:58 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 25 Oct 2022 02:42:58 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b6cdd3c4f04a6a611badcb0210b13df1430faf9e1bcbb3d09c250db0335722`  
		Last Modified: Tue, 25 Oct 2022 02:54:15 GMT  
		Size: 200.8 MB (200843786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002fb4889b7643e6efbd6663eb7094d4770d8618719392c5899171a8a7e40221`  
		Last Modified: Tue, 25 Oct 2022 02:53:57 GMT  
		Size: 2.4 MB (2362103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e712504e0116b0bb52f12931b97213d9a38f6fa43ded7056b2aa6c1b8bbe075`  
		Last Modified: Tue, 25 Oct 2022 02:54:00 GMT  
		Size: 58.8 MB (58820411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7c16d01af11c9a306a9c44abbaf97e39e62d33843f72b779d3ae44cac2ee0f`  
		Last Modified: Tue, 25 Oct 2022 02:53:56 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:fb9881b97d8068fde8a658fb529d23f88d491b5d196441817a3ca83b8cdd1f53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.5 MB (314457600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111411c03c18c4fbcf05987ae0581c18b6ecd99c20ffb2012317682616720ef8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 00:06:30 GMT
COPY dir:58f6c37df253d3555e493197f96e3f21593e31d3faf1967e0a7b9d8f0ae9e30c in /opt/java/openjdk 
# Wed, 26 Oct 2022 00:06:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:06:34 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 00:06:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 00:06:35 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 00:06:39 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 00:06:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 00:06:39 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 00:06:56 GMT
RUN boot
# Wed, 26 Oct 2022 00:06:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 00:06:56 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 00:06:57 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707988d24114aa7e1cce7575a23ad15d756aa99d918a94ce41d15291af85fd6`  
		Last Modified: Wed, 26 Oct 2022 00:24:00 GMT  
		Size: 199.6 MB (199582427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb2586ca974b7e96468c9663dc201b8f94b1e79d3c7d80bf4ed46d900834643`  
		Last Modified: Wed, 26 Oct 2022 00:23:48 GMT  
		Size: 2.4 MB (2352289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed28cbc04b9d4a77a0f0908ffca29fcbbbacb0ed98bcc786a79fd601eccf20ee`  
		Last Modified: Wed, 26 Oct 2022 00:23:50 GMT  
		Size: 58.8 MB (58820519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b2b6696b79eee98acf584ac3612a47a38ace6208adb78f11fdc15066dc6d4`  
		Last Modified: Wed, 26 Oct 2022 00:23:47 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
