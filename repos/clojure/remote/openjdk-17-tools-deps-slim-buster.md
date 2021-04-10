## `clojure:openjdk-17-tools-deps-slim-buster`

```console
$ docker pull clojure@sha256:613b8ca66c65c167d14c47da8d132ec631f7c678f33867515c9aecc173b0a126
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-tools-deps-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:cec3e4c86fd261a30711da9e4bd88c0745479fa7710e9ef469594e7a9328305b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255124423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:652d874346d168d179a2730f2b752f2e27a816cb2d531f8badf2bb1e7457c159`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:41:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 31 Mar 2021 05:41:07 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 05:41:07 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:55:52 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:56:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:56:07 GMT
CMD ["jshell"]
# Fri, 09 Apr 2021 19:35:31 GMT
ENV CLOJURE_VERSION=1.10.3.822
# Fri, 09 Apr 2021 19:35:31 GMT
WORKDIR /tmp
# Fri, 09 Apr 2021 19:35:47 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ebc820fe0e74de4bd77e6d5bd7db4a262ec1902efdf4d0553309485afcd75abf *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Apr 2021 19:35:48 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875a154571f097680e56e5acc7383853036fac0e52855a4dd4fa740bfabf3f95`  
		Last Modified: Wed, 31 Mar 2021 05:52:39 GMT  
		Size: 3.3 MB (3268916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66cb6c029e779c6f74df0e401df856a138f1dc6ab2ec879fa41e0e2dbc800c1`  
		Last Modified: Fri, 09 Apr 2021 19:03:08 GMT  
		Size: 186.3 MB (186345208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7932505ca086988e6363057393d66f90159f9bcf628dd1ca181800c881315312`  
		Last Modified: Fri, 09 Apr 2021 19:40:17 GMT  
		Size: 38.4 MB (38371006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-tools-deps-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5d7c7de7eb9639fa386ec07f587cb978884ba9c1d5663329be369bba309f064c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.3 MB (249282286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ced706664506d2b6824efcf4e0b5445d04f2d14eaa6446ccce2ec8f472e3b1`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:15 GMT
ADD file:a9b57ded2400fc7f60ea40e5ccdd3e9bf0f72acfcc47223ceb66b4fa16955059 in / 
# Tue, 30 Mar 2021 21:47:16 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:39:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:39:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 31 Mar 2021 01:39:30 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 01:39:32 GMT
ENV LANG=C.UTF-8
# Fri, 09 Apr 2021 18:42:43 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:43:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='a53ace955971ef1ad745c2e9fef7f76b57b51d57e7076dd3a55243ab65febf87'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/17/GPL/openjdk-17-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='ccd8ee7bb908835e697ebae8dbe38d2cf68d9f266e2d9787bdf34d26da30e45b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 09 Apr 2021 18:43:32 GMT
CMD ["jshell"]
# Fri, 09 Apr 2021 19:47:42 GMT
ENV CLOJURE_VERSION=1.10.3.822
# Fri, 09 Apr 2021 19:47:43 GMT
WORKDIR /tmp
# Fri, 09 Apr 2021 19:48:22 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ebc820fe0e74de4bd77e6d5bd7db4a262ec1902efdf4d0553309485afcd75abf *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Apr 2021 19:48:24 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:6fcf2156bc23db75595b822b865fbc962ed6f4521dec8cae509e66742a6a5ad3`  
		Last Modified: Tue, 30 Mar 2021 21:54:27 GMT  
		Size: 25.9 MB (25904513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde6667c188c81fcddee021ccbb3e054ebe83350fd4609e17a3d37f0ec7f9d`  
		Last Modified: Wed, 31 Mar 2021 01:49:41 GMT  
		Size: 3.1 MB (3118896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8b16884924ead4ccd567c020ee1730887bce95b7e3280b7c55dd93d97ac2b0`  
		Last Modified: Fri, 09 Apr 2021 18:49:26 GMT  
		Size: 182.4 MB (182393391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2eeef68ba97e1dc4915741b4f5478f11529ec5a2a3a8ca5e53e35226ad0a6e5`  
		Last Modified: Fri, 09 Apr 2021 19:52:07 GMT  
		Size: 37.9 MB (37865486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
