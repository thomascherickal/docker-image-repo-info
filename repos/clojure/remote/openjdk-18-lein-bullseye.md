## `clojure:openjdk-18-lein-bullseye`

```console
$ docker pull clojure@sha256:3581615eeb593898190fdbf72fcdf4f79211af1a21cb3675f8334cad0e2f77e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f0e9c4813e0feb8ee19c55f42dd75f7493e8cb3a0453066e2122b2bf6c248e6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.7 MB (343689674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a3ae6869839e27982bca60f0fd9da000ebb583977c19a7236ed11ef507012a`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:30 GMT
ADD file:aea313ae50ce6474a3df142b34d4dcba4e7e0186ea6fe55389cb2ea903b9ebbb in / 
# Tue, 12 Oct 2021 01:20:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:42:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:27:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 12 Oct 2021 16:27:22 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:27:22 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:27:23 GMT
ENV JAVA_VERSION=18-ea+18
# Tue, 12 Oct 2021 16:27:36 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/18/GPL/openjdk-18-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='425b4f9afe439b4690593e5f78e27b6687525114a66f652c285a7dcca95b1961'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/18/GPL/openjdk-18-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='af5b0d66cf7c4f7450066fd67dbb0d48c17bcc5ab8ddb105cf7fe66176427f87'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 12 Oct 2021 16:27:36 GMT
CMD ["jshell"]
# Wed, 13 Oct 2021 13:20:27 GMT
ENV LEIN_VERSION=2.9.7
# Wed, 13 Oct 2021 13:20:27 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 13 Oct 2021 13:20:28 GMT
WORKDIR /tmp
# Wed, 13 Oct 2021 13:20:34 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "f78f20d1931f028270e77bc0f0c00a5a0efa4ecb7a5676304a34ae4f469e281d *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -r "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Wed, 13 Oct 2021 13:20:35 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 13 Oct 2021 13:20:35 GMT
ENV LEIN_ROOT=1
# Wed, 13 Oct 2021 13:20:38 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 13 Oct 2021 13:20:39 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:bb7d5a84853b217ac05783963f12b034243070c1c9c8d2e60ada47444f3cce04`  
		Last Modified: Tue, 12 Oct 2021 01:25:37 GMT  
		Size: 54.9 MB (54917520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02b617c6a8c415a175f44d7e2c5d3b521059f2a6112c5f022e005a44a759f2d`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 5.2 MB (5153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e17419b7ee61bbd89c2f0d2833a99cf45e594257d15cb567e4cf7771ce34a`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 10.9 MB (10871935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d2d81226a43a97871acd5afb7e8aabfad4d6b62ae1709c870df3ee230bc3f5`  
		Last Modified: Tue, 12 Oct 2021 15:53:13 GMT  
		Size: 54.6 MB (54567761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae81fdbbf50b4f75c539f7e4ab9fa83b3fbad9f297ed467c5b05cae3a83872`  
		Last Modified: Tue, 12 Oct 2021 16:42:23 GMT  
		Size: 14.1 MB (14071834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0852410489090ea2db39b26b72e19253e58dc2f02c15cffc92f709b406be1437`  
		Last Modified: Tue, 12 Oct 2021 16:42:36 GMT  
		Size: 188.0 MB (187967661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c838d3674caada65f3047f8667281428770e400b35bdce49d86e0ffa0bab33`  
		Last Modified: Wed, 13 Oct 2021 13:40:40 GMT  
		Size: 11.9 MB (11932465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c03859fff6f2f6bd3ffbc73d751532521a74603f2a727fab55a73c3d70e0b53`  
		Last Modified: Wed, 13 Oct 2021 13:40:39 GMT  
		Size: 4.2 MB (4207225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a7591051f3e2ff46ba16b52b844df313bb53cd6f7ad0539ad5d0c50c7505b3a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342652389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:767b49408bac5b0ddffb64b6855877cb05bdaeaa6cb3700af83e003b4135e4fa`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:04 GMT
ADD file:1529ae12e334fd992892d3fb97c103297cff7e0115b0475bec4c093939a2bff7 in / 
# Tue, 12 Oct 2021 01:41:04 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:10:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:10:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:10:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:00:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:00:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Wed, 13 Oct 2021 06:00:25 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:00:26 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 00:06:03 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:06:16 GMT
CMD ["jshell"]
# Sat, 16 Oct 2021 00:47:10 GMT
ENV LEIN_VERSION=2.9.7
# Sat, 16 Oct 2021 00:47:10 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 16 Oct 2021 00:47:11 GMT
WORKDIR /tmp
# Sat, 16 Oct 2021 00:47:17 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "f78f20d1931f028270e77bc0f0c00a5a0efa4ecb7a5676304a34ae4f469e281d *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -r "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Sat, 16 Oct 2021 00:47:18 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 16 Oct 2021 00:47:19 GMT
ENV LEIN_ROOT=1
# Sat, 16 Oct 2021 00:47:23 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Sat, 16 Oct 2021 00:47:23 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:1c47a423366578e5ce665d03788914bf0459485a627a27896fa9c5663ce55cdf`  
		Last Modified: Tue, 12 Oct 2021 01:47:41 GMT  
		Size: 53.6 MB (53603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580c36351f836fd83ee4aee909834823b15f90ce0ec580f869717dc3679a020b`  
		Last Modified: Tue, 12 Oct 2021 02:18:53 GMT  
		Size: 5.1 MB (5142731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b655be758028f8234aab1f828dc2f79ee5abf3ce0a85560430b5f7c806367d1`  
		Last Modified: Tue, 12 Oct 2021 02:18:53 GMT  
		Size: 10.9 MB (10872848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831021d515bc09a375e4761b088d68a71b5db76ecfcc814957479d29faa6bd38`  
		Last Modified: Tue, 12 Oct 2021 02:19:16 GMT  
		Size: 54.7 MB (54668919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc2b4d8f164c1fe58711eaaff191652e3ba3bfb191e87c8022e38f4e5881ad`  
		Last Modified: Wed, 13 Oct 2021 06:24:52 GMT  
		Size: 15.5 MB (15525123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bd95a8e69520d8c222e0f2a8029cea51a6fe2f85d7a9189c6ebf273bf262ba`  
		Last Modified: Sat, 16 Oct 2021 00:19:39 GMT  
		Size: 186.9 MB (186940319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb7567c998f113634b3d7be7c3196f351d16f910e4de4e7160a10fedd3a23f2`  
		Last Modified: Sat, 16 Oct 2021 00:58:06 GMT  
		Size: 11.7 MB (11692342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e37addc8aa583249e7849f28d4a9b112ef1777d3e854d6944de324e79f244`  
		Last Modified: Sat, 16 Oct 2021 00:58:06 GMT  
		Size: 4.2 MB (4207092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
