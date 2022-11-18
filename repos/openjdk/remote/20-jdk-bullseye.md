## `openjdk:20-jdk-bullseye`

```console
$ docker pull openjdk@sha256:74df245535a36eba26fca53c389769e95e09593c3aa74d46cc4b27aae4b3882d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:f006e152266ff1f7a2ca9c5eb71e188d8af83337949c5fa8a7798a685db01255
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338125708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e833057828f80a0a4a7bab34fa1bf05817bcc6b3c714949ff413e5db5a4700`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 10:23:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:36:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:36:38 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 15 Nov 2022 13:36:38 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 13:36:38 GMT
ENV LANG=C.UTF-8
# Fri, 18 Nov 2022 01:42:08 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:42:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:42:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195ea6a58ca87a18477965a6e6a8623112bde82c5b568a29c56ce4581b6e6695`  
		Last Modified: Tue, 15 Nov 2022 10:31:57 GMT  
		Size: 54.6 MB (54587188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa20b8a2ae1afe12305a84546149fd0097f01dd9e601b127b84405c9a4e7b134`  
		Last Modified: Tue, 15 Nov 2022 13:41:39 GMT  
		Size: 14.1 MB (14073858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac9010d35d1e82a1e5eda05cdd5ab17d227db17d6d7fbe51e8b9ee985993d0a`  
		Last Modified: Fri, 18 Nov 2022 01:47:03 GMT  
		Size: 198.4 MB (198383762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d00c90c97aecc723bb5ce285fdd7b3309476ce430c79209eb4c42b5f33fe7794
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336892258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc44bd389db091b2ebce374d7e8c009dca0a75ee8a1d4dee828caa2c169e2f66`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 05:36:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:59:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 15 Nov 2022 06:59:02 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 06:59:02 GMT
ENV LANG=C.UTF-8
# Fri, 18 Nov 2022 01:58:08 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:58:16 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:58:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e8acfed2a5373bd99b22b5a968d55a148e14bc0e0f51c5cf0d779afefe291`  
		Last Modified: Tue, 15 Nov 2022 05:43:14 GMT  
		Size: 54.7 MB (54683589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f848caae63d0cb0442197d6604f9037220a8910d9c40e2c1b0084926b4377b6`  
		Last Modified: Tue, 15 Nov 2022 07:03:48 GMT  
		Size: 15.5 MB (15529728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b87d51d2f89a39d9d28387164c5f6c276a9f977c3055f5e683f529c1814b350`  
		Last Modified: Fri, 18 Nov 2022 02:02:57 GMT  
		Size: 197.0 MB (196953498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
