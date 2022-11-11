## `openjdk:20-jdk-bullseye`

```console
$ docker pull openjdk@sha256:a0edefb1473cb49c430af6b3e6f682be60ef6efaeb33d8a7f441562199f6718c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:b82a1ed6254f2b48ab6b6743d89cb0389e8c4d20ea6a905eaf3f4d28ba661a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338094187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858cfde4964f8c8ed7158bf9b15b75cf1b6bef3b2ac466852e2a237ff72b9a64`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 09:23:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:07:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:08:00 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 26 Oct 2022 01:08:00 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 00:56:20 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 00:56:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 00:56:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4a4c6caea8801bb0b7377e10220a914da403bc93fa79663cbf2dcf1800b6f1`  
		Last Modified: Tue, 25 Oct 2022 09:47:36 GMT  
		Size: 5.2 MB (5164775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edced8587e6c18412817019074f5e04a8ede4e2fc89d06af13df3f80d78a70d`  
		Last Modified: Tue, 25 Oct 2022 09:47:36 GMT  
		Size: 10.9 MB (10877322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7969cffbf46e6a91291fd76b19ecbe93c03ea4ded0d14042aecb4c0c4211a43`  
		Last Modified: Tue, 25 Oct 2022 09:47:56 GMT  
		Size: 54.6 MB (54586464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0108ba67265c7c92c6282962b524a2be98e41302f7147f1d09a179fd1000d571`  
		Last Modified: Wed, 26 Oct 2022 01:11:38 GMT  
		Size: 14.1 MB (14073886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59fbf39f58868e30f58e2112d1d837929896ce605976dddf1d24630c2f7b585`  
		Last Modified: Fri, 11 Nov 2022 01:01:29 GMT  
		Size: 198.3 MB (198345408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:03c8eaf1308902d47b0d4ae8084abd55016e86ebddb8e6d00cd0c3d931bde404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.8 MB (336846085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ff4bca1911943a6b970c9ab290de0e2009e83c33e256ec79a5939cc01702d6`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 07:59:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:44:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:44:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 26 Oct 2022 00:44:39 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:44:39 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 11:34:09 GMT
ENV JAVA_VERSION=20-ea+23
# Fri, 11 Nov 2022 11:34:22 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Nov 2022 11:34:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d337cb12fd7c6fe341850cd38e880f1806d49a65832c9804b06d00f9032382e0`  
		Last Modified: Tue, 25 Oct 2022 08:30:42 GMT  
		Size: 54.7 MB (54683990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0736831300ed7d1daf6523f91f57ad7cf010209c255cc5312b147a34876518b6`  
		Last Modified: Wed, 26 Oct 2022 00:51:11 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d40ba54959886bdbc48670fd505efe3f6a79c833d990c8a1298fb0aaac45ec8`  
		Last Modified: Fri, 11 Nov 2022 11:39:09 GMT  
		Size: 196.9 MB (196904753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
