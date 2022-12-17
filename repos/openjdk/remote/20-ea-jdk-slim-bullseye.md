## `openjdk:20-ea-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:299cdc9439d91a8fe1fac7388dd66d2cc99456ec38281e888af00d51fb784e7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:c5e79e7d958392c5250af28e4e6997d6b45fad693d044b7697ad3400d7d91159
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231461314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa58a796304ccfe4650af848c2bfb449cf44dc08ae25295c4bb6caf459177ff7`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 05:06:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 05:06:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 06 Dec 2022 05:06:08 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 05:06:08 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 23:32:22 GMT
ENV JAVA_VERSION=20-ea+28
# Fri, 16 Dec 2022 23:32:42 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='d7b481073f0135b7862e9867a61f2133012fc7e555c7f04a383004cedcaad316'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='2201e01fa03d9921f68a072ff6175eddef9370d6ecb1b47f2e6dc200f12f0aca'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Dec 2022 23:32:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca06928f532b9db5daaeea1a6cfedc2be5faa3421714209b828baa3f96741b02`  
		Last Modified: Tue, 06 Dec 2022 05:11:13 GMT  
		Size: 1.6 MB (1584014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392c1a1555cd45f77a9d7726762005246aa0a0358641e347cb96b547abcd0e07`  
		Last Modified: Fri, 16 Dec 2022 23:42:13 GMT  
		Size: 198.5 MB (198464448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7b025e2d6ce85f8c7cd57ce0c9b701c41d31eaae1797813323dc1b4e17cf9681
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228586410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cea9e5b76aae855f74e983e340a478bc1c66acabaf6e34fb1771239c6bbfb2`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:27:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:27:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 06 Dec 2022 04:27:21 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 04:27:21 GMT
ENV LANG=C.UTF-8
# Sat, 17 Dec 2022 00:28:08 GMT
ENV JAVA_VERSION=20-ea+28
# Sat, 17 Dec 2022 00:28:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='d7b481073f0135b7862e9867a61f2133012fc7e555c7f04a383004cedcaad316'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='2201e01fa03d9921f68a072ff6175eddef9370d6ecb1b47f2e6dc200f12f0aca'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 17 Dec 2022 00:28:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e352a64899d702442b046fd5b4919ea4eef3df76860668bc610c2162af8eec`  
		Last Modified: Tue, 06 Dec 2022 04:32:15 GMT  
		Size: 1.6 MB (1567461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bcbcac9c058257c83744432809c4b9375b8d3d3ad266ed6e87fc971149ce6f`  
		Last Modified: Sat, 17 Dec 2022 00:37:38 GMT  
		Size: 197.0 MB (196958629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
