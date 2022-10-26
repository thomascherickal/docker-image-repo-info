## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:32ee556e16aa6d5f70300c115f00bd2a81b6a1a9296279e53f3d41265b75b213
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
$ docker pull clojure@sha256:7d33d3876d542906328785932de0090fed5bc57b4b0ff34256fd53090697828e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.7 MB (309741179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca4dd2e11301f813d0c372561c193bf49f0066b40385365aba9a64d941081ec`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 23:58:29 GMT
COPY dir:0dc06d70d42a32ae203bdf41d3806f1204b90ca101c4efe4662ba862f2c76b8a in /opt/java/openjdk 
# Tue, 25 Oct 2022 23:58:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 23:58:34 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 23:58:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 23:58:34 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 23:58:38 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 23:58:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 23:58:39 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 23:58:55 GMT
RUN boot
# Tue, 25 Oct 2022 23:58:55 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99902a91af1a5ac43f8cea176770b6ec766f5259b18c45fd17a0de6098ce0bac`  
		Last Modified: Wed, 26 Oct 2022 00:16:49 GMT  
		Size: 194.9 MB (194866492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda3102a4cd474104d6eabb512adee4e3c55941f6169345ef201a85fb22c23bb`  
		Last Modified: Wed, 26 Oct 2022 00:16:38 GMT  
		Size: 2.4 MB (2352291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc620917521f22c2584fcccda1d3164b67674423ed0f6d21897305def0aaee5`  
		Last Modified: Wed, 26 Oct 2022 00:16:41 GMT  
		Size: 58.8 MB (58820430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
