## `clojure:temurin-19-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:e5b7cda460650176ee6d651533917a915de7836c9c1c60f2810fcf0756d7ecbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a49e618dba367f1ea0841117de578cd7e93d6f6f32fc31a9205b0d1d7262393e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292416041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe4fce2e2a09f8488980b4af42cadcef9794473baad0f23b31f73a959932e83`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:58:15 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:58:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:58:17 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:58:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:58:17 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:58:23 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:58:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:58:23 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:58:41 GMT
RUN boot
# Tue, 06 Dec 2022 01:58:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:58:41 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:58:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f07ccb399757ca2eb22ecfbed8b8e0fe753148c9c99205f4b73d03bcc43ef0d`  
		Last Modified: Tue, 06 Dec 2022 02:09:27 GMT  
		Size: 201.1 MB (201103429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061637c2a8ef138f02b7c0a9e251e5c03d302172c448f8bae60d3a32033a1513`  
		Last Modified: Tue, 06 Dec 2022 02:09:11 GMT  
		Size: 1.1 MB (1078970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fca135a9b513a7ba7e1894685d32ea9e4240ae69cfa636529f54db90a940ba`  
		Last Modified: Tue, 06 Dec 2022 02:09:15 GMT  
		Size: 58.8 MB (58820390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb43be7fe185f5c5855dfccc776038ef4083ae2730a87db80b613cd43e42207`  
		Last Modified: Tue, 06 Dec 2022 02:09:11 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e6f382a83d0a5d868cace48968e47d803bc69a9c73a8d7d8bd4c37e0356aaeb0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289812217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e6ec6de6784fbd7e31de1bff254f4a1b17832eda4d6f3cd6b7355da6e429b1`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:49:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 15 Nov 2022 05:57:11 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 15 Nov 2022 05:57:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 05:57:16 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 15 Nov 2022 05:57:16 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 15 Nov 2022 05:57:16 GMT
WORKDIR /tmp
# Tue, 15 Nov 2022 05:57:20 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 15 Nov 2022 05:57:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 15 Nov 2022 05:57:20 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 15 Nov 2022 05:57:38 GMT
RUN boot
# Tue, 15 Nov 2022 05:57:38 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 15 Nov 2022 05:57:38 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 15 Nov 2022 05:57:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e822da9eb481d8723150163c7ea4b157d85c48d2dde40328d24aac329303d4f`  
		Last Modified: Tue, 15 Nov 2022 06:06:59 GMT  
		Size: 199.9 MB (199864406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a4edf818fac1474574af28a9d0f27152b1f27e4801bfb6b177a0ddd7d8d1e9`  
		Last Modified: Tue, 15 Nov 2022 06:06:47 GMT  
		Size: 1.1 MB (1066317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c3708ef49f2301b2fa8e8df12a68f2aa2eaac3558dfc423aefa01684130eb2`  
		Last Modified: Tue, 15 Nov 2022 06:06:49 GMT  
		Size: 58.8 MB (58820489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3d564a851ae90c2dd5cd017843316a7274acef1a1e07fd239cedf16e912459`  
		Last Modified: Tue, 15 Nov 2022 06:06:46 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
