## `openjdk:15-ea-23-buster`

```console
$ docker pull openjdk@sha256:3f9473a4187faefd35f81ee1ba23b85b800ac87a1332a658efa5c31478b500ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-23-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:06ba88cc43af0164e4d21859bdbfe018bbbc735afe0f6f8dae20f90527f8cf3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.0 MB (326047558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a945122c3d95c303c806d06ba95c6b0e3e5f0167c45361134da9a3641b07cf9`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:32:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:32:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:59:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:59:27 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 20:59:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 15 May 2020 20:59:28 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 20:59:29 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 15 May 2020 20:59:29 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 15 May 2020 20:59:30 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz
# Fri, 15 May 2020 20:59:30 GMT
ENV JAVA_SHA256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0
# Fri, 15 May 2020 20:59:47 GMT
RUN set -eux; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 15 May 2020 20:59:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a63a0a859d859478f30461786a49c2fca3ae7d89ab5b5ce3c81c54951d30f88`  
		Last Modified: Fri, 15 May 2020 17:50:44 GMT  
		Size: 7.8 MB (7812354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496548a8c952b37bdf149ab3654f9085d721ee126b8c73b16860778be5137f5e`  
		Last Modified: Fri, 15 May 2020 17:50:49 GMT  
		Size: 10.0 MB (9996284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adae3950d4d0f11875568c325d3d542d1f2e2d9b49bdd740bb57fcfc1f6478f`  
		Last Modified: Fri, 15 May 2020 17:51:06 GMT  
		Size: 51.8 MB (51827083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e77013fe29f244314ba9ced8c62b5615de673a1413327ce0d5c27edc88e7363`  
		Last Modified: Fri, 15 May 2020 21:06:51 GMT  
		Size: 13.9 MB (13920351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09175c50f8ca7e1d2d7c355c4d7809418a0b9628196511e6b3ff00134f2fc`  
		Last Modified: Fri, 15 May 2020 21:06:49 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9c715f1ec89351adc43b6ed83092feb0fb7bbccf962bdf5e8f6b72726eb18`  
		Last Modified: Fri, 15 May 2020 21:07:07 GMT  
		Size: 192.1 MB (192099981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
