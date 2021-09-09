## `clojure:openjdk-11-boot-2.8.3`

```console
$ docker pull clojure@sha256:532a79c2ddeec81b9e425cc3b91bb3d5a2d319ebcde92d3d1146bef1f86c40da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-11-boot-2.8.3` - linux; amd64

```console
$ docker pull clojure@sha256:515b4d5659453b16ca027b33d9e6c6e37059b979ec1cdf6f659a0f1591e77104
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.9 MB (392888794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e6a42a3e88d272c1f9c2b9b97ad7135f4d58af2c84c108c79bd556e3ef00b8`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:07 GMT
ADD file:1fedf68870782f1b44cd50691444aab4061cc0c70f24e5fabe9c562cc46eb9af in / 
# Fri, 03 Sep 2021 01:21:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:31:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:31:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:36:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:36:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 03 Sep 2021 08:36:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 08:36:46 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:36:46 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:36:47 GMT
ENV JAVA_VERSION=11.0.12
# Fri, 03 Sep 2021 08:37:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Sep 2021 08:37:10 GMT
CMD ["jshell"]
# Thu, 09 Sep 2021 19:28:01 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Sep 2021 19:28:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Sep 2021 19:28:01 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:28:02 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Thu, 09 Sep 2021 19:28:02 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Sep 2021 19:28:03 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Sep 2021 19:28:23 GMT
RUN boot
# Thu, 09 Sep 2021 19:28:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:955615a668ce169f8a1443fc6b6e6215f43fe0babfb4790712a2d3171f34d366`  
		Last Modified: Fri, 03 Sep 2021 01:26:55 GMT  
		Size: 54.9 MB (54926871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2756ef5f69a5190f4308619e0f446d95f5515eef4a814dbad0bcebbbbc7b25a8`  
		Last Modified: Fri, 03 Sep 2021 06:39:22 GMT  
		Size: 5.2 MB (5153100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ea9f2bd51e53a455297e0631e18a72a86d7e2c8e1807176e80f991bde5d64`  
		Last Modified: Fri, 03 Sep 2021 06:39:23 GMT  
		Size: 10.9 MB (10871687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0a22ee906271a6ce9ddd1754fdd7d3b59078e0b57b6cc054c7ed7ac301587`  
		Last Modified: Fri, 03 Sep 2021 06:39:45 GMT  
		Size: 54.6 MB (54566834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785dffb36c6c7fbfd1c98d950a9b49054e84bccdd4b54ebfab50b0e93dbfeefe`  
		Last Modified: Fri, 03 Sep 2021 08:57:20 GMT  
		Size: 5.4 MB (5419927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fccb14f036954b636e49dbcf931976a06ecca6fc5336d8a3d32f4e03e57e95d`  
		Last Modified: Fri, 03 Sep 2021 08:57:19 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0c30fedd9c48311ffe0ca7cdf5e0bbd514d76f31d70b948f64fd218bffb93c`  
		Last Modified: Fri, 03 Sep 2021 08:57:40 GMT  
		Size: 203.1 MB (203122725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4141e76e04a3bd664be3de26709571018c37a73b27c8761e8a3d026b6efec9b`  
		Last Modified: Thu, 09 Sep 2021 19:44:46 GMT  
		Size: 6.9 KB (6930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5a7bfb87461a2144bc7f88e4b70732971fe5e6f30c120d00483c7ffd3233ad`  
		Last Modified: Thu, 09 Sep 2021 19:44:49 GMT  
		Size: 58.8 MB (58820512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-11-boot-2.8.3` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:34fef5e8b42abc7e1891f731bcb2170780e96b153194ed8fee9f1f0e8cfbb590
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.9 MB (383902765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b607482a4cdfe18bc5d23d98392df860dab35d9d28a07a49de4f2fc95128d004`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:33:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:50:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:50:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 03 Sep 2021 10:50:42 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 10:50:42 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 10:50:42 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 10:50:42 GMT
ENV JAVA_VERSION=11.0.12
# Fri, 03 Sep 2021 10:50:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Sep 2021 10:50:59 GMT
CMD ["jshell"]
# Sat, 04 Sep 2021 02:11:15 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 04 Sep 2021 02:11:15 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 04 Sep 2021 02:11:16 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 02:11:22 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Sat, 04 Sep 2021 02:11:22 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Sep 2021 02:11:22 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 04 Sep 2021 02:11:48 GMT
RUN boot
# Sat, 04 Sep 2021 02:11:48 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529bf6c2a9fdb0edf93a87f6fbc959069a0068fe2ed046af546fca48e8ed6ffe`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 7.7 MB (7695770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9703bfb802a7157134df39897b2625906f8057c03e52daa3e8298ca41dfd7b`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 10.0 MB (9984267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a64745ecb3a1d83570e6c503995c0eb3f97176e23bd91210bf235e5646a4e96`  
		Last Modified: Fri, 03 Sep 2021 04:42:38 GMT  
		Size: 52.2 MB (52167858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0b955a6813cb29ae066e0377af71d69a91642eee1500d24b72ae13c7ceb7f8`  
		Last Modified: Fri, 03 Sep 2021 11:15:27 GMT  
		Size: 5.3 MB (5277666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc68d208c38e033fa165d33031c719e6d18b22a261e547408432187432120560`  
		Last Modified: Fri, 03 Sep 2021 11:15:26 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c8644f5c617575404faeab4b98a187a24c3ba2ec4b5d303dfb95b2b2105477`  
		Last Modified: Fri, 03 Sep 2021 11:15:44 GMT  
		Size: 200.7 MB (200727376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b491e11e2592986f9b35155382ffd97f19dcbb181f8cd24d2ec26742ec308383`  
		Last Modified: Sat, 04 Sep 2021 02:25:41 GMT  
		Size: 6.9 KB (6930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c200fb380a39117c7fb0d4bd14f1f2dcbaa68c7933f72c9054e8002ccd596a`  
		Last Modified: Sat, 04 Sep 2021 02:25:45 GMT  
		Size: 58.8 MB (58820545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
