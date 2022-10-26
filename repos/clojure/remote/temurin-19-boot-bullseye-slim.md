## `clojure:temurin-19-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:ca503e2b6b36202a7503a7ded9b2a7657e34e00d741f1946d256e010e0dfd98b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:e3ca4cca7e8a53f5dfb205bb75151f24e38d7e2bc6e18c4d8bc0e927b273393c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.2 MB (292163678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3f7feef748e078032bf633ac8216a44f5806279b05f32ee54f209c22f0d5d4d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:43:04 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:43:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:43:05 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:43:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:43:06 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:43:12 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:43:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:43:12 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:43:30 GMT
RUN boot
# Tue, 25 Oct 2022 02:43:30 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 25 Oct 2022 02:43:31 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 25 Oct 2022 02:43:31 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef26e3fe67290659a7b3a065746d54031cd623809f8df384628be68ee2d54a24`  
		Last Modified: Tue, 25 Oct 2022 02:54:40 GMT  
		Size: 200.8 MB (200843786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eb45ac2b21603d6dbc013f3bc7ee8db0096db523ad3216748b9c7f3b1bb869`  
		Last Modified: Tue, 25 Oct 2022 02:54:25 GMT  
		Size: 1.1 MB (1078969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d80eae301b693cf079f018bbfd02028c30542acdc2baa47205eb744f99206cf`  
		Last Modified: Tue, 25 Oct 2022 02:54:29 GMT  
		Size: 58.8 MB (58820484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e60ac0629db00c6704cbe33c1894c1de24985934157a3aa7feb1b391e148155`  
		Last Modified: Tue, 25 Oct 2022 02:54:25 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f8c9818a46178d4887f209dbbc3c926ef002d483eaaa64ba907045cf7cdfd8b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289533559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fc253617048a9c33f39e7ca6e75b49bcdcb7576bd21c9da2b8e4c58b39d02d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 00:07:03 GMT
COPY dir:58f6c37df253d3555e493197f96e3f21593e31d3faf1967e0a7b9d8f0ae9e30c in /opt/java/openjdk 
# Wed, 26 Oct 2022 00:07:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:07:08 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 00:07:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 00:07:08 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 00:07:12 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 00:07:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 00:07:13 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 00:07:30 GMT
RUN boot
# Wed, 26 Oct 2022 00:07:30 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 00:07:30 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 00:07:30 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cd2f77b9ca1d88a3518469394f637729f6d045c474567a40a45a79d7fcc83b`  
		Last Modified: Wed, 26 Oct 2022 00:24:22 GMT  
		Size: 199.6 MB (199582396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212c6022edec10800e4529adedb626e4b27b0953d34ada6a39ef793b7a69429`  
		Last Modified: Wed, 26 Oct 2022 00:24:10 GMT  
		Size: 1.1 MB (1066360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2cf9adce16c68f5b84e7c56101cfafc7c71ca89b4b0755c51c313b732cd6af`  
		Last Modified: Wed, 26 Oct 2022 00:24:13 GMT  
		Size: 58.8 MB (58820492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aef9b53682c8f2e7d448b1fe72b423fbd7ac9001516b1b84240b822a76fadea`  
		Last Modified: Wed, 26 Oct 2022 00:24:10 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
