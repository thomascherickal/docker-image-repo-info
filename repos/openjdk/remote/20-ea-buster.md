## `openjdk:20-ea-buster`

```console
$ docker pull openjdk@sha256:77d91fb69f934002c452e2c9806092aee42ad230cd1951bc1524803fb3b5cf00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:6d72d0d153a5c0d7fa9672e9fbb4895e3b0bf1bf586be2f2ea6a93b8004616eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331076319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6133ca2b9e5d116dd07e890094a8bdb4f0e13ced6294ce05c0e109455e3a5dfc`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:01:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:01:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 13:01:29 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 13:01:30 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 13:01:30 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 13:01:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 13:01:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6315e893372434bf09990677f857fdd026ba0abdd98d435decc2ec5742cee4`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 7.9 MB (7857339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad12dd0da3ea9c59f4c4fc53d6a204e11e2930b9dc4143376024ed8fa5c71bb`  
		Last Modified: Wed, 05 Oct 2022 01:20:24 GMT  
		Size: 10.0 MB (9998384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0ceb4387f59959418bd2da17176107c9ce0ea542cf017ce14835999fa8437`  
		Last Modified: Wed, 05 Oct 2022 01:20:41 GMT  
		Size: 51.8 MB (51844142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce765e1cc6c0bfde215679620f9f3d420f1eb249616a359ee107cce6ba3971`  
		Last Modified: Wed, 05 Oct 2022 13:06:58 GMT  
		Size: 13.9 MB (13924265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dea7335c42f09cf1545fbd50fb29902d7736c4e77b1b119799e87c8cef87a27`  
		Last Modified: Wed, 05 Oct 2022 13:07:11 GMT  
		Size: 197.0 MB (197011087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5b3ad444fedda40ecc8fb607b4aa093795b4df6cae14cec5eb86e3966206d4b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.1 MB (329144312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d81c5cf5409759b3e4ddad25ecc6daa90538fc55cc06bf24698466bbefa671`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:24:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:24:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:24:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:27:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:27:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 05 Oct 2022 04:27:12 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 04:27:13 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:27:14 GMT
ENV JAVA_VERSION=20-ea+17
# Wed, 05 Oct 2022 04:27:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='9d46acb0892a134f62ab21fca33fdef1da5d579f61ddbd0ae3ff0b4d33c5eca2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/17/GPL/openjdk-20-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='31245b15195bf9f12a6db08474bfcbd1ddbccc76436372bf4db538c6ede8f976'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 05 Oct 2022 04:27:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ae492f07ea828401b80eb34c8c630b72cb66cac155b003e81ab2921dc57f3d`  
		Last Modified: Wed, 05 Oct 2022 00:38:37 GMT  
		Size: 7.7 MB (7722031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c91e11c5a0db8322590ddbb61600624fdd82d3d6174d1de01c30be3e7ca535`  
		Last Modified: Wed, 05 Oct 2022 00:38:37 GMT  
		Size: 9.8 MB (9769003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647de18a9400fa5e9ba5c0c5aaacd374b6728cbf14527e0ac59947e0b864af27`  
		Last Modified: Wed, 05 Oct 2022 00:38:55 GMT  
		Size: 52.2 MB (52175488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123f4f9caecd89ce907bd1cc7635a78ee3adbdf4fcd12120c708e4e0f2e18a04`  
		Last Modified: Wed, 05 Oct 2022 04:36:25 GMT  
		Size: 14.7 MB (14670029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3de7eb85f32204d9dadd94fcfdb83254d254a79f7945f9598a8542ca76ab9e`  
		Last Modified: Wed, 05 Oct 2022 04:36:39 GMT  
		Size: 195.6 MB (195578876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
