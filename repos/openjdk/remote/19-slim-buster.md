## `openjdk:19-slim-buster`

```console
$ docker pull openjdk@sha256:202cc59341112e656388d6685d016c006a42d4d48c349d6302c18a4d304a0448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:30cc96399eaf8e2bcb123c14c1d93e45a5c18ac772c47f5680bf7abb67254be1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.5 MB (225544495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb263b2f9bff148ae8049ef131c743dc2662752d837a023183b377aae779866`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:47:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:47:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 05:47:35 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:47:35 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:47:35 GMT
ENV JAVA_VERSION=19-ea+21
# Wed, 11 May 2022 05:47:48 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 11 May 2022 05:47:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9930d1f61e9a044df90a13c9456f95b2e6b31da0c5f483757324dfe0a5fc33`  
		Last Modified: Wed, 11 May 2022 05:59:57 GMT  
		Size: 3.3 MB (3273265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f776361c6af6943ccb8cc9ab9d55f85ce7be88c405a4081631f284c13bf4e0`  
		Last Modified: Wed, 11 May 2022 06:00:11 GMT  
		Size: 195.1 MB (195130508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:14c8a982a3479817bba77b1e42994dff6074c321763bcaf7fdd210822c1c0c86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.8 MB (222806272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caabc5042b3bc9a8118a7b355bb25940b82ac732eec90dfc48ae616776133941`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:16:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:16:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 14:16:58 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:16:59 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:17:00 GMT
ENV JAVA_VERSION=19-ea+21
# Wed, 11 May 2022 14:17:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 11 May 2022 14:17:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ef35bf9af0d08f4a170567ffeb4f2374230da90c85eec67344eb6c8994306b`  
		Last Modified: Wed, 11 May 2022 14:35:37 GMT  
		Size: 3.1 MB (3125755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bdced7bb7c1d123f1b7ff6b37f3f176d23c2821ad419eb9859a5d7174e076a`  
		Last Modified: Wed, 11 May 2022 14:35:53 GMT  
		Size: 193.8 MB (193771503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
