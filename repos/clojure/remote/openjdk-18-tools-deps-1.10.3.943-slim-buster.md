## `clojure:openjdk-18-tools-deps-1.10.3.943-slim-buster`

```console
$ docker pull clojure@sha256:cdc37a8a5df022da027ca4b16250199d3209d2f426164e8dea0c5d002499e123
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-1.10.3.943-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:437ad569db5c9f74c694c2d9f6ab9ecd371b0d18799e2effae36dc7333c36f60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.7 MB (256731829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4838c05208537fb6c8858b7d733a5eb0ee215db1b942e5870087acc797955fe3`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:53:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 17 Aug 2021 06:53:11 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:53:11 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 17:32:05 GMT
ENV JAVA_VERSION=18-ea+12
# Fri, 27 Aug 2021 17:32:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='a9bc316abb2e03378f35fc574685b8bbdd15cd6803df70c02e71ff8f19ad292b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='08129b3c4ef9956a14a7112565a185ac9ea7e3b327875089114ce6fe2563f585'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 27 Aug 2021 17:32:19 GMT
CMD ["jshell"]
# Sat, 28 Aug 2021 01:25:56 GMT
ENV CLOJURE_VERSION=1.10.3.943
# Sat, 28 Aug 2021 01:25:56 GMT
WORKDIR /tmp
# Sat, 28 Aug 2021 01:26:16 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f1fdb786fa8b9ef3a08d0b331a51861cd5a6eea277e93bbad64bf37774df17c6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 28 Aug 2021 01:26:17 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4da59afefd4321f8d175c5bd1b393c479d6733a58eece9df143ca37c633fd7`  
		Last Modified: Fri, 27 Aug 2021 17:42:30 GMT  
		Size: 187.9 MB (187897894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a03c2b2efa013eb2452cce1335769240c2a2de4366423ffcf4aa8ec04128d7`  
		Last Modified: Sat, 28 Aug 2021 01:30:41 GMT  
		Size: 38.4 MB (38419182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-1.10.3.943-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cf0c206c11abec8bb70c9eee6277ac27b1afa389b62f6f2140f2ce52bb7a0092
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.6 MB (253579925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb09215316fe11eb30152b677725eb18e0e1a704828ef3570b1a1f3391d08cc`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:04:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:04:05 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 17 Aug 2021 06:04:06 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:04:06 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 17:51:00 GMT
ENV JAVA_VERSION=18-ea+12
# Fri, 27 Aug 2021 17:51:17 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='a9bc316abb2e03378f35fc574685b8bbdd15cd6803df70c02e71ff8f19ad292b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/12/GPL/openjdk-18-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='08129b3c4ef9956a14a7112565a185ac9ea7e3b327875089114ce6fe2563f585'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 27 Aug 2021 17:51:18 GMT
CMD ["jshell"]
# Sat, 28 Aug 2021 02:05:16 GMT
ENV CLOJURE_VERSION=1.10.3.943
# Sat, 28 Aug 2021 02:05:16 GMT
WORKDIR /tmp
# Sat, 28 Aug 2021 02:05:33 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f1fdb786fa8b9ef3a08d0b331a51861cd5a6eea277e93bbad64bf37774df17c6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 28 Aug 2021 02:05:33 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a27af984eefbe6b82ccb775aead56e92f82cf16d079218087ebe132125cf5`  
		Last Modified: Tue, 17 Aug 2021 06:15:41 GMT  
		Size: 3.1 MB (3118861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c2f7b6d0e50c72cec02e8f9f1af7f75a17bdd36f40add0a16696f37c596a71`  
		Last Modified: Fri, 27 Aug 2021 18:07:39 GMT  
		Size: 186.6 MB (186633190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf655e3c1062b043441b14a7810bff8d3e5cce78eefadbc62eb4a666a5da4e`  
		Last Modified: Sat, 28 Aug 2021 02:11:48 GMT  
		Size: 37.9 MB (37912802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
