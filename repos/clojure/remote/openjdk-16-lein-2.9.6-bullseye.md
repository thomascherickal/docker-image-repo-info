## `clojure:openjdk-16-lein-2.9.6-bullseye`

```console
$ docker pull clojure@sha256:470b59a45e7b3351ecb7878a3b21946ffff364cb37d70505f3594bb97e180735
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-16-lein-2.9.6-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:79f7b7034d06489acc8fea69f08cb1321eb94aeb32dc37cd82890f664bce1ef2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.6 MB (340583925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0a021043890dc26de0e72f40afa3b0f30ba63321dbaa8b20da87fd6c4357985`
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
# Fri, 03 Sep 2021 08:35:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 03 Sep 2021 08:35:12 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:35:12 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:35:12 GMT
ENV JAVA_VERSION=16.0.2
# Fri, 03 Sep 2021 08:35:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Sep 2021 08:35:23 GMT
CMD ["jshell"]
# Thu, 09 Sep 2021 19:29:23 GMT
ENV LEIN_VERSION=2.9.6
# Thu, 09 Sep 2021 19:29:23 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Sep 2021 19:29:23 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:29:29 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Thu, 09 Sep 2021 19:29:30 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Sep 2021 19:29:30 GMT
ENV LEIN_ROOT=1
# Thu, 09 Sep 2021 19:29:33 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Sep 2021 19:29:33 GMT
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
	-	`sha256:c0c965e8fb8dc18667119f0e6e2bf13db24c86078a1ab58e95b4bc0279e63314`  
		Last Modified: Fri, 03 Sep 2021 08:54:10 GMT  
		Size: 184.9 MB (184917708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511c2952dc8ebe643114e35f22b201d2a51284f978f64315e9e127b60a7caeae`  
		Last Modified: Thu, 09 Sep 2021 19:46:40 GMT  
		Size: 11.9 MB (11872315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1b082ec355385561791ed8dad41e55c3cfd8e940151ae857678313438219fc`  
		Last Modified: Thu, 09 Sep 2021 19:46:39 GMT  
		Size: 4.2 MB (4203732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
