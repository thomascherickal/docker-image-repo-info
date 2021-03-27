## `clojure:openjdk-17-boot-2.8.3-buster`

```console
$ docker pull clojure@sha256:9849c0b434dee932531048526f64c0574a82598a1997dc7989412e5d0de73c10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-2.8.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:518cab9a84de725dc97a0d7a508442c99a492cf821dff1380b7a6875d6ec6196
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.5 MB (378498078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80db8bee97c49573e0bff27e18bec9c6ae87861c9c8f6a4650c3960514bd8412`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:09:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:09:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 12 Mar 2021 22:09:32 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:09:32 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 05:43:01 GMT
ENV JAVA_VERSION=17-ea+15
# Fri, 26 Mar 2021 05:43:11 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='da690c53a8d23b278b4878acf414b0d95ca40dd1533d08ce313589cf1df1c9c3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93178b313750b38e1bbc811b989dcee27d988cb223b30ba829122ecdbd08f403'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 05:43:12 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:12:15 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Mar 2021 20:12:15 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Mar 2021 20:12:15 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:12:16 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 26 Mar 2021 20:12:17 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Mar 2021 20:12:17 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Mar 2021 20:12:38 GMT
RUN boot
# Fri, 26 Mar 2021 20:12:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc5e25d4a8a1517c089381c0299ea2a0dbf472a2310940edd3aaaeda7c0041d`  
		Last Modified: Fri, 12 Mar 2021 22:21:36 GMT  
		Size: 13.9 MB (13921265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624a53d72e1f9e3c69d2696a561ec2137c7169ceff2ab5634f72a3fd7f3d5d02`  
		Last Modified: Fri, 26 Mar 2021 05:50:15 GMT  
		Size: 185.7 MB (185679974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2a3638c990755d2573b1b0b6c73ab57aceace0dd6917d57b6d794f76d3de3d`  
		Last Modified: Fri, 26 Mar 2021 20:23:07 GMT  
		Size: 6.9 KB (6918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e4761bf271abdd0abc9cfd7f877b79c976f9ad7148806aa9bb76257734b13f`  
		Last Modified: Fri, 26 Mar 2021 20:23:11 GMT  
		Size: 58.8 MB (58820441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-2.8.3-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:33e3cebc6abdb51b66651c03b9a5e036d7d0a56e79b234bfee167c8391b960f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.3 MB (374297712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b62dccfe09040a20b0fa3c710743d9647ee84ada7da66aa0c2d6b7d52d5bddd`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:16 GMT
ADD file:b2e2cca51e131b97e6a7e02af893c7f9b1f7a491b3d5fdaafa80409ed248a706 in / 
# Fri, 12 Mar 2021 01:53:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:29:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:29:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:33:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 12 Mar 2021 06:33:43 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:33:44 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 13:34:29 GMT
ENV JAVA_VERSION=17-ea+15
# Fri, 26 Mar 2021 13:34:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='da690c53a8d23b278b4878acf414b0d95ca40dd1533d08ce313589cf1df1c9c3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93178b313750b38e1bbc811b989dcee27d988cb223b30ba829122ecdbd08f403'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 13:35:02 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:21:34 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Mar 2021 20:21:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Mar 2021 20:21:36 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:21:38 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 26 Mar 2021 20:21:39 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Mar 2021 20:21:40 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Mar 2021 20:22:02 GMT
RUN boot
# Fri, 26 Mar 2021 20:22:04 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e9742a63e95a88f8685c4f23a73f7dd15e4039ac1862ce5753c53406a5f7c04a`  
		Last Modified: Fri, 12 Mar 2021 02:01:14 GMT  
		Size: 49.2 MB (49195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90273c85fdda8648cee9282aa7b01faf0ec1f45451931985b3504c37cf1ac3e6`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 7.7 MB (7694407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685f873e984153af9a44cf556c7679b430b9c557d901c7d476725134f28754e7`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 10.0 MB (9984339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34041dfaf60ca49c213d83e89205fc2b7e222817c9728a4aa4f7d3f09d579c9`  
		Last Modified: Fri, 12 Mar 2021 02:43:54 GMT  
		Size: 52.2 MB (52165212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea7dd455a2166654bd3d729e78a91e18b7d2fb982780428bf02e0d1d700cb88`  
		Last Modified: Fri, 12 Mar 2021 06:44:30 GMT  
		Size: 14.7 MB (14673622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc6657c95a21cc819a57d15b5cf3ae7bc7e5177df92ade97c1e4b9e3e2b977`  
		Last Modified: Fri, 26 Mar 2021 13:41:24 GMT  
		Size: 181.8 MB (181757146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a511ab3742af56bc1a16c58dfe744c80229014eddea093e83a89a72327b2e1`  
		Last Modified: Fri, 26 Mar 2021 20:29:00 GMT  
		Size: 6.9 KB (6922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79eb910ab9fd3c7a8e35fad3036b336e672d45b3199a63ee5d8ab4f0f8d44a7`  
		Last Modified: Fri, 26 Mar 2021 20:29:08 GMT  
		Size: 58.8 MB (58820301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
