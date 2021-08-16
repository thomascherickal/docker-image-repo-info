## `clojure:openjdk-18-buster`

```console
$ docker pull clojure@sha256:f33cf3b1d9020a39cc782eb4ec12ed753c7e64c0481c677ac28a81e9f78bc2f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-buster` - linux; amd64

```console
$ docker pull clojure@sha256:b2b220d878c89ecef4c33b1368584234fe9b7a4ef150df7220dde1f74dbffdf4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337686529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814148aa891489560b10c36a656220449c940e0f7c52f291278ffc2690028fe7`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:33:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 22 Jul 2021 13:33:13 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:33:13 GMT
ENV LANG=C.UTF-8
# Fri, 13 Aug 2021 17:27:04 GMT
ENV JAVA_VERSION=18-ea+10
# Fri, 13 Aug 2021 17:27:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='f02c5e52c193b349688216e85ab6fb67548861e93d96dd454f74881abfb696b2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6a6ba79485e560d0d7687152a2a1dfa92cbe80871f16eb24b52e01274f9f4f6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Aug 2021 17:27:15 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 20:23:57 GMT
ENV LEIN_VERSION=2.9.6
# Mon, 16 Aug 2021 20:23:57 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Mon, 16 Aug 2021 20:23:58 GMT
WORKDIR /tmp
# Mon, 16 Aug 2021 20:24:04 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Mon, 16 Aug 2021 20:24:05 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 16 Aug 2021 20:24:05 GMT
ENV LEIN_ROOT=1
# Mon, 16 Aug 2021 20:24:08 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Mon, 16 Aug 2021 20:24:08 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4de66c57277180420b7663842bf72269ceeb8ddb3b87e83d9d5a4b708ac740`  
		Last Modified: Thu, 22 Jul 2021 13:43:09 GMT  
		Size: 13.9 MB (13921248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf28cbe84e179afe37b71e900696a26c014994de5713503c8da37ccc9d95fc7`  
		Last Modified: Fri, 13 Aug 2021 17:33:17 GMT  
		Size: 187.6 MB (187575629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862340ff586bf6872ae431633cfb014b4135db94ca0a540497bc837f13edb9a`  
		Last Modified: Mon, 16 Aug 2021 20:31:08 GMT  
		Size: 11.9 MB (11878953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6013584e24a969bb2d2d204347404576b43f9570330b066e2090388dbf19874`  
		Last Modified: Mon, 16 Aug 2021 20:31:07 GMT  
		Size: 4.2 MB (4203704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2d29c70e502222cd55b06be2c526a755570303481e711671b2618d49c51ca8c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.2 MB (336155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d5fa35f5c801da7d5644b2bf5e66dbfd1068348dcc39ede1451ab7c1f20534`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:15:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:15:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Thu, 22 Jul 2021 05:15:12 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 05:15:12 GMT
ENV LANG=C.UTF-8
# Fri, 13 Aug 2021 17:41:21 GMT
ENV JAVA_VERSION=18-ea+10
# Fri, 13 Aug 2021 17:41:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='f02c5e52c193b349688216e85ab6fb67548861e93d96dd454f74881abfb696b2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/10/GPL/openjdk-18-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6a6ba79485e560d0d7687152a2a1dfa92cbe80871f16eb24b52e01274f9f4f6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Aug 2021 17:41:30 GMT
CMD ["jshell"]
# Mon, 16 Aug 2021 20:43:58 GMT
ENV LEIN_VERSION=2.9.6
# Mon, 16 Aug 2021 20:43:58 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Mon, 16 Aug 2021 20:43:58 GMT
WORKDIR /tmp
# Mon, 16 Aug 2021 20:44:10 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Mon, 16 Aug 2021 20:44:10 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 16 Aug 2021 20:44:10 GMT
ENV LEIN_ROOT=1
# Mon, 16 Aug 2021 20:44:13 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Mon, 16 Aug 2021 20:44:13 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967a8f1385966af47c9f250997e3158c319d498adc004c91570f770ceac5045a`  
		Last Modified: Thu, 22 Jul 2021 01:25:24 GMT  
		Size: 52.2 MB (52167528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176877461d089b6f2c205b71c8892552af1b56d6cd599f6db980e3275e7f589c`  
		Last Modified: Thu, 22 Jul 2021 05:29:29 GMT  
		Size: 14.7 MB (14673538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f074c4a88d9841da217b0c38836e1597b7ca617b49eeee9d29cc4fc218619c`  
		Last Modified: Fri, 13 Aug 2021 17:52:44 GMT  
		Size: 186.3 MB (186330378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02b1f96254ceb0f3cfe1a3512f7a33b7ca7bd6f92535bd4d0eca6f6519c4b6`  
		Last Modified: Mon, 16 Aug 2021 20:52:58 GMT  
		Size: 11.9 MB (11878780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dba235865511dd5d748922e81ca0590cdf7d6caef6ccf38cf98f42a9bb41bb9`  
		Last Modified: Mon, 16 Aug 2021 20:52:57 GMT  
		Size: 4.2 MB (4203729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
