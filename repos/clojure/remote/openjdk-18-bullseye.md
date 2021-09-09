## `clojure:openjdk-18-bullseye`

```console
$ docker pull clojure@sha256:ccc08b6bbdd74f61362d8217686fdd09bb9595ac8f4cb23b145a1dd7faab3e77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:5ac0c00c7fd943ed96992b948331d42c5df09162e272fa0147c90408b80cde34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.2 MB (343177128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409d242511d97a553d85e35b733baeeedd1cd49f219a928ff64bb866aac574e4`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:07 GMT
ADD file:1fedf68870782f1b44cd50691444aab4061cc0c70f24e5fabe9c562cc46eb9af in / 
# Fri, 03 Sep 2021 01:21:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:31:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:31:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:30:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:30:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:30:45 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:30:46 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 09:42:04 GMT
ENV JAVA_VERSION=18-ea+13
# Sat, 04 Sep 2021 09:42:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='396584ea555ad439176473f4e22c146817290a8eeaad02e3072dfb398ba786e0'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='4601ee9811daa3bf282753e1fa6b8caffd869d0e56c9acfe95e1670bc580ed34'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Sep 2021 09:42:14 GMT
CMD ["jshell"]
# Thu, 09 Sep 2021 19:33:24 GMT
ENV LEIN_VERSION=2.9.6
# Thu, 09 Sep 2021 19:33:24 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Sep 2021 19:33:24 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:33:31 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Thu, 09 Sep 2021 19:33:31 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Sep 2021 19:33:31 GMT
ENV LEIN_ROOT=1
# Thu, 09 Sep 2021 19:33:35 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Sep 2021 19:33:35 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:955615a668ce169f8a1443fc6b6e6215f43fe0babfb4790712a2d3171f34d366`  
		Last Modified: Fri, 03 Sep 2021 01:26:55 GMT  
		Size: 54.9 MB (54926871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2756ef5f69a5190f4308619e0f446d95f5515eef4a814dbad0bcebbbbc7b25a8`  
		Last Modified: Fri, 03 Sep 2021 06:39:22 GMT  
		Size: 5.2 MB (5153100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ea9f2bd51e53a455297e0631e18a72a86d7e2c8e1807176e80f991bde5d64`  
		Last Modified: Fri, 03 Sep 2021 06:39:23 GMT  
		Size: 10.9 MB (10871687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0a22ee906271a6ce9ddd1754fdd7d3b59078e0b57b6cc054c7ed7ac301587`  
		Last Modified: Fri, 03 Sep 2021 06:39:45 GMT  
		Size: 54.6 MB (54566834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b79c82cab03ddf5fc88cf1ab0550217980b866ec12c52b0f16751bc45be87b6`  
		Last Modified: Fri, 03 Sep 2021 08:48:24 GMT  
		Size: 14.1 MB (14071678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62677b7a9b3a7197ce1a9feb62c0aa14ea83397d3263ce8cb5101bc1bbba178b`  
		Last Modified: Sat, 04 Sep 2021 09:50:28 GMT  
		Size: 187.5 MB (187510947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f744070c0cce4b915d01e131952956b2a433f7a0814a030e5fc6d7e361f33ba`  
		Last Modified: Thu, 09 Sep 2021 19:50:05 GMT  
		Size: 11.9 MB (11872318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b776e78b44a137ba7737ab70b61f9c0b3a8ba89f40e9cd20b92e62d70d113df8`  
		Last Modified: Thu, 09 Sep 2021 19:50:05 GMT  
		Size: 4.2 MB (4203693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
