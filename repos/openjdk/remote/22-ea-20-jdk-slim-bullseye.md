## `openjdk:22-ea-20-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:4d0720f071a594842a0f42624ee475a594a6bb226c82eccbfecb25bbdc353d0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:22-ea-20-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:076ad6a0fc66b27ff74eab496ba24afb5d3f58ceec3825801ddb33df95d204ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235489206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80b5858a533ad672da560f8845f1a2c0a7bae55c5342007988ee6d6d103cb0b3`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:50:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 11 Oct 2023 22:50:55 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:50:55 GMT
ENV LANG=C.UTF-8
# Fri, 20 Oct 2023 23:59:45 GMT
ENV JAVA_VERSION=22-ea+20
# Sat, 21 Oct 2023 00:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='5f1627efa81951307900954bbf7b2e49d8c5303615cf116959c273e9707b0496'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='8fa022a3b05cc606bccbb014baea9e821954a789ba40b6fd39b40cd4453fb9f5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 21 Oct 2023 00:00:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f730b1d8252d43d9f960a724f9763804c245215a614762e839fb4b06c2c33bf`  
		Last Modified: Wed, 11 Oct 2023 22:53:31 GMT  
		Size: 1.6 MB (1567906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504458b747a27ac5fb35de30100df93a0ae35085ebef89f001a8b7398753b143`  
		Last Modified: Sat, 21 Oct 2023 00:06:49 GMT  
		Size: 203.9 MB (203857214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
