## `openjdk:21-ea-17-bullseye`

```console
$ docker pull openjdk@sha256:f90811990d15428f69c2ccb716dcdc2a372d5f737588c2270dc9780918e23a16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-17-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:fd36014e5950f24e6d3ad27d1a147636af2f871f9582c2fa8b717cf570792a5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.3 MB (341282985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2830b620cf4ed811d8ddcbf00b0b75e2b759784f4d76787838e9e28e2505fc9`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:01:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 06:01:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:43:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 23 Mar 2023 16:43:58 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 16:43:58 GMT
ENV LANG=C.UTF-8
# Tue, 11 Apr 2023 23:33:13 GMT
ENV JAVA_VERSION=21-ea+17
# Tue, 11 Apr 2023 23:33:22 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='98dcda513be6f72005f9b52c79d88f7e6bef066baddf0b89d9847c125b6d9bed'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='795231d9254753b31583afabc08fb092c00cc2459962cfdd3e0b0bd32edcad92'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 11 Apr 2023 23:33:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a71c865a2c34678c6dea55e4b0928f751ee3c0ca91cace6e4e0578c534d6cf`  
		Last Modified: Thu, 23 Mar 2023 06:08:01 GMT  
		Size: 5.2 MB (5166592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670730c27c2eacf07897a6e94fe55423ea50b884d9c28161a283bbbf064d1124`  
		Last Modified: Thu, 23 Mar 2023 06:08:02 GMT  
		Size: 10.9 MB (10876735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7a2c95f0f8b221d776ccf35911b68eec2cf9414a44d216205a6f03e381d3d7`  
		Last Modified: Thu, 23 Mar 2023 06:08:19 GMT  
		Size: 54.6 MB (54583510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8dcb5102ca902e2a58b698b899fa3cd3444bd088c2c8b6cc0dd23b6e89edfc`  
		Last Modified: Thu, 23 Mar 2023 16:45:55 GMT  
		Size: 14.1 MB (14071945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2456ad4bb63378be11f5b2c868f9a0af1dda1709173a765231f01a4c0ddf2b6e`  
		Last Modified: Tue, 11 Apr 2023 23:36:10 GMT  
		Size: 201.5 MB (201538595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7095de837475cc946713492afb97e0bd3bd94d014e6dab999460dca46f35cdda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.8 MB (339834432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e8051367e208b68d2b40796b9fe55b8c867178e3267786905fd6635bdc9c2c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:11:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:11:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:32:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Thu, 23 Mar 2023 09:32:48 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:32:49 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 00:01:04 GMT
ENV JAVA_VERSION=21-ea+17
# Wed, 12 Apr 2023 00:01:11 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='98dcda513be6f72005f9b52c79d88f7e6bef066baddf0b89d9847c125b6d9bed'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/17/GPL/openjdk-21-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='795231d9254753b31583afabc08fb092c00cc2459962cfdd3e0b0bd32edcad92'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 Apr 2023 00:01:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7971239fe1d69763272ccc0b2527efa95547d37c53630ed0a71db4e00d3ef964`  
		Last Modified: Thu, 23 Mar 2023 07:17:07 GMT  
		Size: 5.2 MB (5152756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c861b53509d61c37240d2f80efb3a351d2f1d7f4f8e8ec2e5004c1d86af89c`  
		Last Modified: Thu, 23 Mar 2023 07:17:07 GMT  
		Size: 10.9 MB (10873620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1714880ecc1c021a5f708f4369f91d3c2c53b998a56d563d0a9aa9be2488d794`  
		Last Modified: Thu, 23 Mar 2023 07:17:23 GMT  
		Size: 54.7 MB (54676068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131a790807c32d35d008bb181fd117e5707533f32521e79dc14cbb9702a03c01`  
		Last Modified: Thu, 23 Mar 2023 09:34:39 GMT  
		Size: 15.5 MB (15529075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a647f8aa27659ad2947a5946945e4daf48523e1a82adf4bc0ccf5f21b3057f`  
		Last Modified: Wed, 12 Apr 2023 00:03:43 GMT  
		Size: 199.9 MB (199899814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
