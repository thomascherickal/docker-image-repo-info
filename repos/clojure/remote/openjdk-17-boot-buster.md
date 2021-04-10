## `clojure:openjdk-17-boot-buster`

```console
$ docker pull clojure@sha256:f3016630e12c5385b1e9315230290be09880dc567bd82a2206fe37bbf03e4824
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot-buster` - linux; amd64

```console
$ docker pull clojure@sha256:f5bc6d4e4be3df9220e93f250d67609c82159f79372222d644332abd8517e316
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.9 MB (378930015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952e69b3d9e99a90e1eb061e16a20869b9cafef1b737206a201484c4d2f82f06`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:03:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:40:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:40:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 31 Mar 2021 05:40:26 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 05:40:26 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:55:37 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:55:47 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:55:48 GMT
CMD ["jshell"]
# Fri, 09 Apr 2021 19:35:05 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Apr 2021 19:35:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Apr 2021 19:35:06 GMT
WORKDIR /tmp
# Fri, 09 Apr 2021 19:35:07 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 09 Apr 2021 19:35:07 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Apr 2021 19:35:07 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Apr 2021 19:35:27 GMT
RUN boot
# Fri, 09 Apr 2021 19:35:27 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234b70d0479d7f16d7ee8d04e4ffdacc57d7d14313faf59d332f18b2e9418743`  
		Last Modified: Tue, 30 Mar 2021 23:14:37 GMT  
		Size: 51.8 MB (51840782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba3dff9f19003d9bccdb99aff6591b545b6bfd1c7dd7bd791f8c695f45339ce`  
		Last Modified: Wed, 31 Mar 2021 05:51:50 GMT  
		Size: 13.9 MB (13921332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593128b16c8200a79e445704857e2a55bddd99b70c712246986664ed03215154`  
		Last Modified: Fri, 09 Apr 2021 19:02:31 GMT  
		Size: 186.1 MB (186077846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918ffbd83816e5e16e145a84d197ccb654b89e1cee8e2fa32a9ffc851f33ac56`  
		Last Modified: Fri, 09 Apr 2021 19:39:50 GMT  
		Size: 6.9 KB (6921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e1de5b3de71a6669af60a6000e5f755a62498674bf3b17e3c10bf2022e332e`  
		Last Modified: Fri, 09 Apr 2021 19:39:55 GMT  
		Size: 58.8 MB (58820476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b517e3312ac20b7e9a8899eb22d60a6a4040e384c61696e86b5c04f9b200168b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.7 MB (374697523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeecfe901032b0a84e9dad5e0a77e0a9ff9723db38d4cf7afba8c2165a3413d7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:38:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 31 Mar 2021 01:38:03 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 01:38:04 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:42:16 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:42:34 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:42:36 GMT
CMD ["jshell"]
# Fri, 09 Apr 2021 19:47:06 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Apr 2021 19:47:07 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Apr 2021 19:47:08 GMT
WORKDIR /tmp
# Fri, 09 Apr 2021 19:47:10 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Fri, 09 Apr 2021 19:47:11 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Apr 2021 19:47:12 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Apr 2021 19:47:34 GMT
RUN boot
# Fri, 09 Apr 2021 19:47:35 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70c372ae296f23e908bf1e1ed9f4c0c81a8a6d7fc48c0e2db16035bb9b7a54`  
		Last Modified: Wed, 31 Mar 2021 00:30:24 GMT  
		Size: 52.2 MB (52165620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca103f822d8cb58a9704fc742e0a249375e6458c2a46de766e57f6cc850ee8d`  
		Last Modified: Wed, 31 Mar 2021 01:49:05 GMT  
		Size: 14.7 MB (14673676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3854132c9285f3d7ca2043c05afcc5b145beb56f47c7555bc6d579cb885cc84`  
		Last Modified: Fri, 09 Apr 2021 18:48:48 GMT  
		Size: 182.1 MB (182126705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711649a0450acc5b574f9ededf293ad34c2fba9ae773ce353b8aed2315451852`  
		Last Modified: Fri, 09 Apr 2021 19:51:43 GMT  
		Size: 6.9 KB (6923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4370c4bd7e8ef150a2e4af9be545780fba211cc5dce6a1ffaa70b8eb629734e4`  
		Last Modified: Fri, 09 Apr 2021 19:51:51 GMT  
		Size: 58.8 MB (58819870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
