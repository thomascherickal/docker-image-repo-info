## `clojure:openjdk-16-boot-slim-buster`

```console
$ docker pull clojure@sha256:32a91ef84bd4db61a399a8809bcf242ba78bbefb397cf5a9d1ff7c140fda8101
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:023961fc423558253e289ea91d1e3971422fa023eb3c6c1a58aa2dfa367b134b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274705032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044b5afe108eb076791ebbd1a5beea5ee6b7206f1df9fc602304c5b223e31d0c`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:32:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:36:05 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 03 Sep 2021 08:36:06 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:36:06 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:36:06 GMT
ENV JAVA_VERSION=16.0.2
# Fri, 03 Sep 2021 08:36:22 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Sep 2021 08:36:23 GMT
CMD ["jshell"]
# Sat, 04 Sep 2021 10:00:10 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 04 Sep 2021 10:00:11 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 04 Sep 2021 10:00:11 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 10:00:15 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 04 Sep 2021 10:00:16 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Sep 2021 10:00:16 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 04 Sep 2021 10:00:35 GMT
RUN boot
# Sat, 04 Sep 2021 10:00:35 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb538b78785f115f86e312f41ac522a9b30e0cb77d061dd273f331e57ae2e471`  
		Last Modified: Fri, 03 Sep 2021 08:50:36 GMT  
		Size: 3.3 MB (3269611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39ea5a0b4177449167d2431a9775ae5f25ef5d99bd187377966ef9cc7b773e7`  
		Last Modified: Fri, 03 Sep 2021 08:56:42 GMT  
		Size: 185.2 MB (185189574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37230d5e3d50438ade5e89a63f2ecdacae8a3608922350d80b2f7084f347fed1`  
		Last Modified: Sat, 04 Sep 2021 10:12:57 GMT  
		Size: 279.7 KB (279705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c324e1d821e0db9c43ece900f78f61e1e0ac133a796f2b9ea35f3ad78a4f817`  
		Last Modified: Sat, 04 Sep 2021 10:13:02 GMT  
		Size: 58.8 MB (58820298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-boot-slim-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:084f4c616d7c858ea46a1bcbd2bcecb01b3e72d255c9a49dce87d94bfcf239f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.7 MB (267698964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69339e89effb7c8edc502d8e64e7cd90dbda95c7e10a386f40bca7290b78c95b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 05:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:46:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 28 Sep 2021 05:46:52 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 05:46:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 05:46:53 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 28 Sep 2021 05:47:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 05:47:05 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 02:16:27 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 29 Sep 2021 02:16:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 29 Sep 2021 02:16:27 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 02:16:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 29 Sep 2021 02:16:33 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 02:16:33 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 29 Sep 2021 02:16:57 GMT
RUN boot
# Wed, 29 Sep 2021 02:16:57 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f844c3c3d3fdf0c62ff77a82ed24a2a010ad55e3206255c75275457b868825`  
		Last Modified: Tue, 28 Sep 2021 06:06:17 GMT  
		Size: 3.1 MB (3119080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4986d60774827f7e5dffc6bcae3725843438f1a695ef557e50d27c30919a9ad`  
		Last Modified: Tue, 28 Sep 2021 06:12:34 GMT  
		Size: 179.6 MB (179564666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642a1d5a69ffe1d98c6aaa6b08264d4a9eb457d86dac8e382dcad7873e573ea6`  
		Last Modified: Wed, 29 Sep 2021 02:45:01 GMT  
		Size: 279.6 KB (279578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37a04d27d7f9fda370bf09cd657d0a969735ed301a78cb1592b89006e306bcf`  
		Last Modified: Wed, 29 Sep 2021 02:45:05 GMT  
		Size: 58.8 MB (58820601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
