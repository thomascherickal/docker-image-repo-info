## `openjdk:22-slim-bookworm`

```console
$ docker pull openjdk@sha256:60d8c5576f157b3278b4e2dbf30514a98a9de65f5965813f09c6e01eccc1e231
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:22-slim-bookworm` - linux; amd64

```console
$ docker pull openjdk@sha256:b1c286226ca849e6d832f1f53df1b22811581b52e22e836f2211f9d5813f2c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235868522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578192cabd57afaff20c98fd08312c1904a22a0a34737a943f4ce61e5306be55`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:609b254ae3b337a0b4850ba592526bac580600c5dbb7057a0643e68bccc56aef`  
		Last Modified: Fri, 15 Dec 2023 22:05:35 GMT  
		Size: 3.8 MB (3821580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81a6a98df415360d0d231f79c87e9201984106fd951311b559b4aa494c7dc326`  
		Last Modified: Fri, 15 Dec 2023 22:05:38 GMT  
		Size: 202.9 MB (202897034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-slim-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:4b1d6ae83a62fd9a8290369886c74285a69fe68278f3b2225084063a7ee250d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2056450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d52e974528da5d0a93c42fd8251ef0e20e05e8227898415518b31980176e1d4f`

```dockerfile
```

-	Layers:
	-	`sha256:23988c789033d862b18c888d0d7c7ce3234ca7fa43d0d290d1a39907a6adeef6`  
		Last Modified: Fri, 15 Dec 2023 22:05:35 GMT  
		Size: 2.0 MB (2037107 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bae8f06cfe9590b444e4838fe072aef6515e9627ba527b991d63f73185066c84`  
		Last Modified: Fri, 15 Dec 2023 22:05:34 GMT  
		Size: 19.3 KB (19343 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:22-slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:670e351ef095744938fd02239bd699e69f76c95e113f6b50c5c3d78cfb38c111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.8 MB (233756018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2378845900e1f6ed1639a7bf60cb56fb7b76bd48f3aacd4f02c1799025c33225`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Fri, 08 Dec 2023 19:48:25 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 19:48:25 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 19:48:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 19:48:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 08 Dec 2023 19:48:25 GMT
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
	-	`sha256:4586b83fbeb777199fc4859d0be4ecef48fa932a9acec528fabf9423b9dc4911`  
		Last Modified: Fri, 15 Dec 2023 23:29:52 GMT  
		Size: 200.9 MB (200947119 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:22-slim-bookworm` - unknown; unknown

```console
$ docker pull openjdk@sha256:3090d652292e6e3ae0727acaeb227739867b3125014431ec74fd9c04cf95eb2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2055684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0571687ad4566774471b00f8ceb032710a3a86a8348a0a299f5f04773cb1d2`

```dockerfile
```

-	Layers:
	-	`sha256:c00100c80bda007e7fd23db17c2300a489c772d71b33018914df0e0cce2cc8b7`  
		Last Modified: Fri, 15 Dec 2023 23:29:47 GMT  
		Size: 2.0 MB (2036481 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f5f68da3ff7d6ab1152ed79004ea6bdbb39715c97f5d1ce31badd5eb3db5042`  
		Last Modified: Fri, 15 Dec 2023 23:29:47 GMT  
		Size: 19.2 KB (19203 bytes)  
		MIME: application/vnd.in-toto+json
