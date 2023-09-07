## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:91f2703bd7e1c097ed5f61092c6647b14a7fcebe2af6d838cfc8e307a23aba89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:9fce21930930c9cc04323e294a47335b8845a2afb0ca441602cb9bfd6c23f977
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.8 MB (219824386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:462bdb239bb47ef6157c372645412527b8cb9cdd2bd1405eecb3d2a02ebc0f73`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:17:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 03:17:26 GMT
COPY dir:66cfc1773e07dead4d108eefca05e38bbe528aec6797deefc0559c5a4d41e721 in /opt/java/openjdk 
# Thu, 07 Sep 2023 03:17:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:17:27 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 03:17:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 03:17:27 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 03:17:33 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 03:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 03:17:33 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 03:18:21 GMT
RUN boot
# Thu, 07 Sep 2023 03:18:21 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b481a024ba4d33f0e597e2fced4d71eab6fc3c8ebf663470405837b953224`  
		Last Modified: Thu, 07 Sep 2023 03:29:35 GMT  
		Size: 103.6 MB (103585059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e601bd1503c340453d6905568d706c5bfb74165c27af7cfce79239d4efc5f93`  
		Last Modified: Thu, 07 Sep 2023 03:29:27 GMT  
		Size: 2.4 MB (2362150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a76cb88a9f95dca551722a92b74dce4529bb21d959432c61b32085dd732e21`  
		Last Modified: Thu, 07 Sep 2023 03:29:30 GMT  
		Size: 58.8 MB (58820932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a11a05416d9ae35329db569c1082b93831a15962a1e1f0740305b1c4ff2ef7a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217567307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34b07d60f05a9d5deb38895320a8b3d2f83cc7c8622ef99e5f52e65fd344f4cf`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:03:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 09:03:53 GMT
COPY dir:b83f0a0f236c1f97de459c8ae266f437d3630abb3700f3b868301c8fe017c49a in /opt/java/openjdk 
# Thu, 07 Sep 2023 09:03:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 09:03:55 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 09:03:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 09:03:55 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 09:04:01 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 09:04:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 09:04:01 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 09:04:25 GMT
RUN boot
# Thu, 07 Sep 2023 09:04:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c9b10898343ff844fa6dfe6448ebad584c5b03b783f81be4ce715ad2b88b1b`  
		Last Modified: Thu, 07 Sep 2023 09:14:27 GMT  
		Size: 102.7 MB (102690511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dda039e2bb980fb309b859d6bd77e0ca131c6961eea402ca81384c316da3038`  
		Last Modified: Thu, 07 Sep 2023 09:14:20 GMT  
		Size: 2.4 MB (2351460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1001eb63f095a0e8b8610f55366ea75cb903596bc76962244fac68c74a6f0e6d`  
		Last Modified: Thu, 07 Sep 2023 09:14:23 GMT  
		Size: 58.8 MB (58820620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
