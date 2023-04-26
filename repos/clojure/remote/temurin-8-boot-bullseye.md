## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:fcc441b826ae94571be9dc2a05f950dc9b6d33223001228125d74a3e747c9754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:623d815f137414d74a1b2c62003cacac2a6a9b52203be2808641f3e20598bf6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170877387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c9c4744eb1ed51e8f91da10560d70745cd9add98846a3c6b31e7f710edbecb`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 19:57:54 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Wed, 26 Apr 2023 19:57:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 19:57:54 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 19:57:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 19:57:54 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 19:58:00 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 19:58:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 19:58:00 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 19:58:47 GMT
RUN boot
# Wed, 26 Apr 2023 19:58:47 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7012d2eddb96550ad314f8dd31810e3b6623fb5b245468e7416bb6ee11361e4`  
		Last Modified: Wed, 26 Apr 2023 20:17:20 GMT  
		Size: 54.6 MB (54642102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b690979216e16bc1808d9a7d19996f60724a92db1da1581de391561090c0dc6`  
		Last Modified: Wed, 26 Apr 2023 20:17:14 GMT  
		Size: 2.4 MB (2361677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88987d9597cbbe78b300d4d90c429f6bdf3113394c48b8e66d6af91d729d989`  
		Last Modified: Wed, 26 Apr 2023 20:17:17 GMT  
		Size: 58.8 MB (58820872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cfc5996af8d4ea1a791f7956b56537f3d83a86ed13f878d82f9ee3c34100409c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168620117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3a99e8a3c2fcbe696f098565ff21f2426b76027369f4c5d46d72422ae9d12f1`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:34:13 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:34:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:34:14 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:34:14 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:34:14 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:34:20 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:34:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:34:20 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:34:45 GMT
RUN boot
# Wed, 26 Apr 2023 20:34:45 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f50dc3e320d384b38f12d2aa0cd026391310252439e51cec91f33fb8f2b6ba`  
		Last Modified: Wed, 26 Apr 2023 20:50:04 GMT  
		Size: 53.7 MB (53742685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c00c0d9e2ddba06da1f829d7f9c29bf5d487559ac415434cb07ff1f843b5fc`  
		Last Modified: Wed, 26 Apr 2023 20:49:59 GMT  
		Size: 2.4 MB (2351127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af97f1acbbc6a131b2aa619c8802bfd1c7173989250f70ef026e4a66ca6e2ef`  
		Last Modified: Wed, 26 Apr 2023 20:50:02 GMT  
		Size: 58.8 MB (58820776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
