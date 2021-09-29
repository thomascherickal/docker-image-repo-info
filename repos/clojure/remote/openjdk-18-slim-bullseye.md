## `clojure:openjdk-18-slim-bullseye`

```console
$ docker pull clojure@sha256:9cbe52a206eae2e92a25460d37774b6856eb787e5504d6b7e1644e605ed4e7fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:a5fb92c0465d493cf7624511d1ad353953167e2dbc54dfbde486e701b7d56afb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236776992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9855a637d0d508c2bb27f580aa653694d3ed43eda1e26cc49c88e2554ee1d7c2`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:31:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:31:20 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:31:20 GMT
ENV LANG=C.UTF-8
# Tue, 14 Sep 2021 01:32:25 GMT
ENV JAVA_VERSION=18-ea+14
# Tue, 14 Sep 2021 01:32:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='6aee5779ac7488dbd6988658662ca683704ac98cee6b8dde8df3ddffac76142e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/14/GPL/openjdk-18-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='88a106afe903b8f5d552ceae108294d8b36cbc0656a744f84525ccae542c5029'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Sep 2021 01:32:38 GMT
CMD ["jshell"]
# Tue, 14 Sep 2021 02:16:43 GMT
ENV LEIN_VERSION=2.9.6
# Tue, 14 Sep 2021 02:16:43 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 14 Sep 2021 02:16:44 GMT
WORKDIR /tmp
# Tue, 14 Sep 2021 02:16:59 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 14 Sep 2021 02:16:59 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 14 Sep 2021 02:16:59 GMT
ENV LEIN_ROOT=1
# Tue, 14 Sep 2021 02:17:02 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Tue, 14 Sep 2021 02:17:03 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ae0b0c4c13e1ebacfd091b8e226cc8aa92df8937632e3bec2b03a877bf2d87`  
		Last Modified: Fri, 03 Sep 2021 08:49:03 GMT  
		Size: 1.6 MB (1582002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a929f978fca4736906d5ab1ce1ee62551d0d835be57cf6d3d422bc7e9deae159`  
		Last Modified: Tue, 14 Sep 2021 01:40:58 GMT  
		Size: 187.8 MB (187822547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba12dfaa287113e005cfd2ccd9488b3400aee8532f2ea2e5ab4bec9eaa98c1c`  
		Last Modified: Tue, 14 Sep 2021 02:25:39 GMT  
		Size: 11.8 MB (11800012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00950b74ba08cb5335e8d88aa3614fad02be9e1156ce9d8a1be5a5ba2df1030a`  
		Last Modified: Tue, 14 Sep 2021 02:25:39 GMT  
		Size: 4.2 MB (4203729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8d00716fa530b8bd21c163b277a2ad30f7b4e39c04e4c5fc9139c82c4125ae7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234705202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab771e33529f7ab9da4cf1c1379a5e074fe881c3bf09354910d7dd7c161b700`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:42:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:42:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 28 Sep 2021 05:42:51 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:42:51 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:42:51 GMT
ENV JAVA_VERSION=18-ea+16
# Tue, 28 Sep 2021 05:43:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:43:04 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:31:30 GMT
ENV LEIN_VERSION=2.9.7
# Wed, 29 Sep 2021 02:31:30 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 29 Sep 2021 02:31:31 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:31:41 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "f78f20d1931f028270e77bc0f0c00a5a0efa4ecb7a5676304a34ae4f469e281d *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -r "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 29 Sep 2021 02:31:41 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 02:31:41 GMT
ENV LEIN_ROOT=1
# Wed, 29 Sep 2021 02:31:45 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 29 Sep 2021 02:31:45 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc69e286af9edc8fb3518a0692316edc953730d4b65004457f37972b70873fe1`  
		Last Modified: Tue, 28 Sep 2021 06:04:25 GMT  
		Size: 1.6 MB (1566191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48028112f2af20bfa2863589ad5231ced228799108fbbc4460280a1d3a0bb1`  
		Last Modified: Tue, 28 Sep 2021 06:04:43 GMT  
		Size: 187.0 MB (187015722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a356467b3cdd8dd6b2e0579146df09376ec2cde264b1ab53eb2e455890d960`  
		Last Modified: Wed, 29 Sep 2021 02:56:19 GMT  
		Size: 11.9 MB (11860673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f11c6518a22063776a99b8d4fb8ea31492f694a14d3be90515ff773e888dac9`  
		Last Modified: Wed, 29 Sep 2021 02:56:19 GMT  
		Size: 4.2 MB (4207208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
