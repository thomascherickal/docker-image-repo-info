## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:5108109a419c4fd087160a89a2557c92a022e8cd3a52df4d3db0ebcdafa1188a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:ff20fdff0b342670a860a1351116a799c213bf0c44bcc0026374b5761ec640ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.8 MB (308812069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989f50989aed27ec6530b950338cb56d93b27e74c65615e131cb1d8453fa3052`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:58:53 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Thu, 04 May 2023 14:58:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 14:58:54 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 May 2023 14:58:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 14:58:54 GMT
WORKDIR /tmp
# Thu, 04 May 2023 14:58:59 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 04 May 2023 14:58:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 May 2023 14:58:59 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 May 2023 14:59:17 GMT
RUN boot
# Thu, 04 May 2023 14:59:17 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 04 May 2023 14:59:17 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 04 May 2023 14:59:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbada72a4382332aa6aa78d824d0bdddefea4c233d0617f4e8924c1c87446c9`  
		Last Modified: Thu, 04 May 2023 15:09:12 GMT  
		Size: 192.6 MB (192580390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c88e896b65fe7143050c012744fe4d228c1ca96b6b6218519f3c607cef8f9d`  
		Last Modified: Thu, 04 May 2023 15:08:26 GMT  
		Size: 2.4 MB (2361626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8d1a09ee6053183d119cb306e67bb1bbc94f918ceb75421065d481f286c859`  
		Last Modified: Thu, 04 May 2023 15:08:30 GMT  
		Size: 58.8 MB (58820585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6580edd35311b629aa4ea84762d0cb5b9ed3cb6f5c143c22b2ad1ed7b9d9d3c`  
		Last Modified: Thu, 04 May 2023 15:08:26 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d9cc765f875b3f472b38ad88c7c5577609f6f8c90e5cf5c7284311f83720d58f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306252244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed456089946e4d2833ed2a5f7102962bb8c445e4d3e3fc144177077788b12caa`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:29:19 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Tue, 23 May 2023 01:29:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:29:23 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:29:23 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:29:23 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:29:28 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:29:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:29:28 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:29:45 GMT
RUN boot
# Tue, 23 May 2023 01:29:45 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:29:45 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:29:45 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6f4a297b4e40485159fdaaaca21c302eba0567a5165c796f74cdfaaaeeefed`  
		Last Modified: Tue, 23 May 2023 01:37:02 GMT  
		Size: 191.4 MB (191387676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7e1127f0bdff212b7d7fccce2e04e17e08ed54f53f50955c7bde469892a92`  
		Last Modified: Tue, 23 May 2023 01:36:51 GMT  
		Size: 2.4 MB (2351078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7681014644c2f634d8064cf457a8935999a653e8553624fcfe742f4647284a`  
		Last Modified: Tue, 23 May 2023 01:36:54 GMT  
		Size: 58.8 MB (58820478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecfc5407a3e71b919660ad2d8afc5740a417501d54517b118e1493f5fca1546`  
		Last Modified: Tue, 23 May 2023 01:36:51 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
