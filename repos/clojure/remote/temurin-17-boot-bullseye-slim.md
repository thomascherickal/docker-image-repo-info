## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:6a4e2dd35fa35d5116817933a05e9b7fade798f9d274adb3bd1605213358ba13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:cf2613f6199a9c6d7b8d26d5ad062d695990a92707fc31d440eb6707c7beeeb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.9 MB (283897032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a91118f7ba56e0b7c091c116bd3d1aee023dac6d36fe82550e23e3a73a86c21`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:09:11 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:09:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:09:12 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:09:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:09:12 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:09:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:09:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:09:18 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:09:35 GMT
RUN boot
# Wed, 26 Apr 2023 20:09:35 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Apr 2023 20:09:36 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Apr 2023 20:09:36 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dca630898b65b3e3d97ffce265d16549a24facef0348fd8a6d8d5aee0493b3`  
		Last Modified: Wed, 26 Apr 2023 20:24:23 GMT  
		Size: 192.6 MB (192580428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8dc93ac75a348ee7b4ec2fcec25ac191d749da2df80e06bcc4b3c06bdacd58`  
		Last Modified: Wed, 26 Apr 2023 20:24:09 GMT  
		Size: 1.1 MB (1077506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4a7af206e939d030d987e720113a9f4f88ec2b19f2f34a207691e1c67208f4`  
		Last Modified: Wed, 26 Apr 2023 20:24:13 GMT  
		Size: 58.8 MB (58820470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6112ceb4a38c0a1ac3a31a84d5605072db5f292d75882b658f54d2ee444df74e`  
		Last Modified: Wed, 26 Apr 2023 20:24:09 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ee651c1a69c63aefff0eb3add56204848fba95225a3a2fdbc56f36af4f51570f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281337297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90261324fdac6af789621613ce4d1c58bd0a33124545678c83c372eb1cdbec50`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:43:30 GMT
COPY dir:d3d9f08d06fd1214b20f5d901cee398f498773bedf69f0d3cc795772967cfe44 in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:43:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:43:34 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:43:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:43:34 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:43:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:43:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:43:39 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:43:55 GMT
RUN boot
# Wed, 26 Apr 2023 20:43:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Apr 2023 20:43:56 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Apr 2023 20:43:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583bb3029fa1410e5fe69cb8c1d3ec8b162189c224628b2cfd41d97a9456f302`  
		Last Modified: Wed, 26 Apr 2023 20:55:49 GMT  
		Size: 191.4 MB (191387717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a542b1cc9d788882c7bdff40c76a3873a4cfbed44c10b759d1cf766977709da0`  
		Last Modified: Wed, 26 Apr 2023 20:55:38 GMT  
		Size: 1.1 MB (1064825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab859cec27463e0e6134f2af391a3af8b8434dd28325a0a4d121407dfd15849`  
		Last Modified: Wed, 26 Apr 2023 20:55:41 GMT  
		Size: 58.8 MB (58820528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d25e3a1f950325ca5720e6ac646a17c3097ee8ed95dfae251eb78c5e4ba52da`  
		Last Modified: Wed, 26 Apr 2023 20:55:38 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
