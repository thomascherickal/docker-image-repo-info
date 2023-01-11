## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:ce791f33930f530c057782ee1b0a1467803997dfdadfbbf356d92fc84fac929e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:ab9a151b910807b9a3fb98d915cbb7772e8acdf12b3a2ea69f28817769424862
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283726466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91d27e8f70e59abec71239ab143053e9a05c9fc5d4e578380deb294e400caa0d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:26:17 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:26:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:26:19 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:26:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:26:19 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:26:25 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:26:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:26:25 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:26:44 GMT
RUN boot
# Wed, 11 Jan 2023 03:26:45 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:26:45 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:26:45 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d96920cde608b8c4fa7937cb3a26411ad5c2a11f9476a38a3695c1d8ad93cd3`  
		Last Modified: Wed, 11 Jan 2023 03:38:36 GMT  
		Size: 192.4 MB (192431265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a121d6d1d3e3e9e84146bc3305c7945e6cb0270a5cda59dd24b2e7055cc8c28`  
		Last Modified: Wed, 11 Jan 2023 03:38:21 GMT  
		Size: 1.1 MB (1077360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777ca3925e21ea67ef31ed7b2f09af674dbbac298caccef00c7101559de0841d`  
		Last Modified: Wed, 11 Jan 2023 03:38:25 GMT  
		Size: 58.8 MB (58820470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec75fea1138f0f275b4914119df875787c47a12422c0a75c99fb227448379bc`  
		Last Modified: Wed, 11 Jan 2023 03:38:21 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2968b4638df961a56d8c13d94da19cdc884f7e280513bba4517698d37a725578
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281145725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1cc8a8c6f4b360642ade1e15e3ae982c7a25d684da261ce64fc8fd3d8145d40`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:43:55 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:44:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:44:00 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:44:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:44:00 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:44:04 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:44:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:44:04 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:44:22 GMT
RUN boot
# Wed, 11 Jan 2023 03:44:22 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:44:22 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:44:22 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af213950f8cc63689dbc3db5e95e2955b9c5a24f79594f3d9716eec20e2bb23`  
		Last Modified: Wed, 11 Jan 2023 03:54:33 GMT  
		Size: 191.2 MB (191215202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348c0592c408bf9c58ac3fbec8906241b8d04d951c38692e9dbaa64013df93e3`  
		Last Modified: Wed, 11 Jan 2023 03:54:22 GMT  
		Size: 1.1 MB (1064703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595345df8fb6070c9f11ec69bd43518deda5a2716885a89f721cdf33e93d97b`  
		Last Modified: Wed, 11 Jan 2023 03:54:25 GMT  
		Size: 58.8 MB (58820605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce96d0e1fc14d476d0d38813cb7eb86d87d080965ed9a525d4c13b04e8e62be8`  
		Last Modified: Wed, 11 Jan 2023 03:54:21 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
