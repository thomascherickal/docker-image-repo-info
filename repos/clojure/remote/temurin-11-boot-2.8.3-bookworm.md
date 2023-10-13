## `clojure:temurin-11-boot-2.8.3-bookworm`

```console
$ docker pull clojure@sha256:0001b48fb9d0fd798f0cccb7c40af711c0c95f4cc8d44d019cf9513b80403a2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bookworm` - linux; amd64

```console
$ docker pull clojure@sha256:e0459541afc131e8799d4a0e3e827e8d045f965b0c5d238fd6b849aded570270
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258761484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d7e949428d1c922f56e0bb5b81f94943f6e8bb5095da459544e4db9e7ffd996`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:26:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:43:54 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:43:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:43:55 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 13 Oct 2023 12:43:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 12:43:56 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:44:03 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 12:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 12:44:04 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 13 Oct 2023 12:44:22 GMT
RUN boot
# Fri, 13 Oct 2023 12:44:22 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312f54f99658b0b7990d26fe3799c0af7d535f77af55acd1d748d19013cad478`  
		Last Modified: Fri, 13 Oct 2023 13:04:52 GMT  
		Size: 144.8 MB (144826232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356eb8950d12eca27dd6682b64d9cb6c294f89f05315d0e98b68513e6bc5cd40`  
		Last Modified: Fri, 13 Oct 2023 13:04:41 GMT  
		Size: 5.5 MB (5532644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a568755b89c78bec1cd457255b45231986bf53fe2db186767ed7cf6003ab069`  
		Last Modified: Fri, 13 Oct 2023 13:04:45 GMT  
		Size: 58.8 MB (58820384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bookworm` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cc6123846329a8286a91d7fd7ec29b5fa741e4d653c42e10e861c61e764e4894
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255358950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1b7c3867398a248ff2a2a4269f2bd09b323073cf54314d714709141ecf4449`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 00:57:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:12:02 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:12:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:12:05 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 13 Oct 2023 10:12:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 10:12:05 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:12:11 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 10:12:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 10:12:12 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 13 Oct 2023 10:12:28 GMT
RUN boot
# Fri, 13 Oct 2023 10:12:28 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf03c8b0dce1ee3013ef26db39e3fea7b1e7c57443f42116088217a57392c8`  
		Last Modified: Fri, 13 Oct 2023 10:29:26 GMT  
		Size: 141.6 MB (141570586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80132fc81a7508d6ba991bf10f983d43b31aed6f346680ff5310bc72037aaf1`  
		Last Modified: Fri, 13 Oct 2023 10:29:15 GMT  
		Size: 5.4 MB (5355512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cd18bd320f1a83c3f74c2bab5b5facc6b14605edc6b13aeb5a46d7721a222e`  
		Last Modified: Fri, 13 Oct 2023 10:29:19 GMT  
		Size: 58.8 MB (58820274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
