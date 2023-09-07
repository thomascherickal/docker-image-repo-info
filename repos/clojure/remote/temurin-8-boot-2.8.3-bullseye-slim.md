## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:e56e6b287d9d4004a906309beda0e26d851d2dff0633b6f4c41e17bba5c11133
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:01e29bf61f57914e5802004ed62b4c92d9d609cb2f7aee2d7e84f99985b18b06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194900634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb52bb4f2f5ea99c10030bd3b7abb2c748cb491a621a83899c95c196794c7846`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 03:18:35 GMT
COPY dir:66cfc1773e07dead4d108eefca05e38bbe528aec6797deefc0559c5a4d41e721 in /opt/java/openjdk 
# Thu, 07 Sep 2023 03:18:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:18:36 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 03:18:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 03:18:36 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 03:18:42 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 03:18:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 03:18:42 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 03:19:01 GMT
RUN boot
# Thu, 07 Sep 2023 03:19:01 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a386eaaac993939aefc9356b5f6cc0468dd852762a0b7bb3e195a40c8caf53b`  
		Last Modified: Thu, 07 Sep 2023 03:29:54 GMT  
		Size: 103.6 MB (103585038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f1cade318a18d69d2e48da87953688c38e0007607f1593cc887d404fad90fd`  
		Last Modified: Thu, 07 Sep 2023 03:29:45 GMT  
		Size: 1.1 MB (1077566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76c78ce5194c7ff74e2fb2ecd89f78b1e9b098c3b1821a76993ee18d14367c9`  
		Last Modified: Thu, 07 Sep 2023 03:29:48 GMT  
		Size: 58.8 MB (58820527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4b23d14aeb7274b50175b2ac7bae3c97402d7a87c60e035a5e8a7c19908ef211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192638451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424d5a602fc1c3b6037fdbaef828bea2dd2e077a87305c551db76d19d0b3b85b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 09:04:32 GMT
COPY dir:b83f0a0f236c1f97de459c8ae266f437d3630abb3700f3b868301c8fe017c49a in /opt/java/openjdk 
# Thu, 07 Sep 2023 09:04:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 09:04:34 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 09:04:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 09:04:34 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 09:04:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 09:04:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 09:04:40 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 09:04:59 GMT
RUN boot
# Thu, 07 Sep 2023 09:04:59 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256b28be577c49d6f216cda63c69699c76582076b787ffcf77067af08f7f0490`  
		Last Modified: Thu, 07 Sep 2023 09:14:43 GMT  
		Size: 102.7 MB (102690458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d3fce16ad3a2ff224c1775775cc4dd675ceb7f04d63ddfc3bdddeff78427a0`  
		Last Modified: Thu, 07 Sep 2023 09:14:36 GMT  
		Size: 1.1 MB (1064790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c45e58b39621d1ee1b2c7978343570ba43ffcba167dff9d9f85f6436ba279`  
		Last Modified: Thu, 07 Sep 2023 09:14:40 GMT  
		Size: 58.8 MB (58820300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
