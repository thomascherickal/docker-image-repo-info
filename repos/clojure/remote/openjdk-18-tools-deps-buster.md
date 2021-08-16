## `clojure:openjdk-18-tools-deps-buster`

```console
$ docker pull clojure@sha256:fbeeefda9889d68f7bb4206aa586357b2286a71d3e9db8d8381c2eeff1512e08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-buster` - linux; amd64

```console
$ docker pull clojure@sha256:59c7d5288bbdebde0ee86e60d4248fd74c0f72ebafc78cee99a2fd33d5aaf4db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348682262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:887b6f6880186d6f04ae4a87bca349b614935383439c7377169ce9cab137c9ac`
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
# Thu, 22 Jul 2021 13:33:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 22 Jul 2021 13:33:13 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:33:13 GMT
ENV LANG=C.UTF-8
# Fri, 13 Aug 2021 17:27:04 GMT
ENV JAVA_VERSION=18-ea+10
# Fri, 13 Aug 2021 17:27:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='f02c5e52c193b349688216e85ab6fb67548861e93d96dd454f74881abfb696b2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6a6ba79485e560d0d7687152a2a1dfa92cbe80871f16eb24b52e01274f9f4f6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Aug 2021 17:27:15 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 20:25:30 GMT
ENV CLOJURE_VERSION=1.10.3.943
# Mon, 16 Aug 2021 20:25:30 GMT
WORKDIR /tmp
# Mon, 16 Aug 2021 20:25:42 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f1fdb786fa8b9ef3a08d0b331a51861cd5a6eea277e93bbad64bf37774df17c6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Mon, 16 Aug 2021 20:25:42 GMT
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
	-	`sha256:0bf28cbe84e179afe37b71e900696a26c014994de5713503c8da37ccc9d95fc7`  
		Last Modified: Fri, 13 Aug 2021 17:33:17 GMT  
		Size: 187.6 MB (187575629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6576f0557b6222e4707e6161c0de1087eca8027b452a2e9d29c73a0f7c64ca4f`  
		Last Modified: Mon, 16 Aug 2021 20:32:20 GMT  
		Size: 27.1 MB (27078390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ae11d7dabe13ef8bce4783441c772977bfa90f3c632f922044b21f1846da859c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.7 MB (346733423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9881cdf5e4dc70079f271156f2d72448b826e8cb72ac780845c6b883f1d51626`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:15:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:15:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 22 Jul 2021 05:15:12 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 05:15:12 GMT
ENV LANG=C.UTF-8
# Fri, 13 Aug 2021 17:41:21 GMT
ENV JAVA_VERSION=18-ea+10
# Fri, 13 Aug 2021 17:41:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='f02c5e52c193b349688216e85ab6fb67548861e93d96dd454f74881abfb696b2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6a6ba79485e560d0d7687152a2a1dfa92cbe80871f16eb24b52e01274f9f4f6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Aug 2021 17:41:30 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 20:45:40 GMT
ENV CLOJURE_VERSION=1.10.3.943
# Mon, 16 Aug 2021 20:45:40 GMT
WORKDIR /tmp
# Mon, 16 Aug 2021 20:45:52 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f1fdb786fa8b9ef3a08d0b331a51861cd5a6eea277e93bbad64bf37774df17c6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Mon, 16 Aug 2021 20:45:52 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967a8f1385966af47c9f250997e3158c319d498adc004c91570f770ceac5045a`  
		Last Modified: Thu, 22 Jul 2021 01:25:24 GMT  
		Size: 52.2 MB (52167528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176877461d089b6f2c205b71c8892552af1b56d6cd599f6db980e3275e7f589c`  
		Last Modified: Thu, 22 Jul 2021 05:29:29 GMT  
		Size: 14.7 MB (14673538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f074c4a88d9841da217b0c38836e1597b7ca617b49eeee9d29cc4fc218619c`  
		Last Modified: Fri, 13 Aug 2021 17:52:44 GMT  
		Size: 186.3 MB (186330378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31168e34cb6982c626b59a52ad237e80fbaccca9e595643d1cf2eb3d713efd56`  
		Last Modified: Mon, 16 Aug 2021 20:54:22 GMT  
		Size: 26.7 MB (26660629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
