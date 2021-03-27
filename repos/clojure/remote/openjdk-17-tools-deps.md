## `clojure:openjdk-17-tools-deps`

```console
$ docker pull clojure@sha256:4214299024e33760ef0dacd3d45e3361786250fd86cdc344a62b962e924ef068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-tools-deps` - linux; amd64

```console
$ docker pull clojure@sha256:aea91fea9f105dc7280cabd75698d6d1e32f87cd88a479b57d91625afb3f80d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254676030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62c72591b54bec578e63c83fec4e04272eba1cc4bdb33e1066bdbb51e611cdb`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 19:24:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 19:24:33 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 26 Mar 2021 19:24:33 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 19:24:33 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 19:24:33 GMT
ENV JAVA_VERSION=17-ea+15
# Fri, 26 Mar 2021 19:24:48 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='da690c53a8d23b278b4878acf414b0d95ca40dd1533d08ce313589cf1df1c9c3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93178b313750b38e1bbc811b989dcee27d988cb223b30ba829122ecdbd08f403'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 19:24:49 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:12:47 GMT
ENV CLOJURE_VERSION=1.10.3.814
# Fri, 26 Mar 2021 20:12:47 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:13:21 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ea4a943d32496dc2423a529b32a309f2c0365e56ba251d4a56739c5977b906a3 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 26 Mar 2021 20:13:22 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f37f3c8df9c4599e86451848bc7d181558d9106306657ffef1e8a59f44b7f7`  
		Last Modified: Fri, 26 Mar 2021 19:32:50 GMT  
		Size: 3.3 MB (3268744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d64f535a678982062036b0be2acf726821ecb53a9dfe2f57600648194e31c`  
		Last Modified: Fri, 26 Mar 2021 19:33:06 GMT  
		Size: 185.9 MB (185945734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65734296b066860e4b06232a0b877ed1e90972606afbfd206678a6435d289b6e`  
		Last Modified: Fri, 26 Mar 2021 20:23:32 GMT  
		Size: 38.4 MB (38360556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-tools-deps` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5016f60e3c89becf8f24284baa907d267b6adbed7ac9276c374cf9140204a278
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248861684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515edcadaa459cd082d388e819de92a801c8eda09ce4bc3b1b7f9d3ffdeda3b2`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 19:43:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 19:43:15 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 26 Mar 2021 19:43:15 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 19:43:16 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 19:43:17 GMT
ENV JAVA_VERSION=17-ea+15
# Fri, 26 Mar 2021 19:43:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='da690c53a8d23b278b4878acf414b0d95ca40dd1533d08ce313589cf1df1c9c3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/15/GPL/openjdk-17-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93178b313750b38e1bbc811b989dcee27d988cb223b30ba829122ecdbd08f403'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 19:43:59 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:22:11 GMT
ENV CLOJURE_VERSION=1.10.3.814
# Fri, 26 Mar 2021 20:22:12 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:22:49 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ea4a943d32496dc2423a529b32a309f2c0365e56ba251d4a56739c5977b906a3 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 26 Mar 2021 20:22:51 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d8de9377aa4bd4c66d812b6226ebe8ebcb1dbbbdf3be6e3e9d0ea7363e0d3`  
		Last Modified: Fri, 26 Mar 2021 19:50:29 GMT  
		Size: 3.1 MB (3118857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a684536826257d175f2a7600e0046e7e7d2c61220d1c7441161448cd4f4a5`  
		Last Modified: Fri, 26 Mar 2021 19:50:54 GMT  
		Size: 182.0 MB (182021333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c6429b68454f3dd1c94be0f9a2e22c72e7d5f1be3564848e1d0d7f4d1a7f5`  
		Last Modified: Fri, 26 Mar 2021 20:29:27 GMT  
		Size: 37.9 MB (37865110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
