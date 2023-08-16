## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:58712e7f2ad13f6707d41d1f62c99c6641e00de812397df60ca31ddd42cd1611
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:18b8dea55f34a1c86611f99948ab60904bd7bdde858d7003b85b12fbb94834fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.8 MB (219824564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88f46881718921f5f4dea0becb30c1885c725e6344b4cd72e18a76561015488`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:26:08 GMT
COPY dir:66cfc1773e07dead4d108eefca05e38bbe528aec6797deefc0559c5a4d41e721 in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:26:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 01:26:09 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 01:26:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 01:26:09 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 01:26:15 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 01:26:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 01:26:16 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 01:26:52 GMT
RUN boot
# Wed, 16 Aug 2023 01:26:52 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a5a5971aa40d66285a278288b640fe204504a1357230ee711761ceaf3a5937`  
		Last Modified: Wed, 16 Aug 2023 01:38:52 GMT  
		Size: 103.6 MB (103585023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ce7c772cc10339a5fb60c22ed70eb9c2b4ddea4e154bf6d42f1cccc1c6aeca`  
		Last Modified: Wed, 16 Aug 2023 01:38:43 GMT  
		Size: 2.4 MB (2362172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5f3da9afe48cb6029c48841efe32ef756178747b4df27ea59a41d505c327de`  
		Last Modified: Wed, 16 Aug 2023 01:38:46 GMT  
		Size: 58.8 MB (58820748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6846976e030888d28823b65f9ae8da0f101a580232bad5bb703e4f80168fde42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.6 MB (217567140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4656ce5f46953a4ae7608beaa9b8a07db51c6a643930319e2ed6ef0ca4941e54`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:46:16 GMT
COPY dir:b83f0a0f236c1f97de459c8ae266f437d3630abb3700f3b868301c8fe017c49a in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:46:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 01:46:18 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 01:46:18 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 01:46:18 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 01:46:23 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 01:46:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 01:46:24 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 01:46:42 GMT
RUN boot
# Wed, 16 Aug 2023 01:46:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73e72ffee157aface2093ca7b44ca1e9d7d8010e8b3344c5760c1ae633be3d0`  
		Last Modified: Wed, 16 Aug 2023 01:56:15 GMT  
		Size: 102.7 MB (102690463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b7cda0152fc848681cfcb2e8d7e2d37db6cbf6d054d4d78c77730b6f60e28e`  
		Last Modified: Wed, 16 Aug 2023 01:56:08 GMT  
		Size: 2.4 MB (2351417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff4bd27505dabeddc455a9f49259b9f5b2b7b656f3b871f7f0def2cc5a57a21`  
		Last Modified: Wed, 16 Aug 2023 01:56:11 GMT  
		Size: 58.8 MB (58820481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
