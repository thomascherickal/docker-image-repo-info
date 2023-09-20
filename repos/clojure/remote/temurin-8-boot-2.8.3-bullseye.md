## `clojure:temurin-8-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:9dcc8e42df89cb27e57e828d6fe5bc13296c0829835ffedd01532b9a1d656522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f91a7d9bdf20bf4f8e6f8fe12a290582943b522cf26e785330df25170d5f9c11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.8 MB (219824375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a0ed2e724a2e191de9561bf773e26d650cf50fe1bbe4c6f432b27510df7414`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:21:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 07:21:48 GMT
COPY dir:66cfc1773e07dead4d108eefca05e38bbe528aec6797deefc0559c5a4d41e721 in /opt/java/openjdk 
# Wed, 20 Sep 2023 07:21:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 07:21:49 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 07:21:49 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 07:21:49 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 07:21:55 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 07:21:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 07:21:56 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 07:22:18 GMT
RUN boot
# Wed, 20 Sep 2023 07:22:18 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b0aa7fd12821e6e0bd8d864138e0a239c587d7c9e54b266a9620f577d42bf3`  
		Last Modified: Wed, 20 Sep 2023 07:33:50 GMT  
		Size: 103.6 MB (103585016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ad57434bf071b384a66fd1b6680430cfefd6ff8231e0d150f06d742c53b5ac`  
		Last Modified: Wed, 20 Sep 2023 07:33:41 GMT  
		Size: 2.4 MB (2362100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f04cea8bd7ff3c354f23e1c3bbe180c2f377166ea41ba660886b2fcc080e42`  
		Last Modified: Wed, 20 Sep 2023 07:33:45 GMT  
		Size: 58.8 MB (58820545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c6826f88908dcf6388ac4fa6ee1caf60c0526e90534f00a38fd9b1ad1d5d660b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217567502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22c1290b0997878dee13268d2079a548839f54406591b8d95b0b49980124c212`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:47:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 09:47:34 GMT
COPY dir:b83f0a0f236c1f97de459c8ae266f437d3630abb3700f3b868301c8fe017c49a in /opt/java/openjdk 
# Wed, 20 Sep 2023 09:47:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 09:47:36 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 09:47:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 09:47:36 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 09:47:41 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 09:47:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 09:47:42 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 09:48:08 GMT
RUN boot
# Wed, 20 Sep 2023 09:48:09 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d0ce55c1092b158aa3b98322b5a8b5ad90f95419e892e511c16b3656e8f572`  
		Last Modified: Wed, 20 Sep 2023 09:57:49 GMT  
		Size: 102.7 MB (102690462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a24920e63661dc1e73fa2217b7382451b7eba8dd0e946ea8ab2703cbdddacf`  
		Last Modified: Wed, 20 Sep 2023 09:57:42 GMT  
		Size: 2.4 MB (2351401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021b9b0a395a6311bb45d8b4b126a78426b9d6d85a1ed0a66ab7b2f1c9727010`  
		Last Modified: Wed, 20 Sep 2023 09:57:45 GMT  
		Size: 58.8 MB (58820747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
