## `clojure:temurin-11-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:4207c4d1ec4b853d9e66bb94f3c2f553ab5f292c76a596ac58eb2363a7d20f19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:ed0cd4d647adf9f908d40f2365cf3ae3d604ec6ff63f5c3cb113ccc1c0239f26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314787217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76c475c942ec3ffb8cbb9e4d91b102b4756b2d36971fa38ade7b0eb23cd77016`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:59:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:18:57 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Wed, 05 Jul 2023 11:18:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 11:18:59 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 05 Jul 2023 11:18:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 05 Jul 2023 11:18:59 GMT
WORKDIR /tmp
# Wed, 05 Jul 2023 11:19:07 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 05 Jul 2023 11:19:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 05 Jul 2023 11:19:07 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 05 Jul 2023 11:19:24 GMT
RUN boot
# Wed, 05 Jul 2023 11:19:25 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f32c79546e308866ce38369edf4614a73777193f0a490707182288427a0b9a`  
		Last Modified: Wed, 05 Jul 2023 11:32:34 GMT  
		Size: 198.5 MB (198549453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac5474a81b3a655015be1afc5cee182ba9e135fcd6925ebd8f4dad35d714634`  
		Last Modified: Wed, 05 Jul 2023 11:32:21 GMT  
		Size: 2.4 MB (2362061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c27c9375729b384945cea8d8c057bb25f93984b0708269700d596bef1d5b547`  
		Last Modified: Wed, 05 Jul 2023 11:32:24 GMT  
		Size: 58.8 MB (58820403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2249e9fb7909d950c7577c7f4f8adcbe7b7a41a90342bd8bf6b13efb92f59977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.4 MB (256441215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201e691361556a9a6b136d714fe1bd23bb68b13a8228b0ac58fe91ab2c898bf0`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:43:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Jul 2023 01:07:04 GMT
COPY dir:e71da8247d58ed4b0dfbf219951c863c79ac94b7f45cb60320ea827dfa699275 in /opt/java/openjdk 
# Wed, 26 Jul 2023 01:07:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 01:07:07 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Jul 2023 01:07:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Jul 2023 01:07:08 GMT
WORKDIR /tmp
# Wed, 26 Jul 2023 01:07:13 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Jul 2023 01:07:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Jul 2023 01:07:13 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Jul 2023 01:07:32 GMT
RUN boot
# Wed, 26 Jul 2023 01:07:33 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a099a46124988665742eae84cd51e5a2ec69ba12a5a0324bfdecb15c9fcca0ec`  
		Last Modified: Wed, 26 Jul 2023 01:13:29 GMT  
		Size: 141.6 MB (141565305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b34da4dc58b8551e76f9c5e3c916466191bf7ac36466592eabfa5fc42b738c`  
		Last Modified: Wed, 26 Jul 2023 01:13:20 GMT  
		Size: 2.4 MB (2351394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f357330e1bb51be8f74c4f777503bc25b17ba6494113f8c22da6676ec2c430`  
		Last Modified: Wed, 26 Jul 2023 01:13:22 GMT  
		Size: 58.8 MB (58820537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
