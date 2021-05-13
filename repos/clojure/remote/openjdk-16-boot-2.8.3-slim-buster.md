## `clojure:openjdk-16-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:e6ca034c766cb1300034de0793dc8f398636faeb5f1f2c4d1e9b072e798a564f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:2923e1c08f8eef71d8da14282100a54b4a1c1e85849263803babe7d2fa2012c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274690818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe1bd5e75e7819de71df4bb2a599302b6184a1dd77930df0376b22a65ce883a`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:48:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:49:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 12 May 2021 06:49:03 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:49:03 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:49:03 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 12 May 2021 06:49:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 May 2021 06:49:20 GMT
CMD ["jshell"]
# Thu, 13 May 2021 04:38:46 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 13 May 2021 04:38:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 13 May 2021 04:38:46 GMT
WORKDIR /tmp
# Thu, 13 May 2021 04:38:51 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 13 May 2021 04:38:51 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 13 May 2021 04:38:51 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 13 May 2021 04:39:12 GMT
RUN boot
# Thu, 13 May 2021 04:39:12 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b89b6081832b112f9483322d4710c661f12135e79279dc3fb1672883ada8d`  
		Last Modified: Wed, 12 May 2021 06:58:18 GMT  
		Size: 3.3 MB (3268772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d29af6e74a7191129548f5ca528ff6e2fb9f756facbbdf63ddd4fca3529017`  
		Last Modified: Wed, 12 May 2021 07:00:46 GMT  
		Size: 185.2 MB (185175837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e048f46e2020e6780ab37bfaa6f889bfe7cf7e0a2c26e9594882306a87c56f`  
		Last Modified: Thu, 13 May 2021 04:49:28 GMT  
		Size: 279.7 KB (279719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fea7e140de2789976b5157a1eb5754453e05d4889cf51f35260d105cad15c5`  
		Last Modified: Thu, 13 May 2021 04:49:32 GMT  
		Size: 58.8 MB (58820575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-boot-2.8.3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d2556f2cb59ed14d7d221d8e2d272a4ba10b663a1374da1318ff421cd6a07728
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.7 MB (267688281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ab62cc70d4a4239afc13b6de4bd771a35ea35b36153ead31a2776f6f1752bc`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:17:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 12 May 2021 06:17:50 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:17:51 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:17:52 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 12 May 2021 06:18:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 May 2021 06:18:18 GMT
CMD ["jshell"]
# Thu, 13 May 2021 03:31:54 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 13 May 2021 03:31:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 13 May 2021 03:31:56 GMT
WORKDIR /tmp
# Thu, 13 May 2021 03:32:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 13 May 2021 03:32:18 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 13 May 2021 03:32:20 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 13 May 2021 03:32:50 GMT
RUN boot
# Thu, 13 May 2021 03:32:52 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49feb8163b50086a917c966dbaff372d7e4189ec1a1a504bb2b3b5258a09d616`  
		Last Modified: Wed, 12 May 2021 06:26:49 GMT  
		Size: 3.1 MB (3118874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d9d953bd6b37978aa23baa45046e5f720b12d592f09fa3b5e0e25638e1b205`  
		Last Modified: Wed, 12 May 2021 06:29:02 GMT  
		Size: 179.6 MB (179558182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911d95aeb07d61ed87aa42f7985271ce531b2977181be1af111d079ad16b710c`  
		Last Modified: Thu, 13 May 2021 03:42:59 GMT  
		Size: 279.7 KB (279673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd708dc671573b682a46452acee3df955593096698648b899760f40659acb3a`  
		Last Modified: Thu, 13 May 2021 03:43:03 GMT  
		Size: 58.8 MB (58820302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
