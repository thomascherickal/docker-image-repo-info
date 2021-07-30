## `clojure:openjdk-17-tools-deps-1.10.3.933-buster`

```console
$ docker pull clojure@sha256:ae260bdd59881c5da6a81861759c7547581ccf583305c4f8bc57ea500a52ed9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-17-tools-deps-1.10.3.933-buster` - linux; amd64

```console
$ docker pull clojure@sha256:75df12ea20abd61c942aae73cbd205f4810d54f472d3c5edc3f08ecd0350e556
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.4 MB (348360258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ece2939f2cb2cdc8b9fa7542c789b8c3d406e03e6277bb52d5e1c0c382c4d9`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:34:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Thu, 22 Jul 2021 13:34:05 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:34:05 GMT
ENV LANG=C.UTF-8
# Fri, 30 Jul 2021 18:50:44 GMT
ENV JAVA_VERSION=17-ea+33
# Fri, 30 Jul 2021 18:50:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='d89e04f161553560c454bf263924dc49c5c2529698ef8131baff632355baea18'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='d361654c87bae6712f36d7f0d27914c63fbe31f10a9a0d5316072b3c69ed2263'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 30 Jul 2021 18:50:55 GMT
CMD ["jshell"]
# Fri, 30 Jul 2021 20:22:46 GMT
ENV CLOJURE_VERSION=1.10.3.933
# Fri, 30 Jul 2021 20:22:46 GMT
WORKDIR /tmp
# Fri, 30 Jul 2021 20:22:57 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0559cc25d08c3c25c3c0b734aba3a6c80f9b5d2760fdbddf08a4df886873528e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 30 Jul 2021 20:22:58 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4de66c57277180420b7663842bf72269ceeb8ddb3b87e83d9d5a4b708ac740`  
		Last Modified: Thu, 22 Jul 2021 13:43:09 GMT  
		Size: 13.9 MB (13921248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a3f0accd72bd6538610ea6af71b3cba4d85b33dbff904d77d00feead2b10a6`  
		Last Modified: Fri, 30 Jul 2021 19:00:32 GMT  
		Size: 187.3 MB (187253789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c076a7dd0d5e70f9899096ae4ef6c5615f0383d4ec1ecdf03478370705bde7b`  
		Last Modified: Fri, 30 Jul 2021 20:28:49 GMT  
		Size: 27.1 MB (27078226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
