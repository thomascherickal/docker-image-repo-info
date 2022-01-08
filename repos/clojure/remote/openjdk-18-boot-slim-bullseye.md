## `clojure:openjdk-18-boot-slim-bullseye`

```console
$ docker pull clojure@sha256:0f382af6231aab84a0c2c6a64eec90ace767ca41d63bd7403c1fa78d1fc6d4c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:00cab96846eb2644eed6516550c67404f5144e15869cd3f48c4ea73180f3244c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281056998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8964ceeb1849fb168c5979fec7bca077d03a5ee0191d433e9f8664efe590c54`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:57:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 22:59:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 21 Dec 2021 22:59:22 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 22:59:22 GMT
ENV LANG=C.UTF-8
# Sat, 08 Jan 2022 00:32:44 GMT
ENV JAVA_VERSION=18-ea+30
# Sat, 08 Jan 2022 00:33:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='4e34f307a3d9b1c020a864e863a0f47c701036592d634da55c6e548d101526ed'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='10fd6ab1369a4cd536570c4cccfd2aead86bfd733fd7171de74e0b979c04b96e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 08 Jan 2022 00:33:02 GMT
CMD ["jshell"]
# Sat, 08 Jan 2022 01:17:41 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 08 Jan 2022 01:17:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 08 Jan 2022 01:17:42 GMT
WORKDIR /tmp
# Sat, 08 Jan 2022 01:17:46 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 08 Jan 2022 01:17:47 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 08 Jan 2022 01:17:47 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 08 Jan 2022 01:18:13 GMT
RUN boot
# Sat, 08 Jan 2022 01:18:14 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 08 Jan 2022 01:18:14 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 08 Jan 2022 01:18:14 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbde5250315969db657b55bd8b2f5507fb659c0cf7f135edc84b684ffeab44a`  
		Last Modified: Tue, 21 Dec 2021 23:14:38 GMT  
		Size: 1.6 MB (1582039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f0ca5cc42a2cc308a396f6c08f7604c421a9c79e41c983be4e382ceab8e73a`  
		Last Modified: Sat, 08 Jan 2022 00:52:05 GMT  
		Size: 189.0 MB (189013452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea884ae37d49619b454c76e3cf89943eb18b4eb040359c780cc0c172c67fbfef`  
		Last Modified: Sat, 08 Jan 2022 01:27:02 GMT  
		Size: 283.1 KB (283059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0644ca0f5d89dd1badddd33f10b06ddb86fabd29a946b6d740934f522124a6`  
		Last Modified: Sat, 08 Jan 2022 01:27:05 GMT  
		Size: 58.8 MB (58820418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef406c706679e03561e475b3c10c8d31ab6e979ada54c28084b0e56f6429e5`  
		Last Modified: Sat, 08 Jan 2022 01:27:02 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:579efec945cf67659e0a7fd50e4e448884dafc32d9f8414658d225893b3baef3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.2 MB (278226901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9d478d9aa06e46ea719b65116b2da6ca16f7f19cb16bd7276201fa94ed8922`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:53:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:55:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 21 Dec 2021 02:55:51 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:55:52 GMT
ENV LANG=C.UTF-8
# Sat, 08 Jan 2022 00:53:59 GMT
ENV JAVA_VERSION=18-ea+30
# Sat, 08 Jan 2022 00:54:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='4e34f307a3d9b1c020a864e863a0f47c701036592d634da55c6e548d101526ed'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='10fd6ab1369a4cd536570c4cccfd2aead86bfd733fd7171de74e0b979c04b96e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 08 Jan 2022 00:54:13 GMT
CMD ["jshell"]
# Sat, 08 Jan 2022 01:45:44 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 08 Jan 2022 01:45:44 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 08 Jan 2022 01:45:45 GMT
WORKDIR /tmp
# Sat, 08 Jan 2022 01:45:50 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 08 Jan 2022 01:45:50 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 08 Jan 2022 01:45:51 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 08 Jan 2022 01:46:08 GMT
RUN boot
# Sat, 08 Jan 2022 01:46:09 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 08 Jan 2022 01:46:09 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 08 Jan 2022 01:46:10 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3380d13c6c3ddd0cc31ece5496ad1481500cb07b7feb31c81bc907a9a1ad71`  
		Last Modified: Tue, 21 Dec 2021 03:15:59 GMT  
		Size: 1.6 MB (1565954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f85cf79811e7fe57b773af7d072032636ad02721bb4d40554fee33038b6c41a`  
		Last Modified: Sat, 08 Jan 2022 01:13:06 GMT  
		Size: 187.7 MB (187733604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e698594b7d864fda4a4f4ac60d50f1cbf335fcf36bba708f894d71b77be40f30`  
		Last Modified: Sat, 08 Jan 2022 01:55:58 GMT  
		Size: 67.2 KB (67227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdd2de8ea7e2e3cf6fe648fea46cc58be9f5d715553f1283f7ae06badb0bc8c`  
		Last Modified: Sat, 08 Jan 2022 01:56:05 GMT  
		Size: 58.8 MB (58815919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e6ea56bec1b0c0b56c92df65e7e79ed4e28ed8df1538a3a5d22f72a1a9bee9`  
		Last Modified: Sat, 08 Jan 2022 01:55:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
