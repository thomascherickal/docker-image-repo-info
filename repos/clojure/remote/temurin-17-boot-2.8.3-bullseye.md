## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:542cfd246b2fc4d08da39cc472537aba01386b40e590b485d86bdea72c061b1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:5a644a3eaafa783a5fad538e5196770ffb768d12e3124ec8cb37e843c8381b18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308638032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4c411b45a8ff0d4c590212fc8decd290ea9c4d2d6fbc2381cdd240ec30b9f5c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:25:39 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:25:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:25:40 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:25:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:25:41 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:25:47 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:25:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:25:47 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:26:06 GMT
RUN boot
# Wed, 11 Jan 2023 03:26:06 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:26:06 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:26:06 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2359afb593c01bca1799fd29c2d98e1da243e75a77e88c13d9c01c99d2d6472b`  
		Last Modified: Wed, 11 Jan 2023 03:38:12 GMT  
		Size: 192.4 MB (192431213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c8c4e7fb3237fb2b61f0dbf4078ab816bdec49e18f50f5c5b849bb0d0d9a05`  
		Last Modified: Wed, 11 Jan 2023 03:37:58 GMT  
		Size: 2.4 MB (2360651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c1c5c65beacbbff5f4b8ec727aa5dbbc1cf065073d5a8857f1330cdf9f67a1`  
		Last Modified: Wed, 11 Jan 2023 03:38:01 GMT  
		Size: 58.8 MB (58820563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31da7bf719fbe5315141ddfa2513362e8292bbb766e2a7307a10ee5f8350627b`  
		Last Modified: Wed, 11 Jan 2023 03:37:58 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f6558d2af63bd431cedcfc0e1e9c271c0642622c55b3037c33906d6e14db0876
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306068489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44431517a0d8a60ab552436cb9ae4ee02fba52186e2ef14daffabb2b87a7147e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:43:23 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:43:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:43:27 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:43:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:43:27 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:43:32 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:43:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:43:32 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:43:50 GMT
RUN boot
# Wed, 11 Jan 2023 03:43:50 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:43:51 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:43:51 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed584d0f78d42904a7174ba2f0094e605937d56b96a16d626892c244e836746`  
		Last Modified: Wed, 11 Jan 2023 03:54:13 GMT  
		Size: 191.2 MB (191215212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4fed853213aa9a75cf4e588f00f38a5ccb5f15ac1ffdb99f52bc06a08c1a18`  
		Last Modified: Wed, 11 Jan 2023 03:54:02 GMT  
		Size: 2.4 MB (2350596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31abbfcbe88a46230e07a1e87c48c65072e56c7c060f666444062573cd0dd2`  
		Last Modified: Wed, 11 Jan 2023 03:54:04 GMT  
		Size: 58.8 MB (58820423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414180cce49993fde25e89c4a5feb5bdc81a83bd5e59fd02d7ff1c296cb1a797`  
		Last Modified: Wed, 11 Jan 2023 03:54:01 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
