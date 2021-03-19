## `clojure:openjdk-17-boot`

```console
$ docker pull clojure@sha256:615f507bcc64e7ada7985d291323d181df6b37ad86bae92ac9fa4a76bd8185c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-boot` - linux; amd64

```console
$ docker pull clojure@sha256:2c213ec6faf15561f2bb0afbe13b27fc0f3ff7cd3cfbf96848fe4770c6bde7a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275433303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:874458fb5d96ea8f277ec1e0dc4a9c95203d23ed6b19984821ab87acaeff245e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 22:10:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:10:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 12 Mar 2021 22:10:14 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:10:14 GMT
ENV LANG=C.UTF-8
# Fri, 19 Mar 2021 18:24:55 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 19 Mar 2021 18:25:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='d4bfd596e0b4f3eefb416719a5b6ad98ab3f37f27855573e7c94526a4ffad7d2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='16646d2498690f98b44f196e74da8361ef05155038a04cb6f62fbb76df08e72f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 19 Mar 2021 18:25:09 GMT
CMD ["jshell"]
# Fri, 19 Mar 2021 18:57:17 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 19 Mar 2021 18:57:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 19 Mar 2021 18:57:18 GMT
WORKDIR /tmp
# Fri, 19 Mar 2021 18:57:22 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 19 Mar 2021 18:57:23 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 19 Mar 2021 18:57:23 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 19 Mar 2021 18:57:54 GMT
RUN boot
# Fri, 19 Mar 2021 18:57:54 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3555c3885852c38ecf4a297b798053677bc7553f9c7631788ef75e35cb4262c`  
		Last Modified: Fri, 12 Mar 2021 22:22:18 GMT  
		Size: 3.3 MB (3268564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6eadd7ea0ff10503878ecdef0efce1c90dd3b260372701bf5cfd9c6b8f9585`  
		Last Modified: Fri, 19 Mar 2021 18:31:55 GMT  
		Size: 186.0 MB (185963195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af9097dca1fe50511d8a68de0edb5205da69b7f0879b5bf01c4244f6caca1d5`  
		Last Modified: Fri, 19 Mar 2021 19:08:27 GMT  
		Size: 279.7 KB (279697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c288e973514199e94da5ece8551f09979270bd5ac95af877fdb9e66816e8570`  
		Last Modified: Fri, 19 Mar 2021 19:08:31 GMT  
		Size: 58.8 MB (58820846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cb1b8e17692b4d06b649f6cfd0110e816cd1fcc1aef8eaee33bb34a8a81bb300
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270122405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:672764984e6e4c293b862da9da1b668ec9048f5f5969d52613fe0d09564d2e88`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:34:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 12 Mar 2021 06:34:55 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:34:56 GMT
ENV LANG=C.UTF-8
# Fri, 19 Mar 2021 19:02:22 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 19 Mar 2021 19:03:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='d4bfd596e0b4f3eefb416719a5b6ad98ab3f37f27855573e7c94526a4ffad7d2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='16646d2498690f98b44f196e74da8361ef05155038a04cb6f62fbb76df08e72f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 19 Mar 2021 19:03:22 GMT
CMD ["jshell"]
# Fri, 19 Mar 2021 19:34:59 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 19 Mar 2021 19:35:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 19 Mar 2021 19:35:00 GMT
WORKDIR /tmp
# Fri, 19 Mar 2021 19:35:09 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 19 Mar 2021 19:35:10 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 19 Mar 2021 19:35:11 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 19 Mar 2021 19:35:45 GMT
RUN boot
# Fri, 19 Mar 2021 19:35:47 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303a8d33f3a602102b6a15a1f7974fc79449cdcff2c2fa6709b56cd1ac792384`  
		Last Modified: Fri, 12 Mar 2021 06:45:08 GMT  
		Size: 3.1 MB (3118728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451a9a2c802cfd9bb256d5e308fe44167a411566ff01525d361bf27a05965184`  
		Last Modified: Fri, 19 Mar 2021 19:09:22 GMT  
		Size: 182.0 MB (182046831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6392dabad1fb98373b01efabdda4b88af4dbf53ef983448dcec1e2aa851b644`  
		Last Modified: Fri, 19 Mar 2021 19:40:07 GMT  
		Size: 279.6 KB (279577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfd15bad1c40da8162f880d4b88a0e304a9f37eda00f3a0c215ac9f2515894d`  
		Last Modified: Fri, 19 Mar 2021 19:40:09 GMT  
		Size: 58.8 MB (58820757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
