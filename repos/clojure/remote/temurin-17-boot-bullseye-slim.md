## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:33e449f6d3b06319e0ae0067ee2f3cf71c020c2a55ed36f6e6f6933fc7cc0907
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:85c2e4044be4abb95ea4cb305e6a51db8d12285229aec39758a2b7a1ab7557d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283726556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbe1df793ff07d48677c0efe1327ed26c75d4ac09a80376335f61fe82bd215ea`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:57:05 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:57:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:57:06 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:57:07 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:57:07 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:57:12 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:57:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:57:13 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:57:31 GMT
RUN boot
# Wed, 21 Dec 2022 01:57:32 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 01:57:32 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 01:57:32 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3d6f042d4c187dc5ef35678240ad79b89963342d31898de3665a87a1568323`  
		Last Modified: Wed, 21 Dec 2022 02:09:14 GMT  
		Size: 192.4 MB (192431237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98181d821868f793c7f9e59a9df29617ccff0abf2504f2bd45ac1ecae688f9ae`  
		Last Modified: Wed, 21 Dec 2022 02:08:59 GMT  
		Size: 1.1 MB (1077347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90cf1b2d5b8d0db7754a9b214f005a4b034b480f0a81473fb55838c2e74ce91`  
		Last Modified: Wed, 21 Dec 2022 02:09:02 GMT  
		Size: 58.8 MB (58820627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258837f66277d509c2f861bf9c26f865b126d436024ebf64ab74c8c63f5624d`  
		Last Modified: Wed, 21 Dec 2022 02:08:58 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3fb66174afb96e7c37207fa1f0946e6071628134d8cd681b0a55720208205535
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281145476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc8c89dade86d919d368e9e987fc74d8a75a2d8e15e8925fdb92a1dd580c1455`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:23:45 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:23:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:23:50 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:23:50 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:23:50 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:23:54 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:23:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:23:55 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:24:13 GMT
RUN boot
# Wed, 21 Dec 2022 02:24:13 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:24:13 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:24:13 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe0bd60bb0c98d49d30600631e90ec3ae088afce058b74e503fe7c363701de4`  
		Last Modified: Wed, 21 Dec 2022 02:34:16 GMT  
		Size: 191.2 MB (191215202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f00180f074102c3724b18c073ef046abfcc9aa84fc61f8f4b677bccf883d66`  
		Last Modified: Wed, 21 Dec 2022 02:34:05 GMT  
		Size: 1.1 MB (1064633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd45a1a034c123c509d4f511dcf06123386428592d72ac8d3d0601f6b180b4`  
		Last Modified: Wed, 21 Dec 2022 02:34:07 GMT  
		Size: 58.8 MB (58820469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b33bfadabcb90c0a7faef189a3ac61a24794194a54c0065e36a3aaebe49bc5`  
		Last Modified: Wed, 21 Dec 2022 02:34:05 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
