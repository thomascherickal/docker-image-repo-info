## `openjdk:20-ea-bullseye`

```console
$ docker pull openjdk@sha256:ca7c28dc195e21b268e482ebb7f0482a2ce1c58eb5139102fffb8b9e97273594
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:5e561e6502b87f6a585dce684c3f837cab62e2e114295553551e826c85480afd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (337021325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef9ce60ac93798c87d9abcb9a0434aa46f9eec7cb63ba8a9e84873fc2de41ac2`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:47:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:47:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:47:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 02 Aug 2022 05:47:28 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 05:47:28 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:51:49 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 22:52:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='0d07c62c8d17ef034b26568ed71d3025cf9dcbc6b4294987e53d54cab10f549f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='13fc41a17f015ca801975625021a320b5112883194fc5dde964529894907fd83'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:52:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daef329d35093868ef75ac8b7c6eb407fa53abbcb3a264c218c2ec7bca716e6`  
		Last Modified: Tue, 02 Aug 2022 02:18:47 GMT  
		Size: 54.6 MB (54584071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb50685d3bdd31de6428e61e2423e774e3dc599e8e946f0545708b6be40cb0e`  
		Last Modified: Tue, 02 Aug 2022 06:00:43 GMT  
		Size: 14.1 MB (14071388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70517516673f901935c1e5d85b1e67803eae97a40411870ef43759e1972a14a3`  
		Last Modified: Mon, 08 Aug 2022 23:01:38 GMT  
		Size: 197.3 MB (197333794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6f788e2783aef10406fdc5b1de012eb3a9d13812adc7c13d24ebd9c005cf8683
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.7 MB (335727141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab6f02431c465c1dcd002429837367762d943248daa6d3244f25d87e559e923`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:24:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:41:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:41:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 02 Aug 2022 04:41:17 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:41:18 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:30:39 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 23:31:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='0d07c62c8d17ef034b26568ed71d3025cf9dcbc6b4294987e53d54cab10f549f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='13fc41a17f015ca801975625021a320b5112883194fc5dde964529894907fd83'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:31:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9e95aca686baf2f9b88f3822104381dc1cd0e2bd6dc105b7468059336dbab`  
		Last Modified: Tue, 02 Aug 2022 01:44:56 GMT  
		Size: 54.7 MB (54680407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c84f2fed3bc5b2ff7fa0aeda3db25dd1b5862773b1566ea13ae879f522df4a`  
		Last Modified: Tue, 02 Aug 2022 05:02:43 GMT  
		Size: 15.5 MB (15525172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a23a34e38332a558a450416e5063a20a37de86f772e4a483e2de583e6f38a8`  
		Last Modified: Mon, 08 Aug 2022 23:47:23 GMT  
		Size: 196.0 MB (196032162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
