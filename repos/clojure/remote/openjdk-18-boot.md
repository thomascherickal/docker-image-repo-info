## `clojure:openjdk-18-boot`

```console
$ docker pull clojure@sha256:8461ada6b73a900158421af7d73c5838d4a8a8b05e52e195dc887022e90243ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-boot` - linux; amd64

```console
$ docker pull clojure@sha256:41b9d38b9c6fe856413b21051b73dea057e17b26a52a7b4abc6f96d8571b6cb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.3 MB (280334795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:808ef4cc14ba10f195e476a2fe97984de388152424cb81945f56902eef7bf1fb`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:27:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 12 Oct 2021 16:27:47 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:27:47 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 00:25:57 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:26:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:26:12 GMT
CMD ["jshell"]
# Sat, 16 Oct 2021 01:29:32 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 16 Oct 2021 01:29:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 16 Oct 2021 01:29:33 GMT
WORKDIR /tmp
# Sat, 16 Oct 2021 01:29:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 16 Oct 2021 01:29:37 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 16 Oct 2021 01:29:38 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 16 Oct 2021 01:30:08 GMT
RUN boot
# Sat, 16 Oct 2021 01:30:08 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225be9814eda07dabebf0e4deb415366f34b2cfe12ef1ad167ba1104423f42d7`  
		Last Modified: Tue, 12 Oct 2021 16:42:59 GMT  
		Size: 1.6 MB (1582043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ade8c50d0feafc1d676c9c58fc742b1d6a2efab9a73200c21ba415f0a9f9cad`  
		Last Modified: Sat, 16 Oct 2021 00:34:24 GMT  
		Size: 188.3 MB (188291675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a903e75981a7a6f040fdea138fa203665201f68348343107d94db1d6a3b92`  
		Last Modified: Sat, 16 Oct 2021 01:37:28 GMT  
		Size: 283.1 KB (283091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed49fa4af64cece29be019d39ef211727d1b11ab07313b53e8facca85d3280f`  
		Last Modified: Sat, 16 Oct 2021 01:37:31 GMT  
		Size: 58.8 MB (58820675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-boot` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d7e3d9de8ba34f22d693301df10292bab90098b3d1418f01678b0e2a058c8ede
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.5 MB (277488678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e7d0c21648cbc2becb7291acbae5effe5de5f1b9726adbb858d1b841a804da`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 06:00:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:00:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Wed, 13 Oct 2021 06:00:54 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:00:55 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 00:06:23 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:06:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='42b5b8f65bed00be3fa810f876581eb1cd5eebcfe44dae0361e9f4128ec905cd'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/19/GPL/openjdk-18-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='518af06c8ba2d135a7ba43a937f1ed061e7d6acf55dc296cef60b1fd50413438'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 16 Oct 2021 00:06:39 GMT
CMD ["jshell"]
# Sat, 16 Oct 2021 00:47:29 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 16 Oct 2021 00:47:30 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 16 Oct 2021 00:47:31 GMT
WORKDIR /tmp
# Sat, 16 Oct 2021 00:47:36 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 16 Oct 2021 00:47:36 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 16 Oct 2021 00:47:37 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 16 Oct 2021 00:47:52 GMT
RUN boot
# Sat, 16 Oct 2021 00:47:52 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:a9eb63951c1c2ee8efcc12b696928fee3741a2d4eae76f2da3e161a5d90548bf`  
		Last Modified: Tue, 12 Oct 2021 01:48:13 GMT  
		Size: 30.0 MB (30043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552e0d309d6deaf17b87f395ca03a5bb0b4c14128cd49208ab21c34bf39e933`  
		Last Modified: Wed, 13 Oct 2021 06:25:32 GMT  
		Size: 1.6 MB (1565908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3b2d8d6832e44becf1d2716fdf898488e6ad21e93b670a7da9ce428ce3d550`  
		Last Modified: Sat, 16 Oct 2021 00:20:22 GMT  
		Size: 187.0 MB (186995759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5c36d0d1ccf63479554f6fcd0afa262ead4881321bdfbc452f1ef8fecbea7a`  
		Last Modified: Sat, 16 Oct 2021 00:58:21 GMT  
		Size: 67.2 KB (67227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10aa0c8a771bc287162b53f9f5fc1079b6820b823ebf1c67d7f464c9403b3bd3`  
		Last Modified: Sat, 16 Oct 2021 00:58:26 GMT  
		Size: 58.8 MB (58815878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
