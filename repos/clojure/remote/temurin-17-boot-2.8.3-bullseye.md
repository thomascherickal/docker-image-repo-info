## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:d392e3d165d69ef0d072d6da5df920eead4d1c25c940e208dd90c8b4758d36e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

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

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:44e43245361e133fdc009dad72528d2b9f6ebdcc8a7960b55d2bf06ee0defdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306252209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21342e934f4537493affe4dacb42e723a38409b11b2efe5a6a9d6cd4e8e207a2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:43:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:13:41 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 10:13:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 10:13:45 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 May 2023 10:13:45 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 10:13:45 GMT
WORKDIR /tmp
# Thu, 04 May 2023 10:13:50 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 04 May 2023 10:13:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 May 2023 10:13:51 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 May 2023 10:14:07 GMT
RUN boot
# Thu, 04 May 2023 10:14:07 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 04 May 2023 10:14:07 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 04 May 2023 10:14:07 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11090c6457d65efbe72f084b567111755856da82721e52490ffc8bec9b85abff`  
		Last Modified: Thu, 04 May 2023 10:22:02 GMT  
		Size: 191.4 MB (191387646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b1059ae696f7e09817658659d4c6e22191c074e031113b488825e5a8bca486`  
		Last Modified: Thu, 04 May 2023 10:21:51 GMT  
		Size: 2.4 MB (2351131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e021733db85fc32d0cbf8b82b82c0f4d6966157cf4a343fe7f4aea04db717a`  
		Last Modified: Thu, 04 May 2023 10:21:54 GMT  
		Size: 58.8 MB (58820329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d3b61177dfd6cee11fb3366feaaa34b8f7acb4e9b0d211e7859a70c4bae37`  
		Last Modified: Thu, 04 May 2023 10:21:50 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
