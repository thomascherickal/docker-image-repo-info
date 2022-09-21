## `openjdk:20-ea-jdk-bullseye`

```console
$ docker pull openjdk@sha256:c32b4d63b4f63d903b6a035ea2b876d5efa2ab90a827e397199ac08425138c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:d7f26b90667f2d21fa4c2ac8a34366740dc877f9bbb5f7e7119cf42d87229e52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336695441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561c319f79fa26404478cabdc520c4b22d32dfc4518c7eb4cedbf74413db292c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:01:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:01:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 13 Sep 2022 07:01:39 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 07:01:39 GMT
ENV LANG=C.UTF-8
# Wed, 21 Sep 2022 00:00:46 GMT
ENV JAVA_VERSION=20-ea+15
# Wed, 21 Sep 2022 00:00:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='2ee417bc5d9f36c634a5e004c201967b70b6b3a5382147d74406cc9b015eac97'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ec219647905af892891d6fd018538043bf19cfae2a40df439b9fde070476681'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Sep 2022 00:00:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8471b75885efc7790a16be5328e3b368567b76a60fc3feabd6869c15e175ee05`  
		Last Modified: Tue, 13 Sep 2022 03:50:26 GMT  
		Size: 54.6 MB (54584419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a417ba6efed46614cf2c647352c58c789bc5b46ce4b1edf5d885af25eec5d9`  
		Last Modified: Tue, 13 Sep 2022 07:08:38 GMT  
		Size: 14.1 MB (14071910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffccd1453a9b548704f5dba5f7253763e7124be5ec21e901271559ce8595d0cd`  
		Last Modified: Wed, 21 Sep 2022 00:05:52 GMT  
		Size: 197.0 MB (196969796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:72f11799af4ad5bcf7b930599fd8dff82610a30e340254875a611dce1fe0317d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.2 MB (335203060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f57b7a7486ada59fc29b5e4094401757fcc4763d56e3f584150b4e23c9696891`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 14:37:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 13 Sep 2022 14:37:22 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 14:37:23 GMT
ENV LANG=C.UTF-8
# Wed, 21 Sep 2022 00:34:14 GMT
ENV JAVA_VERSION=20-ea+15
# Wed, 21 Sep 2022 00:34:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='2ee417bc5d9f36c634a5e004c201967b70b6b3a5382147d74406cc9b015eac97'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ec219647905af892891d6fd018538043bf19cfae2a40df439b9fde070476681'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Sep 2022 00:34:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9360b3024e18f921a2fcec8614f617312c87ea1a31b5c94c9c643535bde9775`  
		Last Modified: Tue, 13 Sep 2022 05:10:20 GMT  
		Size: 54.7 MB (54681497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6968571fec9e6970e53ddd2e6eb88d89c4bcf91b69d71397dc9034151960bf75`  
		Last Modified: Tue, 13 Sep 2022 14:49:29 GMT  
		Size: 15.5 MB (15527490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb28ee3cc27ca3419d77735b1f77c09cd3101061acc4a434fc927642d960b39e`  
		Last Modified: Wed, 21 Sep 2022 00:42:21 GMT  
		Size: 195.5 MB (195496270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
