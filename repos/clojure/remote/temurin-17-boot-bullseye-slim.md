## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:8901bdce7151553e924a4e2f2a07fa1215a0acb8bb36373396baaf4299bdbddf
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
$ docker pull clojure@sha256:007b89247b8b1faa5a7c7d5731ac95694034e287f4936fe0ec13154fd0a2a0e8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281162984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80f35e39bc4a867d9ed103f6429d239d20140295775207256132181545d396f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:49:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 15 Nov 2022 05:54:33 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Tue, 15 Nov 2022 05:54:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 05:54:38 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 15 Nov 2022 05:54:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 15 Nov 2022 05:54:38 GMT
WORKDIR /tmp
# Tue, 15 Nov 2022 05:54:42 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 15 Nov 2022 05:54:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 15 Nov 2022 05:54:42 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 15 Nov 2022 05:54:59 GMT
RUN boot
# Tue, 15 Nov 2022 05:54:59 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 15 Nov 2022 05:54:59 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 15 Nov 2022 05:54:59 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0032fd948a5495fec37e26e9d086c7c0fa24d0623f43f8ad0471aac3350e5f61`  
		Last Modified: Tue, 15 Nov 2022 06:05:10 GMT  
		Size: 191.2 MB (191215234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd82123c314640caf9ef70a6ff9cbd22dbab52e98b8e3d189af14846e2c7dbf9`  
		Last Modified: Tue, 15 Nov 2022 06:04:59 GMT  
		Size: 1.1 MB (1066314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f662c395e477b14935738e6eaa21409f06fbe49b5563949f6acc552e7b84c4`  
		Last Modified: Tue, 15 Nov 2022 06:05:02 GMT  
		Size: 58.8 MB (58820433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12376f6ae0880f69c35b83c4c956bf256285e159ff7bd127fbb4c0e78584dd13`  
		Last Modified: Tue, 15 Nov 2022 06:04:58 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
