## `openjdk:20-ea-26-slim-bullseye`

```console
$ docker pull openjdk@sha256:ef87764f4990d2a4e93cbd44c0962d4ec775b032a84e6fb2bad51c5ebbe5542d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-26-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:0851f5fc26264aa6f85267ca24c128bc1e8089ca8f6c15fdaf64a56728177dc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231323252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b754ab4a00f8b88c093ebed8530fba91dd923ef2bad187052fec9ccba683b94f`
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
# Tue, 06 Dec 2022 05:06:08 GMT
ENV JAVA_VERSION=20-ea+26
# Tue, 06 Dec 2022 05:06:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 06 Dec 2022 05:06:23 GMT
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
	-	`sha256:60f647c9faca97b557bc6162ad57f441301e0ad32964fd7f8112e7254802da9c`  
		Last Modified: Tue, 06 Dec 2022 05:11:28 GMT  
		Size: 198.3 MB (198326386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-26-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:a1d85f8f57bd100b832cb666a17cd6884d18a5b4f2e4d4eaa2cfec0bc8d6571c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.5 MB (228503094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1be3e6e6cb7bc65114b5450b842281e68e4bfbd8f525304ce50536397caad0d`
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
# Tue, 06 Dec 2022 04:27:21 GMT
ENV JAVA_VERSION=20-ea+26
# Tue, 06 Dec 2022 04:27:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 06 Dec 2022 04:27:33 GMT
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
	-	`sha256:d00e19b093591ab940d7787b53407016be6abf0b5ddc632d60f67b4b3b8979c9`  
		Last Modified: Tue, 06 Dec 2022 04:32:27 GMT  
		Size: 196.9 MB (196875313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
