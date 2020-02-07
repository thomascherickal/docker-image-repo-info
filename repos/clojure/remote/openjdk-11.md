## `clojure:openjdk-11`

```console
$ docker pull clojure@sha256:e9a5fc27f7250e2c56a3fb224ee95f02af540eb8a34870fe1ea9c0921ec390ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-11` - linux; amd64

```console
$ docker pull clojure@sha256:719af2315ed79ae87b636f53669e2dc27e828191dfa2da7096c5bac5b245af88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.9 MB (328921273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c8bb8338c9bdaa2ff4c68a911dc9c68a27e7c103972a8f2aba9dd4486ccf3e`
-	Default Command: `["lein","repl"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:41 GMT
ADD file:8a9218592e5d736a05a1821a6dd38b205cdd8197c26a5aa33f6fc22fbfaa1c4d in / 
# Sat, 01 Feb 2020 17:23:41 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:33:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:34:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:26:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:26:12 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:26:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sun, 02 Feb 2020 06:26:12 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:26:13 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:26:13 GMT
ENV JAVA_VERSION=11.0.6
# Sun, 02 Feb 2020 06:26:13 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Sun, 02 Feb 2020 06:26:14 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Sun, 02 Feb 2020 06:26:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:26:30 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:35:49 GMT
ENV LEIN_VERSION=2.9.1
# Sun, 02 Feb 2020 21:35:49 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:35:49 GMT
WORKDIR /tmp
# Fri, 07 Feb 2020 03:35:44 GMT
RUN mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha1sum lein-pkg && echo "93be2c23ab4ff2fc4fcf531d7510ca4069b8d24a *lein-pkg" | sha1sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver pool.sks-keyservers.net --recv-key 2B72BF956E23DE5E830D50F6002AF007D1A7CC18 && echo "Verifying Jar file signature ..." && gpg --verify leiningen-$LEIN_VERSION-standalone.zip.asc && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar
# Fri, 07 Feb 2020 03:35:44 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 07 Feb 2020 03:35:44 GMT
ENV LEIN_ROOT=1
# Fri, 07 Feb 2020 03:35:53 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 07 Feb 2020 03:35:53 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:3192219afd04f93d90f0af7f89cb527d1af2a16975ea391ea8517c602ad6ddb6`  
		Last Modified: Sat, 01 Feb 2020 17:28:49 GMT  
		Size: 45.4 MB (45380658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c160265e75550c2ed099aa7d3906b3fef0bf046a2aeead136f8e587a015159`  
		Last Modified: Sun, 02 Feb 2020 00:42:04 GMT  
		Size: 10.8 MB (10797219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4fe40d0e618e3319afb689c3570bb87e8e8cf51bca080364d1552317bc66c2`  
		Last Modified: Sun, 02 Feb 2020 00:42:02 GMT  
		Size: 4.3 MB (4340216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d647f502a07e6daaee43c23cfac9399501b1d7f55fb4c60d56307e23f0ed5a5`  
		Last Modified: Sun, 02 Feb 2020 00:42:26 GMT  
		Size: 50.1 MB (50073989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d108b8c498aa300c0375abb3c74caebbf95e7ed768f49b1028fd6ace22e98051`  
		Last Modified: Sun, 02 Feb 2020 06:35:11 GMT  
		Size: 4.9 MB (4935305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9d47e6969884e68f4eed6bd69b77a2ffa118f0f558ec79dc5c38876635eb17`  
		Last Modified: Sun, 02 Feb 2020 06:35:09 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8600203e8c30381c9af3f9e048d74679a7017cfb73fa100613ecea6ff1e0ccb0`  
		Last Modified: Sun, 02 Feb 2020 06:35:31 GMT  
		Size: 196.1 MB (196085959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3e540cbe0c8ad6e20ab03c0d2b7064d417e18d282b748763f4b29677e7bbff`  
		Last Modified: Fri, 07 Feb 2020 03:39:21 GMT  
		Size: 13.1 MB (13139432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ae954aba4359118c87c1265c90673c448b143b24fd4a14c35bfdfc80ccddb9`  
		Last Modified: Fri, 07 Feb 2020 03:39:23 GMT  
		Size: 4.2 MB (4168273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-11` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8c0ae458fc6d1af35c34d88af9b2a62bd61ae1bcb80b6fa4de1261ca18919208
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320939931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750ec2864e8dd383a4ecb4ca2b269142694cc84c2933880a2192340cf45fe52c`
-	Default Command: `["lein","repl"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:01 GMT
ADD file:1618e6474dbe6462a610ce7eed99f0bfd087ea37ddfc287bbd69def5c24ede47 in / 
# Sat, 01 Feb 2020 16:43:02 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:29:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:29:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:30:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:35:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:35:11 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 21:35:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 01 Feb 2020 21:35:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 21:35:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 01 Feb 2020 21:35:15 GMT
ENV JAVA_VERSION=11.0.6
# Sat, 01 Feb 2020 21:35:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Sat, 01 Feb 2020 21:35:17 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Sat, 01 Feb 2020 21:35:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Sat, 01 Feb 2020 21:35:35 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 15:09:12 GMT
ENV LEIN_VERSION=2.9.1
# Sun, 02 Feb 2020 15:09:12 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 15:09:13 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 15:09:18 GMT
RUN mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha1sum lein-pkg && echo "93be2c23ab4ff2fc4fcf531d7510ca4069b8d24a *lein-pkg" | sha1sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver pool.sks-keyservers.net --recv-key 2B72BF956E23DE5E830D50F6002AF007D1A7CC18 && echo "Verifying Jar file signature ..." && gpg --verify leiningen-$LEIN_VERSION-standalone.zip.asc && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar
# Sun, 02 Feb 2020 15:09:18 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 15:09:19 GMT
ENV LEIN_ROOT=1
# Sun, 02 Feb 2020 15:09:34 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Sun, 02 Feb 2020 15:09:34 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:df3de44c7096ba135556a1e7044f9e1feee3ef713ab96f0416f71fe78422cbf6`  
		Last Modified: Sat, 01 Feb 2020 16:48:40 GMT  
		Size: 43.2 MB (43166749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf173a01baf7d45b479bb380ece219cbf0ea52178e9b8cdc5b87891759d1122`  
		Last Modified: Sat, 01 Feb 2020 17:39:19 GMT  
		Size: 9.7 MB (9748586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3392eac7bc27f3bd5fcb024413ca55ec4115c22da3e229567d5fc03cd4ff4e4`  
		Last Modified: Sat, 01 Feb 2020 17:39:18 GMT  
		Size: 4.1 MB (4094322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a82fc9ca296b095585ba7f3f6d83566428dbefcbfd284e242039aba97840b2`  
		Last Modified: Sat, 01 Feb 2020 17:39:40 GMT  
		Size: 48.0 MB (48024205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441917e764b91faf75f000df58cc6c02c3f7f238a28ff1a251e0f6ac479b0526`  
		Last Modified: Sat, 01 Feb 2020 21:38:40 GMT  
		Size: 4.8 MB (4843204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd602b7039207070a46906e27a11621bf674331f4117f23d12323b01104b4e`  
		Last Modified: Sat, 01 Feb 2020 21:38:37 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb5a36563911f461268a420dbd0fd7286f31606aa4e07fa5b3d31ec1ad4a8de`  
		Last Modified: Sat, 01 Feb 2020 21:39:06 GMT  
		Size: 193.8 MB (193754915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e9931d1416b87c5ad8a9fcc82233324db0ae8d74b5268a48893f1f98ed7ad0`  
		Last Modified: Sun, 02 Feb 2020 15:14:52 GMT  
		Size: 13.1 MB (13139430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d5d3949a4b33085660772f0e501dd08a347d8fef8daf1d7d76b568b02a4162`  
		Last Modified: Sun, 02 Feb 2020 15:14:51 GMT  
		Size: 4.2 MB (4168301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
