## `openjdk:19-ea-jdk-buster`

```console
$ docker pull openjdk@sha256:42783a2d273f0274c9511dd1996a64342914d89197c120b1af499f7b1f73d44e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-jdk-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:ecd094f2f11788d6670c7b2a90b97b2063508d97f3aaa793e682b1f9aefb0ca6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329861443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ecbdcb1384cfc3dbfde6d61810fc150ab778f9064e2dc2a4dc04d31a95975b3`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:47:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:47:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 11 May 2022 05:47:15 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 05:47:15 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 02:16:53 GMT
ENV JAVA_VERSION=19-ea+24
# Sat, 28 May 2022 02:17:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='3f7b2351ee42bc75d9200072d7fd241fcbd9accd60983a245cd005531723e051'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='baa4ad8447e5d179e22d269a8a9f653b86173df964fef78c95aef5c2ca902b7a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 May 2022 02:17:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0162432a49c07aa492d3e1031af58a9a9f9b22acde859829434e5a54d019aa1c`  
		Last Modified: Wed, 11 May 2022 01:58:46 GMT  
		Size: 51.8 MB (51843657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c991e290c00eaf78c3b16a504803042009e8ab196f4d572d415dc6916274f0c2`  
		Last Modified: Wed, 11 May 2022 05:59:23 GMT  
		Size: 13.9 MB (13921435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f552835aa8a1f014dbe04c8b19b52b579e7c1e9a547914f1efbbce1ab1e8b13`  
		Last Modified: Sat, 28 May 2022 02:28:54 GMT  
		Size: 195.8 MB (195804690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-jdk-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:dc9f026d0597ee890dc9ee75ac37d70acdb84c8cce0510dee798dc84a6e537fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.3 MB (328258588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b804999d63db3bf867ac467d3ee2fa09b55715ecb721d1b45b3b13705e251e`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 11:07:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:46:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:46:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Sat, 28 May 2022 16:46:24 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 16:46:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 16:46:26 GMT
ENV JAVA_VERSION=19-ea+24
# Sat, 28 May 2022 16:46:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='3f7b2351ee42bc75d9200072d7fd241fcbd9accd60983a245cd005531723e051'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='baa4ad8447e5d179e22d269a8a9f653b86173df964fef78c95aef5c2ca902b7a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 May 2022 16:46:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfac45ba23f255c176d3688a882854cfc56b2e822c56e0eb0d91ecc8bad25f`  
		Last Modified: Sat, 28 May 2022 11:18:40 GMT  
		Size: 52.2 MB (52174936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b944756973e115bb0bf3d5ee9ec6ed297bf653784c238a06bcb50f98e5f887`  
		Last Modified: Sat, 28 May 2022 17:01:16 GMT  
		Size: 14.7 MB (14670966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c44cced0ecaa91b44b7307518521c3cbc7e43a87ec3c11757d29677e15a6a93`  
		Last Modified: Sat, 28 May 2022 17:01:31 GMT  
		Size: 194.7 MB (194696502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
