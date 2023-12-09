## `openjdk:22-bullseye`

```console
$ docker pull openjdk@sha256:b0c3e0385e53daadafc498b47c292d501310c2637fba7f16fca3a46f9da67f66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:cce87fc3dd5f51c191868797edb7281e4c770f751e7bd11e0a86ed6ddeebbe72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344761435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974260b0a0955032b79f39b86504a5c58f6cbfe5790e05f1c065ef7907a9d004`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:54:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:21:18 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Wed, 22 Nov 2023 00:21:18 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Nov 2023 00:21:18 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 20:55:59 GMT
ENV JAVA_VERSION=22-ea+26
# Fri, 01 Dec 2023 20:56:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='65f135f44a1f33848f9d8398b7773807cf90eeec08d6ec8e2a9b44d81b7b6d99'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='3933a8d405ab7f0293ecd4351177e731f1eacd1a96ee3f0528b9157940581ce2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 01 Dec 2023 20:56:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b1e60e9d5a0f16eb1f998245666f7a64a44f8b1f2317bd31e8a658150c23d3`  
		Last Modified: Tue, 21 Nov 2023 10:02:45 GMT  
		Size: 54.6 MB (54595728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cbbdd2ce15de9bf78b6a0a0cb14da256c39d2cf101ad4bf4e3c5fab2db244`  
		Last Modified: Wed, 22 Nov 2023 00:22:45 GMT  
		Size: 14.1 MB (14074079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215d5a0bc4cb78f35ff793f58b5a1415fde00c09fbb76305809de78e6d2aa631`  
		Last Modified: Fri, 01 Dec 2023 20:59:54 GMT  
		Size: 205.3 MB (205269478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:a3e1baa7439b301aec22108a294ae48a82b5f6beb2d225ebebe4296b046506fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.6 MB (340577082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9f6f6306b63186ca8899f1e086896aac06f4cb1df88878253871096892c494`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:59:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:30:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:30:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 21 Nov 2023 10:30:04 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:30:05 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 23:24:41 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 23:24:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 08 Dec 2023 23:24:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e860a4a6ca9e583881322c2e78baef1911e4d61bc607563e8ad9891e2d91f9`  
		Last Modified: Tue, 21 Nov 2023 08:07:01 GMT  
		Size: 15.8 MB (15750113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a9d2006a8ea812285a7be34dfc82465b2a592d6217f4d385d373c298de4642`  
		Last Modified: Tue, 21 Nov 2023 08:07:16 GMT  
		Size: 54.7 MB (54700129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c760939ab4cb4a53886cfd8f14b2561a79fe7a18c4d1fec23e694cf58a8e4136`  
		Last Modified: Tue, 21 Nov 2023 10:32:16 GMT  
		Size: 15.5 MB (15529977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6837556de3f7d1d53547d2d674cd9c3b6e42089a4839f45b92d6674a8bf208e6`  
		Last Modified: Fri, 08 Dec 2023 23:28:16 GMT  
		Size: 200.9 MB (200888991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
