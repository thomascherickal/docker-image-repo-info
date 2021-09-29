## `clojure:openjdk-16-buster`

```console
$ docker pull clojure@sha256:e4ccbbce6faba61c2113cdc5ddf41fbcdbd4b20e54a9a33a9f1e9650fc0a17b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-buster` - linux; amd64

```console
$ docker pull clojure@sha256:cf29aedfd56c8ef198fc87a48180112c66a3f2d9a94452a6b912709c197e5443
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335033162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a96844ba9d83592596c6a3db8dbf67bc3174a9f75bba259a831fb65510674b`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:32 GMT
ADD file:948d0998410ef6681d723219eb1dfb4a7d804228e03d84bb296f0d3c8826dd92 in / 
# Fri, 03 Sep 2021 01:21:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:33:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:35:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 03 Sep 2021 08:35:49 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:35:50 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:35:50 GMT
ENV JAVA_VERSION=16.0.2
# Fri, 03 Sep 2021 08:36:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Sep 2021 08:36:01 GMT
CMD ["jshell"]
# Sat, 04 Sep 2021 09:59:55 GMT
ENV LEIN_VERSION=2.9.6
# Sat, 04 Sep 2021 09:59:55 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 04 Sep 2021 09:59:55 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 10:00:02 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Sat, 04 Sep 2021 10:00:02 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Sep 2021 10:00:02 GMT
ENV LEIN_ROOT=1
# Sat, 04 Sep 2021 10:00:06 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Sat, 04 Sep 2021 10:00:06 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:8f04e8168e3873638397ca4beb7d8484b150eca0d10fe1b033a125202ba57692`  
		Last Modified: Fri, 03 Sep 2021 01:27:52 GMT  
		Size: 50.4 MB (50435893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e5f66f5d0e1c97622f33d44fb04efb42bd3562bdc3482537d121040c789f9a`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 7.8 MB (7833606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c8f1c77d6674046d7deb41be1ca07f25cb43fd67f87e879ee79cc6586087f0`  
		Last Modified: Fri, 03 Sep 2021 06:40:37 GMT  
		Size: 10.0 MB (9997249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5095cab277710f0c2883844158323ad986c763ffc37353ddff874dd85585d9b6`  
		Last Modified: Fri, 03 Sep 2021 06:40:55 GMT  
		Size: 51.8 MB (51840968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee27e112836c56c7a7f0e8a1986512005c433ddddbe7aaff39133b826a04844`  
		Last Modified: Fri, 03 Sep 2021 08:50:02 GMT  
		Size: 13.9 MB (13921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2cedb39ebd801010b738a4c4d9577e4220cae9ba14945133fd8136c3de5a20`  
		Last Modified: Fri, 03 Sep 2021 08:56:00 GMT  
		Size: 184.9 MB (184921478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3012239182efa8ced9ce4bc2f062e1ee4f1f6f1308e5f9a3c0660462647ffa9`  
		Last Modified: Sat, 04 Sep 2021 10:12:44 GMT  
		Size: 11.9 MB (11878989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9e7920e2dff58e0791a6c2b877b267c29844bb65e56f4a1b68529fe8823353`  
		Last Modified: Sat, 04 Sep 2021 10:12:44 GMT  
		Size: 4.2 MB (4203719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4e7a3d27c6db82f28989f6152fa4dc89797b31048079d7f05ee0fe025969e243
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.2 MB (329188882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dd041900072d388bb1eece931ea062593f949088d46d325b7b1675fec0b9ae8`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:43:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:46:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 28 Sep 2021 05:46:36 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:46:36 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:46:36 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 28 Sep 2021 05:46:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:46:45 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:16:05 GMT
ENV LEIN_VERSION=2.9.7
# Wed, 29 Sep 2021 02:16:05 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 29 Sep 2021 02:16:05 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:16:16 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "f78f20d1931f028270e77bc0f0c00a5a0efa4ecb7a5676304a34ae4f469e281d *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -r "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Wed, 29 Sep 2021 02:16:17 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 02:16:17 GMT
ENV LEIN_ROOT=1
# Wed, 29 Sep 2021 02:16:20 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 29 Sep 2021 02:16:20 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619d0551980848579ec373733f2fb35c7deddf13e6e56747ddf13dedc6ddbf6b`  
		Last Modified: Tue, 28 Sep 2021 02:26:20 GMT  
		Size: 52.2 MB (52167859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396bc1f0aead28c26643cc8ce4fbe908f91e1f61bd89998566f8fc1c8dfba868`  
		Last Modified: Tue, 28 Sep 2021 06:05:30 GMT  
		Size: 14.7 MB (14673473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a16548aa0b730c94f00e8a56ffb5bac40f0015fc240d6efd5b8f75df7272b5`  
		Last Modified: Tue, 28 Sep 2021 06:11:51 GMT  
		Size: 179.3 MB (179297621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb12ff92d1187be79de4a26840a021dc35ea265e91af43e5e6cb1922806250b`  
		Last Modified: Wed, 29 Sep 2021 02:44:47 GMT  
		Size: 11.9 MB (11940161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042dcc6e4a87bdc7dd8f25708f9c6a206cdd10f2e5380c67a04f8726b745f4f8`  
		Last Modified: Wed, 29 Sep 2021 02:44:46 GMT  
		Size: 4.2 MB (4207217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
