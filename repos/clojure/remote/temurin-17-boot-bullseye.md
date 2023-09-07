## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:8038ceb1ef268472f0b3efe0da0be896335e4bcee16ce9e9b1f052ce24486427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f691bf3ed3d843ad44049a78b6e0307ee823aca25b867a91e174de120e5a1fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261014947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce82e522f96232a91f0f5328e1aa320b58246e08e6c8023ca0aa363083a886e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:17:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 03:23:42 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Thu, 07 Sep 2023 03:23:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:23:43 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 03:23:43 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 03:23:44 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 03:23:49 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 03:23:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 03:23:49 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 03:24:07 GMT
RUN boot
# Thu, 07 Sep 2023 03:24:08 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 07 Sep 2023 03:24:08 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 07 Sep 2023 03:24:08 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f659b2aacdd3e2363ebb3332a830f2dcd93164a10995d976ac13e700435f5`  
		Last Modified: Thu, 07 Sep 2023 03:33:07 GMT  
		Size: 144.8 MB (144775757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d4e0642c0a2744d6ac7f362ed9f7adb9a01154e767c4fd69fa997707b202a9`  
		Last Modified: Thu, 07 Sep 2023 03:32:56 GMT  
		Size: 2.4 MB (2362046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fa48699b8a4017d46e47df9d3091388a7deddff00fd8c69e95b7e2eedbbb8c`  
		Last Modified: Thu, 07 Sep 2023 03:32:59 GMT  
		Size: 58.8 MB (58820499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a193c404a92ec2c3482f7e6bf1a6521fe42e7f9ae96ff30e773206c750a0edef`  
		Last Modified: Thu, 07 Sep 2023 03:32:55 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1e10a2196f080c048c258cd538526f4a2af73700e4529db618ee98bc419e0792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258420374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dae3e98d9984ee439cd3869ecd631ea991ae7896264141cbe5624954c4e360`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:03:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 09:09:15 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Thu, 07 Sep 2023 09:09:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 09:09:18 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 09:09:18 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 09:09:19 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 09:09:24 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 09:09:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 09:09:24 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 09:09:41 GMT
RUN boot
# Thu, 07 Sep 2023 09:09:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 07 Sep 2023 09:09:41 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 07 Sep 2023 09:09:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11abafe6bd868d46b7ee281876a4f1449b1024ece764bcbdf2e54191d6f14bf0`  
		Last Modified: Thu, 07 Sep 2023 09:17:33 GMT  
		Size: 143.5 MB (143543491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be05c2962b5ebaa558079a426a506136d92228b44d2ffd055747b5e83232655`  
		Last Modified: Thu, 07 Sep 2023 09:17:24 GMT  
		Size: 2.4 MB (2351383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33997da7a0b618ef7594a8377e559dbe26038d7191738e9419fc06b4737d5073`  
		Last Modified: Thu, 07 Sep 2023 09:17:26 GMT  
		Size: 58.8 MB (58820385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00699bb9a628d649b3f9ff85acc796643f7a0dce26c32b4e3b52b72e6fa4f88b`  
		Last Modified: Thu, 07 Sep 2023 09:17:23 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
