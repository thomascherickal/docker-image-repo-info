## `clojure:openjdk-8-lein-buster`

```console
$ docker pull clojure@sha256:4f246e788d2f9aab4ddd4679105a769e6fc8e4af58255565f2d5ef52f5be8171
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-8-lein-buster` - linux; amd64

```console
$ docker pull clojure@sha256:6b2baef8f508b31449648ca81423c86b628a9672bf166c227b6ce43738855677
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.5 MB (247468699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d758f1da3c7336467ed943ece25af7ce662e5a29b844a660e30b437202e0fbd3`
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
# Fri, 03 Sep 2021 08:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:41:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 03 Sep 2021 08:41:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 08:41:52 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:41:52 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:41:53 GMT
ENV JAVA_VERSION=8u302
# Fri, 03 Sep 2021 08:41:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 04 Sep 2021 09:55:46 GMT
ENV LEIN_VERSION=2.9.6
# Sat, 04 Sep 2021 09:55:46 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 04 Sep 2021 09:55:46 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 09:55:53 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Sat, 04 Sep 2021 09:55:53 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Sep 2021 09:55:53 GMT
ENV LEIN_ROOT=1
# Sat, 04 Sep 2021 09:55:56 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Sat, 04 Sep 2021 09:55:57 GMT
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
	-	`sha256:9ffbb70985069a18b6cb99f75ac2e6b3210b011fdd55f60dfa98ca3389d566c7`  
		Last Modified: Fri, 03 Sep 2021 08:59:03 GMT  
		Size: 5.3 MB (5286452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc339866e15682e2b6469e399f0ac4dc764f7affe5027f7ab6793e93863800b7`  
		Last Modified: Fri, 03 Sep 2021 09:06:25 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68bf95a3f96b7f824f6571aa054358b628fba5a2df2ff91cd8522a309f53989`  
		Last Modified: Fri, 03 Sep 2021 09:06:38 GMT  
		Size: 106.0 MB (105992983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f66437a3ae9757544d415e64f19234ab8a23817f40e08d485a99bdb0df99563`  
		Last Modified: Sat, 04 Sep 2021 10:08:01 GMT  
		Size: 11.9 MB (11877623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c74c85718c345f3d69be2b6144939b4a8c372b7c756e60e07d2d770065bffe`  
		Last Modified: Sat, 04 Sep 2021 10:08:01 GMT  
		Size: 4.2 MB (4203717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-8-lein-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4e19dcff86f5e1fee53fbb990800b245cb6eed4e6bd5e45ed020e5fd57b6bb60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245503607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4c8bf134aa23c5676eed39fc2c7531853333a07a56ed4fa3aa7ab0a71944ea`
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
# Tue, 28 Sep 2021 05:49:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:53:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 05:53:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 05:53:05 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:53:05 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:53:05 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 05:53:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 02:10:28 GMT
ENV LEIN_VERSION=2.9.7
# Wed, 29 Sep 2021 02:10:29 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 29 Sep 2021 02:10:29 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:10:35 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "f78f20d1931f028270e77bc0f0c00a5a0efa4ecb7a5676304a34ae4f469e281d *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -r "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Wed, 29 Sep 2021 02:10:35 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 02:10:36 GMT
ENV LEIN_ROOT=1
# Wed, 29 Sep 2021 02:10:39 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 29 Sep 2021 02:10:40 GMT
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
	-	`sha256:35fe21140f0f683646c2614ecd23f7f6c98fc637a7fcd891cb22e57af260bde2`  
		Last Modified: Tue, 28 Sep 2021 06:15:02 GMT  
		Size: 5.3 MB (5277730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf33a77085a184eb2cf52d954820c5b8adf08e1a11144feabbf237be5aafa70`  
		Last Modified: Tue, 28 Sep 2021 06:19:36 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c8ad9cd425860704e41039588de3c94e612f8966322724cc836194261a156`  
		Last Modified: Tue, 28 Sep 2021 06:19:47 GMT  
		Size: 105.0 MB (105009360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd69855ab0728b41690b77af87c74c91f8d272fe612664d78229332fe62d0ca1`  
		Last Modified: Wed, 29 Sep 2021 02:40:27 GMT  
		Size: 11.9 MB (11938671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010d5ca6ef658a8e038b23e67039586aa7948dce4326cab4b5e81da797e4ad97`  
		Last Modified: Wed, 29 Sep 2021 02:40:26 GMT  
		Size: 4.2 MB (4207228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
