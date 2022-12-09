## `clojure:temurin-17-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:7abb4495149243e84b519d4ed782496be01a044d3698523ca5ba11de818ac5ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:f8a47faca71f55578c0ce64f519afa75928ec0d09eaf69d93ecaeb9d68e7897e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283743759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c86ceabc33de17499f386d7553e7fdbe535ca7c39c58a69a32fc057d644a6f35`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:42:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:42:09 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 06:42:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 06:42:10 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:42:15 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 06:42:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 06:42:15 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 06:42:33 GMT
RUN boot
# Fri, 09 Dec 2022 06:42:34 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 06:42:34 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 06:42:34 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5f94ae1773704df1e85071e02068cc42f6d82712560e46594b99183adbcea5`  
		Last Modified: Fri, 09 Dec 2022 06:56:53 GMT  
		Size: 1.1 MB (1078949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a83c474018b51c10d435c4e9d157ec074e1dd7ae038acfacfde3b411b973e7`  
		Last Modified: Fri, 09 Dec 2022 06:56:58 GMT  
		Size: 58.8 MB (58820294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a44d65fd61f041354dde0f0ed964270c37fcc505ef166a6175c990aaaef8d5`  
		Last Modified: Fri, 09 Dec 2022 06:56:53 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:78f89db8bb7a0e1b792061fc6696fbea42750e7026eef6288a82574df4626285
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281162898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d6f567dad038bc9fff0842f33a1b6249c1228fa085adc5187704cf9b51a5a49`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:08:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:08:30 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 05:08:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 05:08:31 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:08:35 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 05:08:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 05:08:35 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 05:08:54 GMT
RUN boot
# Fri, 09 Dec 2022 05:08:54 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 05:08:55 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 05:08:55 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213d13a48a5d672da887bdf7fb8911ba631028bf3a1300e8cb9f4a57ccab03c9`  
		Last Modified: Fri, 09 Dec 2022 05:21:24 GMT  
		Size: 1.1 MB (1066327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf187920e09b5f365c4bf6ebb1eda79bc1b84af2609901d36f3317d63dca6631`  
		Last Modified: Fri, 09 Dec 2022 05:21:26 GMT  
		Size: 58.8 MB (58820647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed62bdcd2a680b2c360063a4dc0979719d375a13903b0e99df41cd04e2f1633`  
		Last Modified: Fri, 09 Dec 2022 05:21:23 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
