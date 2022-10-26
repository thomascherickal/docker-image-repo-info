## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:045f75229e60f226226bf1aa1db8934bc9a3011937961a06f87046a01120f3b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:c55b5178270382eb8cb4a7d647f3a6a239d03af8c848aa40a608ec0b051651a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219743300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383d0472c1cd26695f0016f150cbbff9c4d1c69a02d599deaa703fc43d48ad6b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:32:30 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:32:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:32:31 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:32:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:32:31 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:32:37 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:32:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:32:38 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:33:19 GMT
RUN boot
# Tue, 25 Oct 2022 02:33:19 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a9f308d68e7fc10c050f0178ed5da63c43501be70a5e1990e6f5737383502`  
		Last Modified: Tue, 25 Oct 2022 02:48:07 GMT  
		Size: 103.5 MB (103513858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb1a818d1b8727005ebc4e34a7bb26b4c8141d910d5f357fcd82b8b0ee5e455`  
		Last Modified: Tue, 25 Oct 2022 02:47:58 GMT  
		Size: 2.4 MB (2362140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddaf57563cb23a0c8f730bbeacffeca8dd4c71bd22ffc5193d9b6eaa1ca50ba`  
		Last Modified: Tue, 25 Oct 2022 02:48:06 GMT  
		Size: 58.8 MB (58820970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:eea47a90293703c35e441a8d1533d8d5d28dc720a6891086dc92c77943e2ea44
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217488281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8be908c6869daed64b9f873bfd585ebe884d4475a4dde5ca5e38031087b56cc`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 23:53:18 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Tue, 25 Oct 2022 23:53:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 23:53:20 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 23:53:20 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 23:53:20 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 23:53:25 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 23:53:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 23:53:25 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 23:53:42 GMT
RUN boot
# Tue, 25 Oct 2022 23:53:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49c6d9cfee667003a4370293363d578b2b73027ffe0326780e6686aebf34652`  
		Last Modified: Wed, 26 Oct 2022 00:13:32 GMT  
		Size: 102.6 MB (102613479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ec41e5768a9c470393b305777396a180eaae92424baf42a63ab4d2ff33cfa`  
		Last Modified: Wed, 26 Oct 2022 00:13:25 GMT  
		Size: 2.4 MB (2352287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f5019359a7e63f1632c5f13942b92f200b8cd0cb84c92ec2d4a56de91068d5`  
		Last Modified: Wed, 26 Oct 2022 00:13:27 GMT  
		Size: 58.8 MB (58820549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
