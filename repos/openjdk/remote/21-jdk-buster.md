## `openjdk:21-jdk-buster`

```console
$ docker pull openjdk@sha256:9a49394b62f31cdbe00e83ded24e7208722032be274fbf8bc54cc76a583c2eae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:06898d71f3253a2944ee80c3db17c7ea7b0c6ed3da39f391c17990fdc12a97b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335807835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcf43bc4191c9f2135e63e9271f7263f121310cf121368c366616033a03c6b4e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:15 GMT
ADD file:40953ed6e6f96703b2e0c13288437c2aaf8b3df33dbc423686290cbe0e595a5e in / 
# Wed, 12 Apr 2023 00:20:15 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:53:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:38:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:38:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 09:38:48 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 09:38:48 GMT
ENV LANG=C.UTF-8
# Fri, 21 Apr 2023 20:08:04 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:08:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:08:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2ff1d7c41c74a25258bfa6f0b8adb0a727f84518f55f65ca845ebc747976c408`  
		Last Modified: Wed, 12 Apr 2023 00:24:01 GMT  
		Size: 50.4 MB (50448726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253aeafeaa7e0671bb60008df01de101a38a045ff7bc656e3b0fbfc7c05cca5`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 7.9 MB (7863355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2201bd995cccf12851a50820de03d34a17011dcbb9ac9fdf3a50c952cbb131`  
		Last Modified: Wed, 12 Apr 2023 07:58:30 GMT  
		Size: 10.0 MB (10001452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76e268b103d05fa8960e0f77951ff54b912b63429c34f5d6adfd09f5f9ee2`  
		Last Modified: Wed, 12 Apr 2023 07:58:44 GMT  
		Size: 51.9 MB (51876420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399074859846284cf7215864e33c04dcf5cdaea60ce124b322a573d85aaf4f88`  
		Last Modified: Wed, 12 Apr 2023 09:41:05 GMT  
		Size: 13.9 MB (13927462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3302593a36082d27077dc780b1b165f4c391092c3dbc4e75c0224ddce8050106`  
		Last Modified: Fri, 21 Apr 2023 20:11:44 GMT  
		Size: 201.7 MB (201690420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:94e0c2c9893f5f2fa100f85f4f1f9a9cab720bff35a6a0ef60f58e0e408a0305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333896682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30baa844953f4c2be849acf5f879999c476ec9f1e37e366b58ce5f7b5bd57b6a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:55 GMT
ADD file:93facc669dd63b37fb5dde18f3b3a1cb5621aa396e1960ea85facdd1c619a3f0 in / 
# Wed, 12 Apr 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:08:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:11:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:11:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 05:11:23 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 05:11:23 GMT
ENV LANG=C.UTF-8
# Fri, 21 Apr 2023 20:23:24 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:23:32 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:23:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b4910c31031a0301ea4f8b7155269014925aeb17c71b869dea3ff907ba294b55`  
		Last Modified: Wed, 12 Apr 2023 00:42:52 GMT  
		Size: 49.2 MB (49238632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fd617b499747daceba851b67da426c285d1e306b316a193f06968123f49da`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 7.7 MB (7732136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efadebfda1423d1b70a0e991e9ff8bb2e3fe0b08d55562359a004c265fc7c86`  
		Last Modified: Wed, 12 Apr 2023 01:14:12 GMT  
		Size: 10.0 MB (10003581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7c438113f5e58417f97e7eb0a755b17ee63eebd85a7c3b86a2aad4c993e`  
		Last Modified: Wed, 12 Apr 2023 01:14:27 GMT  
		Size: 52.2 MB (52191713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2366261c1c9b2f21e7c4ec50b2d68887e4f635d49fe0d81f2db7f7d01df9c77e`  
		Last Modified: Wed, 12 Apr 2023 05:13:37 GMT  
		Size: 14.7 MB (14672627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e107ff7b15a6e01f61df35fc360760f20b3af9058029eaa684d982c9f0928f73`  
		Last Modified: Fri, 21 Apr 2023 20:26:42 GMT  
		Size: 200.1 MB (200057993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
