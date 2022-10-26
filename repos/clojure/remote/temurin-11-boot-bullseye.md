## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:8699d780d24e445fb835280857bb5adb121ede1e382242b2158c9de81c6cc9fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:394d7bc94fcf65f07e2c8c06645496994fe6d8a5ffe09602b2e350c75ed4b85e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314354033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa6534eada4c96fd2c8e4037f74036dd51a77511d35670e62f92aec769b73e9`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:36:10 GMT
COPY dir:e3c63d67b32fccda756dd62000a0cf47da966d18fe6f1f25cd1f37b60881f0ec in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:36:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:36:11 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:36:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:36:12 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:36:18 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:36:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:36:18 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:36:44 GMT
RUN boot
# Tue, 25 Oct 2022 02:36:45 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e425413bc0ae0b1045fcbc0ad4409b98eeded13a40018b63e55084142fd5a78e`  
		Last Modified: Tue, 25 Oct 2022 02:50:03 GMT  
		Size: 198.1 MB (198124992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95579b13a17b52f247d5d3ff7eee3138dcb4ea92bdd38222b08510ab484641bf`  
		Last Modified: Tue, 25 Oct 2022 02:49:48 GMT  
		Size: 2.4 MB (2362104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a7f9052c1e36ea7dcabb6e34b3a2d4e3784d04e076891cc2ec033fbf9953ac`  
		Last Modified: Tue, 25 Oct 2022 02:49:52 GMT  
		Size: 58.8 MB (58820605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f1ef1f4bd872b8c3f4e7a7be7de1627612dcb4b164b7ceef2b12a797ae48f75c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.7 MB (309741625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc9905c3d15ef4afc7f91b5153f0718516d388ba8687c584e1e239ef7661b08a`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:37:43 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:37:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:37:48 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:37:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:37:48 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:38:06 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:38:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:38:07 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:38:24 GMT
RUN boot
# Wed, 26 Oct 2022 15:38:24 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a7b51e23fc2e53d8018b07b36bae7b1c261267f2981e18b50be0d7b845881`  
		Last Modified: Wed, 26 Oct 2022 15:57:42 GMT  
		Size: 194.9 MB (194866970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef805b45caa2352f0f6905bf81b99263dbfa1b2fc932d475262693899c9c708`  
		Last Modified: Wed, 26 Oct 2022 15:57:30 GMT  
		Size: 2.4 MB (2352281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6147e6b271780d0ec957d2ebd037f7caf814481713593d41c81e00f327f086f9`  
		Last Modified: Wed, 26 Oct 2022 15:57:33 GMT  
		Size: 58.8 MB (58820408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
