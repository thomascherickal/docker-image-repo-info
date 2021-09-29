## `clojure:openjdk-18-tools-deps-slim-bullseye`

```console
$ docker pull clojure@sha256:70e3df5e87ea2675950a642d24f79ff4ff9b93fea2c15d73d1be1e03a1a5dd0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:682b08dba3605d8a0bd253e3f66603558a38728da54d5d77253316ca3a917c00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.0 MB (277994558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42c6a54696df73c68fc1807318e51235ab699741dc0a043c67b662ca5f57e68`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Sat, 25 Sep 2021 00:25:42 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:25:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-x64_bin.tar.gz'; 			downloadSha256='ec604f7aef23624c0acdc0db346a2b226aab47d120538833070f0d5e01d571c1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_linux-aarch64_bin.tar.gz'; 			downloadSha256='623eff3e61bd5f74442fb5699ac3dea167dbe0ade7dd6c1fa9cdd4788e316b96'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 25 Sep 2021 00:25:56 GMT
CMD ["jshell"]
# Sat, 25 Sep 2021 01:22:58 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Sat, 25 Sep 2021 01:22:58 GMT
WORKDIR /tmp
# Sat, 25 Sep 2021 01:23:15 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 25 Sep 2021 01:23:16 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:90416dc6dd4ab7f0222694d32e64bba4e610c0cd0dcf2227cc3631e39d4f3ea0`  
		Last Modified: Sat, 25 Sep 2021 00:34:30 GMT  
		Size: 188.3 MB (188279789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2634f1e510222fc7d85baa3e7de189c44148d272035da58c8a49226884bbe56`  
		Last Modified: Sat, 25 Sep 2021 01:29:17 GMT  
		Size: 56.8 MB (56764065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4476ad4119a8c37b5a753bc7b04b6e5c0a21d0e12ba75965fb1c6ca208a07e30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275533430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22fc95ccd74a593dbe60f6e5cdf54d19ad01049528b2964507c633ddb15eb2f`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Wed, 29 Sep 2021 02:33:12 GMT
ENV CLOJURE_VERSION=1.10.3.967
# Wed, 29 Sep 2021 02:33:13 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:33:28 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d1fba0cd0733b7cb66e47620845ecedfd757a9bf84e8b276fdb37ed9c272d3ae *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 29 Sep 2021 02:33:28 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:907678355b0fa304724ef84dae539239045aeb44ad5319e3711fc52c585a1403`  
		Last Modified: Wed, 29 Sep 2021 02:57:44 GMT  
		Size: 56.9 MB (56896109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
