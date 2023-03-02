## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:bbd657461ef0b62447c6924ce290836ae63a2078f799ea235119582a53c956e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:44b9aa6d98456fd6ff5357d3dbc7ea2fffc29fed10a9e9e73d77fb01b1d12006
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283747694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03e9b818366b348c50af0c0c8275299e2d5d8c863faeb79fe9c7687697d6a8f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:41:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 09:01:07 GMT
COPY dir:186a37b080989e6e1268f71ac4b081d0a966a2c5c8b71fa2a808fe83b4537ae1 in /opt/java/openjdk 
# Thu, 02 Mar 2023 09:01:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 09:01:09 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 02 Mar 2023 09:01:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 02 Mar 2023 09:01:09 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 09:01:15 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 02 Mar 2023 09:01:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 02 Mar 2023 09:01:15 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 02 Mar 2023 09:01:33 GMT
RUN boot
# Thu, 02 Mar 2023 09:01:34 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 09:01:34 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 09:01:34 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93920d1539d63c977bce91553f85dcaf59acca3032ac3d7434770f05c8b85044`  
		Last Modified: Thu, 02 Mar 2023 09:16:09 GMT  
		Size: 192.4 MB (192438217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934cb9a5846c09e8b3f38843e9ad72f6f76a3240dda767660d262d06b688ee1`  
		Last Modified: Thu, 02 Mar 2023 09:15:55 GMT  
		Size: 1.1 MB (1077395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632d8fb7d9dac2684a3aac7d3bf911bd3ab64af9e5e2d2a45c9653669b6f7931`  
		Last Modified: Thu, 02 Mar 2023 09:15:58 GMT  
		Size: 58.8 MB (58820279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3cb5e1933d52c41fc08ddd25afdba921e23a09639bbed6113b0b86b7672ac8`  
		Last Modified: Thu, 02 Mar 2023 09:15:54 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8c2f8a4af19fe9818bfabd85662c0e3cd71d17b00cdc1bd0f67bbf89427b7ada
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281208615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f985e58f6a2b58a6ba838f454f386d97a60b0c350fb21dc2b77104494b7cb54`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:07:04 GMT
COPY dir:47c117bbc947c5c1164b5a20eeec0ba16c306f5991a85f22c54db31ca24ce4a8 in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:07:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:07:09 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 02 Mar 2023 07:07:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 02 Mar 2023 07:07:09 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:07:13 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 02 Mar 2023 07:07:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 02 Mar 2023 07:07:14 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 02 Mar 2023 07:07:30 GMT
RUN boot
# Thu, 02 Mar 2023 07:07:30 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 07:07:30 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 07:07:30 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee2a535b626ac45b3b701a33ede28cb7ec44388615e651313d6818cbca5d626`  
		Last Modified: Thu, 02 Mar 2023 07:20:21 GMT  
		Size: 191.3 MB (191260449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46707d6f176c7caefa33e0ab0895e47c0ae088d77d901b444fbf85f223b07c6`  
		Last Modified: Thu, 02 Mar 2023 07:20:11 GMT  
		Size: 1.1 MB (1064646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1c6b3fcef6147103938a8d330e27f70486db3f06c67f12a62fcac0b766b960`  
		Last Modified: Thu, 02 Mar 2023 07:20:13 GMT  
		Size: 58.8 MB (58820306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce02da0c4210f9dc526383bfcb671bb4c14feec1efc83a01ff1e052835048849`  
		Last Modified: Thu, 02 Mar 2023 07:20:10 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
