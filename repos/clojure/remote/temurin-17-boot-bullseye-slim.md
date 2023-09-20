## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:c1d56bb9765051f844287901f8e19642e039e339d5e303618c9e3d5aac1cf410
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:eb97933742e1eb6df562551f7b7f8d54e8eb7fda7cbbe2942b99d8aab3b8392a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236091720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d7e40f1dd7b9da21450a268da824797fc95bc1f9d295d8a160407fc98f62bdc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:22:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 07:28:19 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Wed, 20 Sep 2023 07:28:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 07:28:20 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 07:28:20 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 07:28:20 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 07:28:26 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 07:28:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 07:28:26 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 07:28:44 GMT
RUN boot
# Wed, 20 Sep 2023 07:28:44 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 20 Sep 2023 07:28:44 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 20 Sep 2023 07:28:44 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f849626c60449d70414a79d12d1df3b48aa0c9fe4ae3176ba320531d57b9d3`  
		Last Modified: Wed, 20 Sep 2023 07:37:37 GMT  
		Size: 144.8 MB (144775758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19c1e8c3a86b82cfaa807035a7a968e324b909729bb3b23575fc38e4372ed12`  
		Last Modified: Wed, 20 Sep 2023 07:37:26 GMT  
		Size: 1.1 MB (1077548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b38adf28b3f10eb3c89043d2d3f738395d27ae1d9fd03b850cf47ab79b29f7`  
		Last Modified: Wed, 20 Sep 2023 07:37:29 GMT  
		Size: 58.8 MB (58820305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1397fcda0b074f0b2fa26444da57a521dcce35d60618e57762217daac493af70`  
		Last Modified: Wed, 20 Sep 2023 07:37:25 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5becc2aa3b2a2045cbe48a4af03643680a20ca0d44cb65f614ff2f328f994e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.5 MB (233492055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e3085db1e5573fbef2c2aaaa66e1436d057c1ae55d86c71d35461c4ac40f28`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:48:13 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 09:53:09 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Wed, 20 Sep 2023 09:53:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 09:53:13 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 09:53:13 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 09:53:13 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 09:53:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 09:53:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 09:53:18 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 09:53:34 GMT
RUN boot
# Wed, 20 Sep 2023 09:53:35 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 20 Sep 2023 09:53:35 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 20 Sep 2023 09:53:35 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603608103e3f4f9bafbfe00174b3aa6d67a38d93136e7e6343f0b5b25ffa8ace`  
		Last Modified: Wed, 20 Sep 2023 10:01:18 GMT  
		Size: 143.5 MB (143543516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e182e8ac0cf2446ca8debd9c36621e87afafc7bf002e800d709351b08a8eb798`  
		Last Modified: Wed, 20 Sep 2023 10:01:08 GMT  
		Size: 1.1 MB (1064785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beb0d02cf1d7e5b0d60e4527f4551246d4f055ce87b52a5179c12097478efc`  
		Last Modified: Wed, 20 Sep 2023 10:01:11 GMT  
		Size: 58.8 MB (58820487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc41f23fd9ee31046e75af219f67dca74c7d334cf64057d12897ab32e9f938`  
		Last Modified: Wed, 20 Sep 2023 10:01:07 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
