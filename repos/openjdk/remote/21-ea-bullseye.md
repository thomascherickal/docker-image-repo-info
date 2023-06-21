## `openjdk:21-ea-bullseye`

```console
$ docker pull openjdk@sha256:059b0fc49c0d51b35211b0d66ff4f9af7dfb7962b94e1c4bf5d6ddc57e0980a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:6e2015c19aaffcad6b7210e22836bdf782961f8bf48508a3f92d3d45329dd153
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.4 MB (343412413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d4c440f537dae721abe846c79af7a3ed791f5c0093e74f9ae876a87e620d8a9`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:19:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:20:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 07:20:35 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:20:36 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:15:12 GMT
ENV JAVA_VERSION=21-ea+27
# Wed, 21 Jun 2023 01:15:22 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='686f2ed6faecd9b5be0306df695bafa576758f00efc51b2250a8044a31ddc9af'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6b6f664146527de70f9dcb2d424cf91c6429a41c6e19e9b940819fdfc73aba4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:15:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4d59f9abaeb4efe1c66ff2176044e93912966342d76d025b6d1a2a37dde7a`  
		Last Modified: Tue, 13 Jun 2023 03:37:49 GMT  
		Size: 54.6 MB (54585023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b6071e5acc46917aa272d6eccdeb02e82f41fada3c7c2a4fb0d54dcab17637`  
		Last Modified: Tue, 13 Jun 2023 07:22:22 GMT  
		Size: 14.1 MB (14071943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098b46e30d828bd1b189f0b83845debd8c4b8ede5f73cf53eaba945a1cf10b0`  
		Last Modified: Wed, 21 Jun 2023 01:23:08 GMT  
		Size: 203.9 MB (203939953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5965d466207644ebd5e729212c5f02cfa40b822ffb67877a9a4c5b59c88be469
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.9 MB (341940036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0243493e7046107290b180c57dedede93aded5a9ac51620ad8b7c2a7c1529e6`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:38:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:40:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 04:40:03 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:40:03 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:16:08 GMT
ENV JAVA_VERSION=21-ea+27
# Wed, 21 Jun 2023 01:16:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='686f2ed6faecd9b5be0306df695bafa576758f00efc51b2250a8044a31ddc9af'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6b6f664146527de70f9dcb2d424cf91c6429a41c6e19e9b940819fdfc73aba4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:16:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b90602383b5196ae0f8744277182f671de6f12c55664a9f36b274ab9266b5cc`  
		Last Modified: Tue, 13 Jun 2023 03:08:47 GMT  
		Size: 54.7 MB (54676037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9763270a318f4900a86c9cd1703dbeac7939447c20ca52598ccbe2f05fabf9a1`  
		Last Modified: Tue, 13 Jun 2023 04:41:48 GMT  
		Size: 15.5 MB (15528952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d92fd90b4903d60814e7e7c696781a86b3f163f68de013bd0127028e113f02d`  
		Last Modified: Wed, 21 Jun 2023 01:23:30 GMT  
		Size: 202.3 MB (202284348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
