## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:35a8df74967933f16b0fe1e1852e929d24999861d70c761b26d810febef7de11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:bb837fe68a51973ca026584a09ed203f1f8befa80eddff78f8442ddef3871848
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170873637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85eb2183b80411b5d7eb779ddab14059a0a0c426d3b85fa3b9adfd60f2ed43e6`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:24:11 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Wed, 03 May 2023 20:24:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 20:24:11 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 03 May 2023 20:24:11 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 03 May 2023 20:24:11 GMT
WORKDIR /tmp
# Wed, 03 May 2023 20:24:17 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 03 May 2023 20:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 03 May 2023 20:24:17 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 03 May 2023 20:24:39 GMT
RUN boot
# Wed, 03 May 2023 20:24:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5e2c1247e792b32dfc253554b769e50b9d0e00b87bda347fdad278b672e1b2`  
		Last Modified: Wed, 03 May 2023 20:35:03 GMT  
		Size: 54.6 MB (54642112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ab8563a7ff31d93d93455ba91350716d4445e104a74c3f5fc95d0eb7aa215e`  
		Last Modified: Wed, 03 May 2023 20:34:57 GMT  
		Size: 2.4 MB (2361754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c4ddd1d7de4f32089310a1123d6b78fe0eb67138f159baed76a66d6f7621a4`  
		Last Modified: Wed, 03 May 2023 20:35:00 GMT  
		Size: 58.8 MB (58820701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ae03b53cf9eb41a6e1bcf9f661a8cb642ca625f52ddd0c803a9090c8cb34dc72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168607130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9474315b574e4667b3cccbe6a88fcb7355a7c2d5b6ad231e2d9f427829c2b7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:24:11 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 23 May 2023 01:24:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:24:12 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:24:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:24:12 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:24:17 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:24:18 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:24:50 GMT
RUN boot
# Tue, 23 May 2023 01:24:51 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec933d3080ef0a9a725f147ed686986ad36ef60808bf5f0ed2091007522988c`  
		Last Modified: Tue, 23 May 2023 01:34:03 GMT  
		Size: 53.7 MB (53742673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070959a9f233868fc78ef05bae1acb49aba6d3df875b0f4e7cf339f7e6715fd`  
		Last Modified: Tue, 23 May 2023 01:33:59 GMT  
		Size: 2.4 MB (2351112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0529d8976c41b9274b951b8bcfeee0fd4e000a4228ff878962f98c816f7ec201`  
		Last Modified: Tue, 23 May 2023 01:34:01 GMT  
		Size: 58.8 MB (58820733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
