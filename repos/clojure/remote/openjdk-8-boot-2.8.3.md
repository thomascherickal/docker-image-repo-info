## `clojure:openjdk-8-boot-2.8.3`

```console
$ docker pull clojure@sha256:25a209b339c5a44255b1c926e4778a42dd16dab987b1be9347e9e8e52629d61c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-8-boot-2.8.3` - linux; amd64

```console
$ docker pull clojure@sha256:cf339b10b9a0bb7fef15dc59cca8426d67114f760fe916574d2d2b8135e5ff08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.6 MB (278570228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328d13ebbab28e4ac4e8901f230b48a791fa47caf8d1e1155ae68031f3aca638`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:33:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:34:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:26:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:26:12 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:28:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sun, 02 Feb 2020 06:28:14 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:28:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:28:16 GMT
ENV JAVA_VERSION=8u242
# Sun, 02 Feb 2020 06:28:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_
# Sun, 02 Feb 2020 06:28:16 GMT
ENV JAVA_URL_VERSION=8u242b08
# Sun, 02 Feb 2020 06:28:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sun, 02 Feb 2020 21:32:33 GMT
ENV BOOT_VERSION=2.8.3
# Sun, 02 Feb 2020 21:32:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:32:34 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 21:32:35 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sun, 02 Feb 2020 21:32:35 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 21:32:35 GMT
ENV BOOT_AS_ROOT=yes
# Sun, 02 Feb 2020 21:33:46 GMT
RUN boot
# Sun, 02 Feb 2020 21:33:46 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c160265e75550c2ed099aa7d3906b3fef0bf046a2aeead136f8e587a015159`  
		Last Modified: Sun, 02 Feb 2020 00:42:04 GMT  
		Size: 10.8 MB (10797219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4fe40d0e618e3319afb689c3570bb87e8e8cf51bca080364d1552317bc66c2`  
		Last Modified: Sun, 02 Feb 2020 00:42:02 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d647f502a07e6daaee43c23cfac9399501b1d7f55fb4c60d56307e23f0ed5a5`  
		Last Modified: Sun, 02 Feb 2020 00:42:26 GMT  
		Size: 50.1 MB (50073989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d108b8c498aa300c0375abb3c74caebbf95e7ed768f49b1028fd6ace22e98051`  
		Last Modified: Sun, 02 Feb 2020 06:35:11 GMT  
		Size: 4.9 MB (4935305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe918b8aa55b28acf6af7bb7e304acad59e87ad62d32f363690cd9cde40dee`  
		Last Modified: Sun, 02 Feb 2020 06:36:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafa1a7c0751f833dd37aa9f280cdb697e1231a2a08909a72b05c7f002907e54`  
		Last Modified: Sun, 02 Feb 2020 06:37:17 GMT  
		Size: 104.2 MB (104214689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79b41ddac58442fccd1f83ce480cac970a35220b0ab02dddaf161766399c96e`  
		Last Modified: Sun, 02 Feb 2020 21:47:19 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf05a68895a2cc4c62bf722ddb80eded9f6c55c9f94fc085124446a335cd3dae`  
		Last Modified: Sun, 02 Feb 2020 21:47:25 GMT  
		Size: 58.8 MB (58821241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
