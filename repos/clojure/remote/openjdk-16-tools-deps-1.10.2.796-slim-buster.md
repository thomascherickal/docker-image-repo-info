## `clojure:openjdk-16-tools-deps-1.10.2.796-slim-buster`

```console
$ docker pull clojure@sha256:0b5b798a27b38be7f757f4db816f578381deeaac413a487bd448f4c30b7b1135
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-tools-deps-1.10.2.796-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:6eab687671e5ef7dd628489d2b0905b509ba0db884d9bb024f0a5a7bec2aad78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258109127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:596daa311019f91c45f210bba453b1d17976c0db8b28f2d9bc4ce5e59317ee37`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Mar 2021 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 20:59:55 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 09 Mar 2021 20:59:55 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:59:55 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 20:59:56 GMT
ENV JAVA_VERSION=16
# Tue, 09 Mar 2021 21:00:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 21:00:09 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:52:13 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Tue, 09 Mar 2021 21:52:13 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:52:29 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 09 Mar 2021 21:52:29 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:57ccab748b0184655ff89a7b21f0844c8635ebb7eaa0ac2c0d5e2fe441fc8c52`  
		Last Modified: Tue, 09 Mar 2021 21:14:52 GMT  
		Size: 185.2 MB (185153170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1e7bf3ffe09a674ef9130a619d42f258e73c53b0c1a8eb7e02a3768eb794e6`  
		Last Modified: Tue, 09 Mar 2021 22:08:04 GMT  
		Size: 42.6 MB (42592267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-tools-deps-1.10.2.796-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:505f085336b01ae11540e1047399881ed05927ec75f9c770e64af401d13530b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250601401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7edeb5bf7aa70c658d6d644e3916823abd7594fdf13872a51723d649ae66538d`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:37:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 12 Mar 2021 06:37:06 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:37:07 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:37:07 GMT
ENV JAVA_VERSION=16
# Fri, 12 Mar 2021 06:37:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:37:31 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 01:07:25 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Sat, 13 Mar 2021 01:07:27 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 01:08:15 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 13 Mar 2021 01:08:17 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:814158e9e12f222a40698e829a10f013b36cb5516d9873c5c28425841d14cd98`  
		Last Modified: Fri, 12 Mar 2021 06:47:01 GMT  
		Size: 179.5 MB (179529577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9096ca85ccd278d0b0596507cee96d4939bc02b9abcb855be51c78456d356cd`  
		Last Modified: Sat, 13 Mar 2021 01:20:01 GMT  
		Size: 42.1 MB (42096584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
