## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:918f6070e7267a14ef60df36b37e1c9dc373c629adbde087a028f46a8820d69e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:46b61b8062f9ad2fb9a60e4414b7df5498fe48d92d6501d16d31e1ed62f215cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261012413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbcd81c1f9199d7109605822475c20f71aa4ebb92c495b107b4d797a66aea05`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 22:36:59 GMT
COPY dir:8ea3eea47bd8b9d37ce2403b2d64b2cdc0fec836a119c10ec3e4ff0bcca8bb4d in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:37:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:37:00 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Aug 2023 22:37:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 22:37:01 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 22:37:06 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Aug 2023 22:37:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 22:37:06 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Aug 2023 22:37:25 GMT
RUN boot
# Tue, 08 Aug 2023 22:37:25 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 08 Aug 2023 22:37:25 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Aug 2023 22:37:25 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad5f652aa0a9735f05b6a5d86369751c117fe48131a7c9ff7427b064b3036c`  
		Last Modified: Tue, 08 Aug 2023 22:49:32 GMT  
		Size: 144.8 MB (144773784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f5740c78f916e6f9a74d8ce98a06d2355cef3f8005d9dd884a8bc3c05889de`  
		Last Modified: Tue, 08 Aug 2023 22:49:21 GMT  
		Size: 2.4 MB (2362232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bf6fa973a9adcea2ff35f903273e3e7d04512db03b8114a719538a17368d52`  
		Last Modified: Tue, 08 Aug 2023 22:49:25 GMT  
		Size: 58.8 MB (58820425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cf15e1a46a95620682c352f70ebc6bb3b4186d022bf845b276df3926cc5cbf`  
		Last Modified: Tue, 08 Aug 2023 22:49:20 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8149c13250870e77e2964ce3ffe7222227e1a04134f661bc4fce0413ff5aba20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258415376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d5b3c3b22c259e7bd515f63aa2c78fe20c9df5bd9ff7d3110123d0022d65f2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 14:35:02 GMT
COPY dir:ea833e6c6c81bc32cfded5d05d30b781acc802f6c770c2720afc9a9f14f4a7d5 in /opt/java/openjdk 
# Fri, 28 Jul 2023 14:35:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:35:06 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 28 Jul 2023 14:35:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 28 Jul 2023 14:35:06 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 14:35:11 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 28 Jul 2023 14:35:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 28 Jul 2023 14:35:11 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 28 Jul 2023 14:35:30 GMT
RUN boot
# Fri, 28 Jul 2023 14:35:30 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 28 Jul 2023 14:35:31 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Jul 2023 14:35:31 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d0f61795693efb86b2bc273c0ea30def7d3c4e57a24be4dac110415235a921`  
		Last Modified: Fri, 28 Jul 2023 14:43:11 GMT  
		Size: 143.5 MB (143538050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3310b9d380f122338aa57bc4b8cc9a19b14803ce0d57ec0d8da83fbd2e7f87`  
		Last Modified: Fri, 28 Jul 2023 14:43:02 GMT  
		Size: 2.4 MB (2351486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23ba02943b43ba70cec21196d202a963b0cd27cb4f0bff24e51d1b5e95e4c0f`  
		Last Modified: Fri, 28 Jul 2023 14:43:07 GMT  
		Size: 58.8 MB (58820651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4567a0bf9975caa9a8b730b6bbf21fbb7c64d230edf1b5a9ef901e3b72a234`  
		Last Modified: Fri, 28 Jul 2023 14:43:02 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
