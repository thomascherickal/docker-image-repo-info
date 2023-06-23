## `openjdk:22-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:be7e9e7f435e3dac5b0bfd5b769fe241f3b9e5244b649e18f7acf8ad435594ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:e9527ee9cf3ef918733b2a5bd36519910e77433891fbfad08ff7ded997df1dc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.0 MB (238012761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13adf9b4ce564ffa1a7dfb14b775747f03f156403e14d58a8a87faecbecfd4f`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:19:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:19:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 13 Jun 2023 07:19:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:19:25 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 00:27:04 GMT
ENV JAVA_VERSION=22-ea+3
# Fri, 23 Jun 2023 00:27:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='6541c5f5f08ec100af327c36768e302185851f548f6c33d1fe26250133998d5a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='e94529988d1c61d552981cc44896e13a1c49f3720567b2a92ad103f24291a167'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:27:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454a143e8504247dc2e9e60b33533bee1b7a6ce927b0222b0354c9ab465ce3bf`  
		Last Modified: Tue, 13 Jun 2023 07:22:50 GMT  
		Size: 1.6 MB (1582441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e91c13456c462b77af64264490a4b96acbcf0623679cc02e185a87a89850d`  
		Last Modified: Fri, 23 Jun 2023 00:33:02 GMT  
		Size: 205.0 MB (205012910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9dcdf356288b7a5efd0380797fedde411543401a6ddf2c0491b7919e5d21e886
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234934884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc956af8ca7de4b4374f299164daefd88e8d896075adc68c26afb731d45b6dd`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:38:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:38:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 13 Jun 2023 04:38:58 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:38:58 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jun 2023 01:14:47 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:15:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='d759c4f3b3cf116701356fb6276cbe5cebac2ff8fbc88e7ca0c10db5c659bf0b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='b60aa1790dc7fa69e983498162b3e0cd883ddc0d89319529cf9dd381b3b04ded'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 21 Jun 2023 01:15:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dc0b678bee14b591fc8dcf5858d219d0fce4abb02971967b35484ea1bfdd40`  
		Last Modified: Tue, 13 Jun 2023 04:42:13 GMT  
		Size: 1.6 MB (1566460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136ca618beb8de99e2645a226cb890bddabfecb0056f3cd02a710f86f65c44da`  
		Last Modified: Wed, 21 Jun 2023 01:20:47 GMT  
		Size: 203.3 MB (203305590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
