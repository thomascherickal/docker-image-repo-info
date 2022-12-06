## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:318e11c4ac594b718707f814d9c7a44ab1044933860be5814dd5db373590ba3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:005cb3de38de23188b29a6d1600d26446135227554c107091d1efe49252e16cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283743801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f710a73b37eaae1ea2a4a15200386af8dd6b5d902cc84690d92c886fe316af1e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:55:16 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:55:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:55:18 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:55:18 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:55:18 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:55:23 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:55:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:55:24 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:55:41 GMT
RUN boot
# Tue, 06 Dec 2022 01:55:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:55:41 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:55:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0e3c2c64e722c7da74f92591596ff13f3ffe19cede0e89102f3c4d99a86eec`  
		Last Modified: Tue, 06 Dec 2022 02:07:22 GMT  
		Size: 192.4 MB (192431246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615f7f21f6b93bd26b7ace89a833041cd9dd947e107f019b00a6d6736a7495cf`  
		Last Modified: Tue, 06 Dec 2022 02:07:08 GMT  
		Size: 1.1 MB (1078938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e70fe9080491ddb5c209a4cd6cba5faa768581ce4dc81cacd3788c6bf71ee70`  
		Last Modified: Tue, 06 Dec 2022 02:07:12 GMT  
		Size: 58.8 MB (58820365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e28ee94605c475b21eff0bef291835fc7ec928bc3756fd584a69aa6c48af339`  
		Last Modified: Tue, 06 Dec 2022 02:07:07 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b2b3c940ccaa3fe72fdb42728db734e5d76468a42b51e7a742a218eabdcad82a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281162583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ab8f7be3730ff4824f1e2c3f650d4ca22799f06c255a1d5810fc554a8de807f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:22:53 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:22:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:22:57 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:22:57 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:22:57 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:23:02 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:23:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:23:02 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:23:19 GMT
RUN boot
# Tue, 06 Dec 2022 02:23:19 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:23:19 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:23:19 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838b5f3398d789eb4642eff775295a017b51ac8034f8a4c2f4ed800e7a30d07`  
		Last Modified: Tue, 06 Dec 2022 02:33:34 GMT  
		Size: 191.2 MB (191215233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b0e3e838f00d06977db3125d4fc971237c57415f5951f4f2a4770819a5af294`  
		Last Modified: Tue, 06 Dec 2022 02:33:22 GMT  
		Size: 1.1 MB (1066320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adbfc4f81533519c9397432af4fe0246caa52759c2d1819f12b462f8cf07b05`  
		Last Modified: Tue, 06 Dec 2022 02:33:25 GMT  
		Size: 58.8 MB (58820311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed3ca43adeac558af32b01d23b5d90d7245cec892b702a537e232d9ed55ee60`  
		Last Modified: Tue, 06 Dec 2022 02:33:22 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
