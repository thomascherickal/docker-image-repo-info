## `clojure:latest`

```console
$ docker pull clojure@sha256:1afe2347b8e35737e288eadb758500dc4cb5378b5f6c370a8b422bc22697a6e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:latest` - linux; amd64

```console
$ docker pull clojure@sha256:16550a3ec093f8a0620674f2654799f4dd501574d96f1f2b3b0995d1e627c728
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.1 MB (351104119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:544ea93b59fb2d2b1ffcd5b88f955e9c3510aae27046ff8d0d61b018ee9f0fde`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:57:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:00:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 21 Dec 2021 23:00:50 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:00:50 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:00:50 GMT
ENV JAVA_VERSION=17.0.1
# Tue, 21 Dec 2021 23:01:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 21 Dec 2021 23:01:06 GMT
CMD ["jshell"]
# Wed, 22 Dec 2021 13:31:21 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 22 Dec 2021 13:31:22 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 22 Dec 2021 13:31:22 GMT
WORKDIR /tmp
# Wed, 22 Dec 2021 13:31:27 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 22 Dec 2021 13:31:27 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 22 Dec 2021 13:31:27 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 22 Dec 2021 13:31:58 GMT
RUN boot
# Wed, 22 Dec 2021 13:31:58 GMT
ENV LEIN_VERSION=2.9.8
# Wed, 22 Dec 2021 13:31:58 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 22 Dec 2021 13:31:58 GMT
WORKDIR /tmp
# Wed, 22 Dec 2021 13:32:10 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 22 Dec 2021 13:32:11 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Wed, 22 Dec 2021 13:32:11 GMT
ENV LEIN_ROOT=1
# Wed, 22 Dec 2021 13:32:14 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 07 Jan 2022 20:19:52 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:19:52 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:20:12 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 07 Jan 2022 20:20:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:20:13 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:20:13 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:20:13 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbde5250315969db657b55bd8b2f5507fb659c0cf7f135edc84b684ffeab44a`  
		Last Modified: Tue, 21 Dec 2021 23:14:38 GMT  
		Size: 1.6 MB (1582039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1343f138b677c0b1457cc7cb6310108df5388665281e0962273fb3492e52b86d`  
		Last Modified: Tue, 21 Dec 2021 23:20:46 GMT  
		Size: 187.5 MB (187548781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28528d53cd48fd4902450e5a6df1e9cf6352532e7cd2eb44748f464b73d51c29`  
		Last Modified: Wed, 22 Dec 2021 13:54:21 GMT  
		Size: 283.1 KB (283093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c60331fc2e0262247e7f20db3fef64a123f39656ef505e97c558d09ab18c15`  
		Last Modified: Wed, 22 Dec 2021 13:54:24 GMT  
		Size: 58.8 MB (58820811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f21bec1a8d5dac6fdcde087ef6d25395218e01412e75a3f0072afb923e884b`  
		Last Modified: Wed, 22 Dec 2021 13:54:19 GMT  
		Size: 11.9 MB (11861574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1506b73bfd11494bff1910c32cd6846ea99c20820bc1d8684134b46ddb3f4a57`  
		Last Modified: Wed, 22 Dec 2021 13:54:19 GMT  
		Size: 4.2 MB (4207321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae541a0b7a7e8d808081ecc6df60b2365e0c91ed7d8a929a5104bfdeb3f843c8`  
		Last Modified: Fri, 07 Jan 2022 20:29:24 GMT  
		Size: 55.4 MB (55441847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d938a48f9db01f16219005dff64ffcf78bb9d98ff7e89cd6a8e857da2444781`  
		Last Modified: Fri, 07 Jan 2022 20:29:17 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8b0fa1759762aca7b46d7f32fc560bba26f56f70f0a0b2c7a874db1a9f3ef4`  
		Last Modified: Fri, 07 Jan 2022 20:29:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:latest` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a9bd2f84c56b6e8e0d7fa151637c149b8082885f53e8b913490bdd2640bff25e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.9 MB (347851165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ad11ea4116cd3af02de7aeddaa372165166987bc3e56ae6c37a95a6e79dfbe`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:53:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 21 Dec 2021 02:57:57 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:57:58 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 02:57:59 GMT
ENV JAVA_VERSION=17.0.1
# Tue, 21 Dec 2021 02:58:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 21 Dec 2021 02:58:14 GMT
CMD ["jshell"]
# Tue, 21 Dec 2021 22:01:26 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 21 Dec 2021 22:01:26 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 21 Dec 2021 22:01:27 GMT
WORKDIR /tmp
# Tue, 21 Dec 2021 22:01:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 21 Dec 2021 22:01:33 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 21 Dec 2021 22:01:34 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 21 Dec 2021 22:02:09 GMT
RUN boot
# Tue, 21 Dec 2021 22:02:10 GMT
ENV LEIN_VERSION=2.9.8
# Tue, 21 Dec 2021 22:02:11 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 21 Dec 2021 22:02:12 GMT
WORKDIR /tmp
# Tue, 21 Dec 2021 22:02:23 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 21 Dec 2021 22:02:23 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Tue, 21 Dec 2021 22:02:24 GMT
ENV LEIN_ROOT=1
# Tue, 21 Dec 2021 22:02:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 07 Jan 2022 20:40:01 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:40:01 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:40:18 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 07 Jan 2022 20:40:19 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:40:20 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:40:20 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:40:21 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3380d13c6c3ddd0cc31ece5496ad1481500cb07b7feb31c81bc907a9a1ad71`  
		Last Modified: Tue, 21 Dec 2021 03:15:59 GMT  
		Size: 1.6 MB (1565954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793a64b0fc1713036909cd54095428181b63814fde3deff4542fa3a1ff57dbdc`  
		Last Modified: Tue, 21 Dec 2021 03:23:05 GMT  
		Size: 186.1 MB (186138689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fd5a291a086a9eccf608f17d05be998a9d528795592aae4d43e50c55b5555b`  
		Last Modified: Tue, 21 Dec 2021 22:28:37 GMT  
		Size: 67.2 KB (67235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a338b34162e195ba665fdbfc3c8ca1723b40f608a30e840bc9cb3451ad203e`  
		Last Modified: Tue, 21 Dec 2021 22:28:47 GMT  
		Size: 58.8 MB (58816700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d77bbdaae40c75aab3e8f38b487dd813c716806428088780e4002b5f9802ab9`  
		Last Modified: Tue, 21 Dec 2021 22:28:36 GMT  
		Size: 11.6 MB (11645522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c1fc9770dbb6b314e543fec8f994236dc7375bc7af6de92379d2583ff12e32`  
		Last Modified: Tue, 21 Dec 2021 22:28:37 GMT  
		Size: 4.2 MB (4207099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3491d8e0aa03d8159d6b0a228fa6b5fdbfb1c54e29a89c09b72c1121d59467f6`  
		Last Modified: Fri, 07 Jan 2022 20:54:31 GMT  
		Size: 55.4 MB (55365140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f082864d6aeb5c10352dae16ee6cc67f1dd97430766a4dc188a19dc6286817`  
		Last Modified: Fri, 07 Jan 2022 20:54:22 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ed1d2b9827de71d0619c846f8cf9263fd0b27c65c5da8e7fe91badf5f16c85`  
		Last Modified: Fri, 07 Jan 2022 20:54:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
