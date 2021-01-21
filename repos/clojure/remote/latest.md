## `clojure:latest`

```console
$ docker pull clojure@sha256:3220f36f5eed32c909d482fe5d2f15e241bd5ab3d5f608e786246dd8eb4f9931
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:latest` - linux; amd64

```console
$ docker pull clojure@sha256:743d582f2d0228dfc7cda9544a09d429f48157ea1cad6ec76c28386b97097300
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.1 MB (341053909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c0697ca713343e5fccb8ff19e0173f651b7ac3ba2e383196607f6b58d3d9a1`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:53:01 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 10:58:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 12 Jan 2021 10:58:17 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 10:58:18 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 21 Jan 2021 02:38:27 GMT
ENV JAVA_VERSION=11.0.10
# Thu, 21 Jan 2021 02:38:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Jan 2021 02:38:53 GMT
CMD ["jshell"]
# Thu, 21 Jan 2021 03:47:43 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 21 Jan 2021 03:47:43 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 21 Jan 2021 03:47:43 GMT
WORKDIR /tmp
# Thu, 21 Jan 2021 03:47:49 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 21 Jan 2021 03:47:50 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 21 Jan 2021 03:47:50 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 21 Jan 2021 03:48:12 GMT
RUN boot
# Thu, 21 Jan 2021 03:48:13 GMT
ENV LEIN_VERSION=2.9.5
# Thu, 21 Jan 2021 03:48:13 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 21 Jan 2021 03:48:13 GMT
WORKDIR /tmp
# Thu, 21 Jan 2021 03:48:23 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 21 Jan 2021 03:48:24 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Thu, 21 Jan 2021 03:48:24 GMT
ENV LEIN_ROOT=1
# Thu, 21 Jan 2021 03:48:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 21 Jan 2021 03:48:29 GMT
ENV CLOJURE_VERSION=1.10.1.763
# Thu, 21 Jan 2021 03:48:29 GMT
WORKDIR /tmp
# Thu, 21 Jan 2021 03:48:50 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "91421551872d421915c4a598741aefcc6749d3f4aafca9c08f271958e5456e2c *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 21 Jan 2021 03:48:50 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d8acaac04a2b66af03bcc85abe1cd3f50e06d7e193634e04d4e55c4fc7cc8`  
		Last Modified: Tue, 12 Jan 2021 11:07:22 GMT  
		Size: 3.2 MB (3248558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9998d19c11696925915d7583990a0b9e239265533655abc5376d117ec9cfe3c`  
		Last Modified: Tue, 12 Jan 2021 11:14:44 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba5b958e0416b8e5d7b2ae81a51f33cfba67f5d9ea139a5ffd099b8956dfdec`  
		Last Modified: Thu, 21 Jan 2021 02:48:35 GMT  
		Size: 197.2 MB (197200421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a9419348cdcd3d4fc08523237ebfecec27cd43ceddebf04878891e2d8c76e`  
		Last Modified: Thu, 21 Jan 2021 03:56:22 GMT  
		Size: 282.7 KB (282740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb8388b0bd7c4b2abc89efa906b4e4b39a92d3389f26de470243195e01bf00d`  
		Last Modified: Thu, 21 Jan 2021 03:56:24 GMT  
		Size: 58.8 MB (58820310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c76b927bc9d06da29ce5745ef0146be658ccc76c4928960067021d127526032`  
		Last Modified: Thu, 21 Jan 2021 03:56:22 GMT  
		Size: 11.8 MB (11794529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d35ed3c7aeab21568347b6b34f6274f4b31391fcc02e5359a58da11f9ce82`  
		Last Modified: Thu, 21 Jan 2021 03:56:20 GMT  
		Size: 4.2 MB (4168795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594d92a139ee97fc7e5bf924f7314a8d3c3a95f2cf06991b805e797244e0b89d`  
		Last Modified: Thu, 21 Jan 2021 03:56:36 GMT  
		Size: 38.4 MB (38430276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:latest` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4e3e146a2a5f461dcb8ff98ceb84b3791b1f174ad7cc121667b3f09732e65215
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336689163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8154b7b05c1001e069894d5769263a8266476fb3a186200a6cedba79fa906dd1`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:00:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:00:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 01:06:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 12 Jan 2021 01:06:06 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 01:06:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 12 Jan 2021 01:06:09 GMT
ENV JAVA_VERSION=11.0.9.1
# Tue, 12 Jan 2021 01:06:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.9.1_1.tar.gz ;; 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.9.1_1.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 12 Jan 2021 01:06:41 GMT
CMD ["jshell"]
# Tue, 12 Jan 2021 19:11:00 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 12 Jan 2021 19:11:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 12 Jan 2021 19:11:01 GMT
WORKDIR /tmp
# Tue, 12 Jan 2021 19:11:12 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 12 Jan 2021 19:11:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 12 Jan 2021 19:11:13 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 12 Jan 2021 19:11:55 GMT
RUN boot
# Tue, 12 Jan 2021 19:11:56 GMT
ENV LEIN_VERSION=2.9.5
# Tue, 12 Jan 2021 19:11:57 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 12 Jan 2021 19:11:58 GMT
WORKDIR /tmp
# Tue, 12 Jan 2021 19:12:19 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 12 Jan 2021 19:12:19 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Tue, 12 Jan 2021 19:12:20 GMT
ENV LEIN_ROOT=1
# Tue, 12 Jan 2021 19:12:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 12 Jan 2021 19:12:29 GMT
ENV CLOJURE_VERSION=1.10.1.763
# Tue, 12 Jan 2021 19:12:30 GMT
WORKDIR /tmp
# Tue, 12 Jan 2021 19:13:04 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "91421551872d421915c4a598741aefcc6749d3f4aafca9c08f271958e5456e2c *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 12 Jan 2021 19:13:06 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6132c56bf059fe6b3844038ac4ca6b320af5f511b4c60addc956fb470ebfcb8`  
		Last Modified: Tue, 12 Jan 2021 01:11:08 GMT  
		Size: 3.1 MB (3101516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839eacc19004a1bca74e60f9d365055748827163da406bac39dc158ac65c6e8d`  
		Last Modified: Tue, 12 Jan 2021 01:16:43 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b6eaf8c50bf4d7470394c121a96f3d953876437f07625fd94f661a0985a33`  
		Last Modified: Tue, 12 Jan 2021 01:17:11 GMT  
		Size: 194.7 MB (194719025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ef9fe60fb4fd65d446ff513c839f10a781e0a519b99b1e67de231b692abe35`  
		Last Modified: Tue, 12 Jan 2021 19:27:15 GMT  
		Size: 282.6 KB (282566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3149bce01f5895e7e1c27ade875d34ac7483f772ab267d2213f7b179c6d7d3`  
		Last Modified: Tue, 12 Jan 2021 19:27:21 GMT  
		Size: 58.8 MB (58820657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a196548fa07906b8b3978a5907299e65acded40efe42df28fc97da7817fb9a9`  
		Last Modified: Tue, 12 Jan 2021 19:27:17 GMT  
		Size: 11.8 MB (11794425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c81df4268de9f325cfa7620c8304ba50af57628fb20354cee2b7bb3718e85`  
		Last Modified: Tue, 12 Jan 2021 19:27:15 GMT  
		Size: 4.2 MB (4168895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddf8fbe2f68c9ab6832896bf447e2153adb73bb8bd095ea5d1c07aab1a07d7`  
		Last Modified: Tue, 12 Jan 2021 19:27:26 GMT  
		Size: 37.9 MB (37937376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
