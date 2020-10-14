## `clojure:openjdk-16-boot-buster`

```console
$ docker pull clojure@sha256:510e96984dabb724c96a54cb391886b16822ad2c6675dee190af8ede7f9dff51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f975bf600eeea7b3b12be8b657835f0b86abb3aa8e5a45029a00290e6bd726e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.4 MB (389432964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc4a5bf4bab719f5a7b228228c7bc736e2c7ff0838c8ddbbc9ab0a1a2081228`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:14:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:15:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:38 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 08:57:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 13 Oct 2020 08:57:38 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 08:57:40 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 13 Oct 2020 08:57:40 GMT
ENV JAVA_VERSION=16-ea+19
# Tue, 13 Oct 2020 08:58:24 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-aarch64_bin.tar.gz; 			downloadSha256=9e7094e0dcba61b6b8111f48934cb7395e6dafb1d1ddea7d2296cb0872d67d66; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-x64_bin.tar.gz; 			downloadSha256=487e44f1ec92106437a96f8af07a83ac314dee51dfd46838c23657e550bc616f; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 08:58:24 GMT
CMD ["jshell"]
# Wed, 14 Oct 2020 05:38:31 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 14 Oct 2020 05:38:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 14 Oct 2020 05:38:31 GMT
WORKDIR /tmp
# Wed, 14 Oct 2020 05:38:32 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Wed, 14 Oct 2020 05:38:32 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 14 Oct 2020 05:38:32 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 14 Oct 2020 05:38:52 GMT
RUN boot
# Wed, 14 Oct 2020 05:38:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c41d0463bc77661fb3343235b16d536a92d2efb687046164d413e51bd4fc4`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 7.8 MB (7811737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275efcd805f9905d7def23603618236284b0be6b9e47455c638fbfb03fa9208`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 10.0 MB (9996326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751620502a7a2905067c2f32d4982fb9b310b9808670ce82c0e2b40f5307a3ee`  
		Last Modified: Tue, 13 Oct 2020 02:28:53 GMT  
		Size: 51.8 MB (51829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f28f646e98144707f2cc19e3ad498b86228306ce9f907e555f8f055d690dd1`  
		Last Modified: Tue, 13 Oct 2020 09:07:43 GMT  
		Size: 13.9 MB (13920357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c897a95d35d1447da4697256d475f3b6e2e93937ff0cadb54fb8553540c76c`  
		Last Modified: Tue, 13 Oct 2020 09:07:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e6382a5be58742c613ca3789ded679e36e795c50b5cee335fe31fdd39b84d9`  
		Last Modified: Tue, 13 Oct 2020 09:07:59 GMT  
		Size: 196.7 MB (196651954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b42bdb6df1318168f5b3975b7797f1e7c7198de2a874dea13aeac8cc62776f1`  
		Last Modified: Wed, 14 Oct 2020 05:47:57 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803421c92f6f4233dbd0e35ff5ccd068f1165bce7f66bef473987ed6f89aff8d`  
		Last Modified: Wed, 14 Oct 2020 05:48:01 GMT  
		Size: 58.8 MB (58820013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
