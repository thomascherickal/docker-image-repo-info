## `openjdk:23-jdk-slim-bookworm`

```console
$ docker pull openjdk@sha256:da9f37d75b9783e0b218110513866e4ca78a636c6345dd851a9447a7b0c40925
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:23-jdk-slim-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:0eff86c978795f6de05f17c50ae3d726283e4aedb0a8f4ffcba97f027e8f54b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235939824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a6d4a7315a390e272fcb3eb502f1f5d993b34c7d3a4ca109799f8f7aaac5a0`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/local/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c260fc1a4c34ded39da5754700919961bed5a00c9404989a7c9e3dd90a0905b`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 3.8 MB (3821591 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe9a5372467d3bf96d5680fa16c54038e7fd6320f566c0be6bcd1339f3ab573e`  
		Last Modified: Fri, 15 Dec 2023 22:05:58 GMT  
		Size: 203.0 MB (202968325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-slim-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:e71b92f07989616e6d41ebdad963fd6b63d0863e2575605af705cc9697beb4db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2056418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2bfcbadbf9eae1238e2cf1aefb094ab64f61fceca20e9d1af8eca67a9c42d95`

```dockerfile
```

-	Layers:
	-	`sha256:6d7a25170b6012b916240899e1b623f21b6c378e104aec9bc1703fe8570b8531`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 2.0 MB (2037091 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b75b3e9d889f3b5a145774d56cfa03ddee5dfc11cdc5f32d9e888e3b363a7236`  
		Last Modified: Fri, 15 Dec 2023 22:05:53 GMT  
		Size: 19.3 KB (19327 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-jdk-slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:34c060fb04047835c6b499e9b435a9518e08d91f67d395eaa306ef1968e2e116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233825706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca947126bf5f2906b7c5c11506633a3c12252402e1a9ef4be8050da1874509d`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-23
# Sat, 09 Dec 2023 18:45:21 GMT
ENV PATH=/usr/local/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 18:45:21 GMT
ENV LANG=C.UTF-8
# Sat, 09 Dec 2023 18:45:21 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 09 Dec 2023 18:45:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='740a84253d35402b9213bf187ee4f058817c614f8cc47cb3414e02760f05099f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='74fe7c8e67c5b80f868ec20daecb112fc090fb91c58bf4ce5297cf77c9935fa5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Sat, 09 Dec 2023 18:45:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:268bfd66b4e399c51afc9123b085a775b9a4a6eb628f71a7bd2f2955bf9a9f65`  
		Last Modified: Fri, 15 Dec 2023 23:23:20 GMT  
		Size: 3.6 MB (3629622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5bbc4680fec83ccc814859af4ef3aa9d6b8439792e3be34ed0a9ddc815990b66`  
		Last Modified: Fri, 15 Dec 2023 23:23:24 GMT  
		Size: 201.0 MB (201016807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-slim-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:4debc47ad8921143993ce29c73931c4b95c19872dbc589b1f4b6f3147dfbd361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2055659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5615208df5d65682fa46275419a4ccff1c0dadbcbd47371b4dffae84bb50cd`

```dockerfile
```

-	Layers:
	-	`sha256:e3531d7982782b4946907fcc8e880b892fbc6a6b5691a7fff23fde75d2aad939`  
		Last Modified: Fri, 15 Dec 2023 23:23:20 GMT  
		Size: 2.0 MB (2036473 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8b66f7f0c686340e70f327614ca7780169c461d8fcf41c1c30531a26a89e3cf5`  
		Last Modified: Fri, 15 Dec 2023 23:23:19 GMT  
		Size: 19.2 KB (19186 bytes)  
		MIME: application/vnd.in-toto+json
