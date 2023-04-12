## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:cd9191d38b35b03ee139ca975b7c45392c55b1dcd768f180daf251ad7acf53e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:d2e3c6de642db663444c8f212e86a57ba76ff510ebcfc065fc593a0cb91babb9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170870487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b0913cd513839fbd036d5141d5d27917c4a2630ba13125c0aad1bc6f33204`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:10:45 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:10:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:10:46 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 08:10:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:10:46 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:10:52 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 08:10:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:10:52 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 08:11:15 GMT
RUN boot
# Wed, 12 Apr 2023 08:11:15 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f23dfc47bb9afbaa36915a5fef9b6f3bddb83e03aa5406397747d7988f783`  
		Last Modified: Wed, 12 Apr 2023 08:21:27 GMT  
		Size: 54.6 MB (54635570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c4433f8d8f2b217ac83a5b2e4ec534aea408b60deda130f2f39346c069ccc8`  
		Last Modified: Wed, 12 Apr 2023 08:21:20 GMT  
		Size: 2.4 MB (2361610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d43c42d2676ec072ac212ad248f5cc3382dcb739dd90b0f50580d7d5e621421`  
		Last Modified: Wed, 12 Apr 2023 08:21:23 GMT  
		Size: 58.8 MB (58820571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4cf274344e9842496936770cf37810b67d7aaa31037caafa966ac2bd5d838054
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168605509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5e4395e67be1dbc17339a2b440757307205f6b3d3925dc7b55fa515e19d423`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:18:07 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:18:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:18:08 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 01:18:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:18:08 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:18:13 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 01:18:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:18:13 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 01:18:43 GMT
RUN boot
# Wed, 12 Apr 2023 01:18:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77229bf38387a79e392fbb99c62cf0fd3217ddff780898642fd3b9455fcd5530`  
		Last Modified: Wed, 12 Apr 2023 01:27:57 GMT  
		Size: 53.7 MB (53727903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69ada62ed0cd7f04cf989aa4a7a005b75c66716657268bdfb678a68634e541a`  
		Last Modified: Wed, 12 Apr 2023 01:27:53 GMT  
		Size: 2.4 MB (2351057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00397887f82b213a7948790ce163a7571b77c2e5c4e6ba88cb66c904025e0c52`  
		Last Modified: Wed, 12 Apr 2023 01:27:55 GMT  
		Size: 58.8 MB (58821020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
