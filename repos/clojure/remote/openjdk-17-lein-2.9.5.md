## `clojure:openjdk-17-lein-2.9.5`

```console
$ docker pull clojure@sha256:e6ad83098d53f50bc36aab5c5d3a2fb0cf04f7ca960fb62a4c62e27e3221d08c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-lein-2.9.5` - linux; amd64

```console
$ docker pull clojure@sha256:5858b912b237cdfe5ac8c726cd22a58eb76f8bb4ff50f55f9434886811de33e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.3 MB (232334817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd66040d23dc34542bda23f29fbed36d83d3e9421be427a65c180d2af8961da7`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 22:10:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:10:14 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 12 Mar 2021 22:10:14 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:10:14 GMT
ENV LANG=C.UTF-8
# Fri, 19 Mar 2021 18:24:55 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 19 Mar 2021 18:25:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='d4bfd596e0b4f3eefb416719a5b6ad98ab3f37f27855573e7c94526a4ffad7d2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='16646d2498690f98b44f196e74da8361ef05155038a04cb6f62fbb76df08e72f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 19 Mar 2021 18:25:09 GMT
CMD ["jshell"]
# Fri, 19 Mar 2021 18:56:43 GMT
ENV LEIN_VERSION=2.9.5
# Fri, 19 Mar 2021 18:56:44 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 19 Mar 2021 18:56:44 GMT
WORKDIR /tmp
# Fri, 19 Mar 2021 18:56:54 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 19 Mar 2021 18:56:54 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 19 Mar 2021 18:56:54 GMT
ENV LEIN_ROOT=1
# Fri, 19 Mar 2021 18:56:58 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 19 Mar 2021 18:56:58 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3555c3885852c38ecf4a297b798053677bc7553f9c7631788ef75e35cb4262c`  
		Last Modified: Fri, 12 Mar 2021 22:22:18 GMT  
		Size: 3.3 MB (3268564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6eadd7ea0ff10503878ecdef0efce1c90dd3b260372701bf5cfd9c6b8f9585`  
		Last Modified: Fri, 19 Mar 2021 18:31:55 GMT  
		Size: 186.0 MB (185963195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c210b01f176d501df2c8b756cfe0c9b87c377deccb0a6c0e187656c553b441b7`  
		Last Modified: Fri, 19 Mar 2021 19:07:52 GMT  
		Size: 11.8 MB (11798340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af02b633dc9048c542a8a168bcf3c4e903aa9e868431a4998d10428d21dbf49a`  
		Last Modified: Fri, 19 Mar 2021 19:07:52 GMT  
		Size: 4.2 MB (4203717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-lein-2.9.5` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:76c336778f4e76eb54db7784177eaac271cf217151ffec13ffdb14f9b840052e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.0 MB (227024046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333319a909771be91a882a3bbe3a8807d345cf0830a4e3abaff45aaff6fa1a98`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:34:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Fri, 12 Mar 2021 06:34:55 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:34:56 GMT
ENV LANG=C.UTF-8
# Fri, 19 Mar 2021 19:02:22 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 19 Mar 2021 19:03:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='d4bfd596e0b4f3eefb416719a5b6ad98ab3f37f27855573e7c94526a4ffad7d2'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/14/GPL/openjdk-17-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='16646d2498690f98b44f196e74da8361ef05155038a04cb6f62fbb76df08e72f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 19 Mar 2021 19:03:22 GMT
CMD ["jshell"]
# Fri, 19 Mar 2021 19:33:55 GMT
ENV LEIN_VERSION=2.9.5
# Fri, 19 Mar 2021 19:33:56 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 19 Mar 2021 19:33:57 GMT
WORKDIR /tmp
# Fri, 19 Mar 2021 19:34:15 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 19 Mar 2021 19:34:16 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 19 Mar 2021 19:34:17 GMT
ENV LEIN_ROOT=1
# Fri, 19 Mar 2021 19:34:23 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 19 Mar 2021 19:34:24 GMT
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
	-	`sha256:451a9a2c802cfd9bb256d5e308fe44167a411566ff01525d361bf27a05965184`  
		Last Modified: Fri, 19 Mar 2021 19:09:22 GMT  
		Size: 182.0 MB (182046831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb92fb8b598bfa256f1f544140495de59445ec53059252272ddb914184df3d7f`  
		Last Modified: Fri, 19 Mar 2021 19:39:42 GMT  
		Size: 11.8 MB (11798250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eaada4072031d713ef3ddf374fa0ddf5555360d3ea7692f0711497dcfb13ca0`  
		Last Modified: Fri, 19 Mar 2021 19:39:41 GMT  
		Size: 4.2 MB (4203725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
