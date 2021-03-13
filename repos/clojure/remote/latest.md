## `clojure:latest`

```console
$ docker pull clojure@sha256:c1b229f7771be6b47d81c84236a8751165d0a5dcafda345f2c92d50c30934120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:latest` - linux; amd64

```console
$ docker pull clojure@sha256:9ef28f34c50ab38735025b44134e8a2d2d612ebd31ab764d0b5a800c3a05d339
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.0 MB (346993415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f8cacae444333bdcabb9ec545b458df6eac8e82c848762e73c52b6796a68f9`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Mar 2021 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 21:02:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 09 Mar 2021 21:03:00 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 09 Mar 2021 21:03:00 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 21:03:00 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 21:03:01 GMT
ENV JAVA_VERSION=11.0.10
# Tue, 09 Mar 2021 21:03:17 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 21:03:18 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:41:58 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 09 Mar 2021 21:41:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:41:58 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:42:04 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 09 Mar 2021 21:42:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:42:04 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 09 Mar 2021 21:42:44 GMT
RUN boot
# Tue, 09 Mar 2021 21:42:45 GMT
ENV LEIN_VERSION=2.9.5
# Tue, 09 Mar 2021 21:42:45 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:42:45 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:43:00 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 09 Mar 2021 21:43:00 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Tue, 09 Mar 2021 21:43:00 GMT
ENV LEIN_ROOT=1
# Tue, 09 Mar 2021 21:43:04 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Tue, 09 Mar 2021 21:43:04 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Tue, 09 Mar 2021 21:43:04 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:43:22 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 09 Mar 2021 21:43:22 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f1fbf102b7eaa0998133d35bbcc37641d4d23626a4a2673cb9a2393cb7c34c`  
		Last Modified: Tue, 09 Mar 2021 21:10:48 GMT  
		Size: 3.3 MB (3268548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1067f9902c49d08116077b996d56b7e092a3b61d723bb08811abb7752bbb438b`  
		Last Modified: Tue, 09 Mar 2021 21:21:09 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3872fd9937ea50005a439d84ab9df8abfe2a82ca1a0dedb9b3672a0c6f6bb4`  
		Last Modified: Tue, 09 Mar 2021 21:21:25 GMT  
		Size: 203.1 MB (203077648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2728544e5fd2be71a0fb15a78e3a6cefaf9f66f0058eeda0281f96c39a575a1`  
		Last Modified: Tue, 09 Mar 2021 21:57:48 GMT  
		Size: 282.8 KB (282796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26b859b53f0700c23a640ef83574b68dee088d27ef9cadcd52cf7d7aa06f847`  
		Last Modified: Tue, 09 Mar 2021 21:57:52 GMT  
		Size: 58.8 MB (58820913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d428222c14f983a9ea6a606bb06348aa89c04e5d9a05a2148a2df8a9ca2b79`  
		Last Modified: Tue, 09 Mar 2021 21:57:49 GMT  
		Size: 11.8 MB (11794517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ca4485c7b5eb33b0eeda2baa6746f1aa7fe7796262dc4a42ef8fcd2aa0f69e`  
		Last Modified: Tue, 09 Mar 2021 21:57:48 GMT  
		Size: 4.2 MB (4195526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8093b19e9dd96c8d436f0880c3813409bd375599cc0336426a710e37979526f`  
		Last Modified: Tue, 09 Mar 2021 21:57:54 GMT  
		Size: 38.5 MB (38458115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:latest` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e36e101f72715e5c3c4a1b3d562ee3c9c93ca3e1b8a95671d1b3801b2cf17714
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342697751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a06d6ce732f3f13a9e35026a70fdefc5ccde06fe795b4774151ae80aa492072`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:40:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 12 Mar 2021 06:40:25 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 06:40:26 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:40:26 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:40:27 GMT
ENV JAVA_VERSION=11.0.10
# Fri, 12 Mar 2021 06:41:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:41:05 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 00:51:03 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 13 Mar 2021 00:51:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 13 Mar 2021 00:51:06 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 00:51:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 13 Mar 2021 00:51:19 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 13 Mar 2021 00:51:20 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 13 Mar 2021 00:52:08 GMT
RUN boot
# Sat, 13 Mar 2021 00:52:10 GMT
ENV LEIN_VERSION=2.9.5
# Sat, 13 Mar 2021 00:52:11 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 13 Mar 2021 00:52:12 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 00:52:32 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Sat, 13 Mar 2021 00:52:33 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Sat, 13 Mar 2021 00:52:33 GMT
ENV LEIN_ROOT=1
# Sat, 13 Mar 2021 00:52:41 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Sat, 13 Mar 2021 00:52:42 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Sat, 13 Mar 2021 00:52:43 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 00:53:23 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 13 Mar 2021 00:53:25 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303a8d33f3a602102b6a15a1f7974fc79449cdcff2c2fa6709b56cd1ac792384`  
		Last Modified: Fri, 12 Mar 2021 06:45:08 GMT  
		Size: 3.1 MB (3118728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b66a2613c2e81c20d5f33497aaa0c185225f7b1a0fc1478b628ad5bce829`  
		Last Modified: Fri, 12 Mar 2021 06:49:58 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d8598ef43f9347e26595111cda32ecbffe0724879c8338f9bab599bcd05b64`  
		Last Modified: Fri, 12 Mar 2021 06:50:28 GMT  
		Size: 200.7 MB (200665723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0466266a0ecf88a599868287f31383ef75346b3595f8734dca96f35f46d56e34`  
		Last Modified: Sat, 13 Mar 2021 01:15:14 GMT  
		Size: 282.8 KB (282762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acac1efcb4f5559befbe1b37673d650d5695c50767cd28ba7f1633f8f03b9835`  
		Last Modified: Sat, 13 Mar 2021 01:15:22 GMT  
		Size: 58.8 MB (58820687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ecad3b910c1af16833f7faf8752f99e5ebe5c54af5ccd21a9e2ffc95349aa1`  
		Last Modified: Sat, 13 Mar 2021 01:15:15 GMT  
		Size: 11.8 MB (11794499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8edc206ff88eafd6d142d529ff79e55ea8691d3fae125f30c184203b52f6773e`  
		Last Modified: Sat, 13 Mar 2021 01:15:14 GMT  
		Size: 4.2 MB (4195555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e86597a3b1353d18e25c208d6cbbb700fd671c62cbf20e43ba5d51fdc5a22b0`  
		Last Modified: Sat, 13 Mar 2021 01:15:22 GMT  
		Size: 38.0 MB (37963074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
