## `openjdk:21-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:8881504edce861eaa9261b44a3f004cdf5a5552325ec0009b153b0ff9999f318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:e468ffd5af3a402b222dcaa85c200d7f0d3d19f91a121f7a4eeab6d22b454e9b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.8 MB (234796098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93192c5283aa44a252b78a9d236afb35ba47d92250c10e15e949dbda31a5a492`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:38:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:38:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 09:38:20 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 09:38:20 GMT
ENV LANG=C.UTF-8
# Sat, 15 Apr 2023 00:30:59 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:31:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:31:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3ccfec852f335c3077cc27f9d826129c3799986d9e3b44f40f5df7a5a28b1c`  
		Last Modified: Wed, 12 Apr 2023 09:40:23 GMT  
		Size: 1.6 MB (1582448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d6a656d37d10edbdb7c7209052ad2a28e18b220401a893f8fb516ae5fec96d`  
		Last Modified: Sat, 15 Apr 2023 00:34:05 GMT  
		Size: 201.8 MB (201795422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2a6fad159e76777f91aa639e353f8e1a31b318d6b63ce420da54188759c8ab7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.8 MB (231780795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a93e4359d0be8dbead702e0cd8bb8c2b9c8b43c9f954c9a5e14626c7a09d2be`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:11:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:11:00 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 12 Apr 2023 05:11:00 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 05:11:00 GMT
ENV LANG=C.UTF-8
# Sat, 15 Apr 2023 00:56:14 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:56:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:56:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742e1b6db7553fd2059cce2c9672c6a73a94022701f01b4dd3569d492ec71a7`  
		Last Modified: Wed, 12 Apr 2023 05:13:00 GMT  
		Size: 1.6 MB (1566462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027e95b78f445ef33b6c1625ea23f48fbcd7070cfb4339d640cbe347fa1cdca9`  
		Last Modified: Sat, 15 Apr 2023 00:59:08 GMT  
		Size: 200.2 MB (200150507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
