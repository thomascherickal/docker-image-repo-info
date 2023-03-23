## `clojure:temurin-8-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:38e62a4fc5914b1fff269d8cc26d56fd65bca6963545fd31b5da437b177c2ee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:7867bf8807ac92b7d761888cbbed4dc5f335821b372ba21411c079bd78b1910d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170863475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb424d3cca19da319b2de290a57c37efaca375a6865c06e8894997b01425559f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:16:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:17:00 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:17:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:17:01 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:17:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:17:01 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:17:06 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:17:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:17:07 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:17:37 GMT
RUN boot
# Thu, 23 Mar 2023 06:17:38 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5629480cb1323c2f01db8609391416fe9380f0b3fc3c8da30bdfaf6c963d0c`  
		Last Modified: Thu, 23 Mar 2023 06:29:13 GMT  
		Size: 54.6 MB (54635545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1407e444e98c37386fdf3fca3f50a789ba69be7685c5e11cecfb9753ecde1420`  
		Last Modified: Thu, 23 Mar 2023 06:29:07 GMT  
		Size: 2.4 MB (2361567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efe9fc4970a55d8d9c9fd53ea16e20248284e131811779b5b69d6fa669f7ffe`  
		Last Modified: Thu, 23 Mar 2023 06:29:10 GMT  
		Size: 58.8 MB (58820755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a79758942846336f443655bd53e16807fefbc82c65d5acba7d5518e2a0dd25c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168602348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b1573d52d32695837dc6cd69792b4f1d28c3dcd7bec50cc4b5c6a20340d010`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:52:13 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:52:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:52:14 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:52:14 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:52:14 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:52:19 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:52:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:52:19 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:52:37 GMT
RUN boot
# Thu, 23 Mar 2023 06:52:37 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db05ddb8bb6879c9a35043060daf1e3be2ff6486c8fdb3f0f54e8240f31ac24`  
		Last Modified: Thu, 23 Mar 2023 07:02:31 GMT  
		Size: 53.7 MB (53727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b8b4e794983470307c6837a456788804d6571d12d409fee14dff942708e11d`  
		Last Modified: Thu, 23 Mar 2023 07:02:27 GMT  
		Size: 2.4 MB (2350880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff290176070d6c6d77a480dead728d27b50b883f11b8b1c7268ad4e9bc459c26`  
		Last Modified: Thu, 23 Mar 2023 07:02:29 GMT  
		Size: 58.8 MB (58820447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
