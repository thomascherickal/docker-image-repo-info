## `clojure:openjdk-11-tools-deps-1.10.3.1075-bullseye`

```console
$ docker pull clojure@sha256:30c310f45fb62287426e4ab510ba730e6d0eab32bc67a03a8073eac84ad806a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-11-tools-deps-1.10.3.1075-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e1c85ab0dd43402874caffeb53195b7877925d02ba9254706d67e205205fe875
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.0 MB (357016932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05f233b95c04ef9d426280b0160f33261cfb478cf8eee71f07aa85f40b87003`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:34:14 GMT
ENV JAVA_VERSION=11.0.14
# Thu, 03 Feb 2022 20:35:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_linux_11.0.14_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.14_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Feb 2022 20:35:40 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 23:50:29 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 23:50:29 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 23:50:38 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 04 Feb 2022 23:50:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 23:50:39 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda090e7df3523dc9db18e06c2619b52e4dd2772c2800105e421552c27e599ed`  
		Last Modified: Thu, 03 Feb 2022 20:58:14 GMT  
		Size: 203.3 MB (203272575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afa1fd35702a33375cb4c6fb0360454b276bfdd0d6a6165bb6adfadc5dfe199`  
		Last Modified: Sat, 05 Feb 2022 01:41:08 GMT  
		Size: 22.8 MB (22814381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3553c8d0f3435938f693ba23502f95b26a83ae5b65ef5fd1de75b9c349f6751`  
		Last Modified: Sat, 05 Feb 2022 01:41:06 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-11-tools-deps-1.10.3.1075-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e13135a689210b29153c8b75508c4885571aa179b8ffb51a6b0169edf080645e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (352956619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a72b76c38c46f259fef4d13a3819c4424c9e4d191217b3cdd1bc5581a796cc67`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:49:24 GMT
ENV JAVA_VERSION=11.0.14
# Thu, 03 Feb 2022 20:50:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_linux_11.0.14_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.14_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Feb 2022 20:50:21 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 21:47:03 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 21:47:04 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 21:47:12 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 04 Feb 2022 21:47:14 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 21:47:14 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094aec66c6a7d824fad2b23976909d7a80fb1306908ad7fdfa38bded6f5d2f8b`  
		Last Modified: Thu, 03 Feb 2022 21:12:31 GMT  
		Size: 200.9 MB (200886679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027e0938a52621bdfd111af8529e3cb96c8b17f1da9b3dd328913ba5999cc676`  
		Last Modified: Fri, 04 Feb 2022 21:59:31 GMT  
		Size: 22.6 MB (22573144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961ea6dd080a8d28f93e10826842580979425162d74d1e4e3a2fe1efc3b9ea1`  
		Last Modified: Fri, 04 Feb 2022 21:59:29 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
