## `openjdk:22-jdk-slim`

```console
$ docker pull openjdk@sha256:84a7a632e5ea1f709c7b976f3ff1119128eafae64067731c4674bc4b6a0561fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-jdk-slim` - linux; amd64

```console
$ docker pull openjdk@sha256:1f44e508fe22f84f1308799a0f9ea41517d04d6d0e818039136b93ab73f1b3be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.7 MB (238699431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d0b29d4a4d9e0b7c46e0242df385a468ac38c8072c238459c1f40bd1a86262`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:20:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 21 Nov 2023 09:20:39 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 09:20:39 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 20:55:39 GMT
ENV JAVA_VERSION=22-ea+26
# Fri, 01 Dec 2023 20:55:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='65f135f44a1f33848f9d8398b7773807cf90eeec08d6ec8e2a9b44d81b7b6d99'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/26/GPL/openjdk-22-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='3933a8d405ab7f0293ecd4351177e731f1eacd1a96ee3f0528b9157940581ce2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 01 Dec 2023 20:55:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a71988e474766aa4283c8ac4ac023b8d3b00c2e51d23a0740e109345192d40`  
		Last Modified: Tue, 21 Nov 2023 09:21:54 GMT  
		Size: 4.0 MB (4017900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba4cb2255b8d021f67925fe99adb4e249b06895d6b8560c91c3aada64d107f5`  
		Last Modified: Fri, 01 Dec 2023 20:58:59 GMT  
		Size: 205.5 MB (205531623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-jdk-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:511c01d41096a689a65ee5b27f6f0e33cd6a91ad7274eb4098ad2d517d379da3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234157693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf06a21de5d8f2518b9d20a5b171e0285f9ec11c5aee36fab333fe6ba855142b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:29:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:29:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 21 Nov 2023 10:29:42 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:29:42 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 23:24:25 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 23:24:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 08 Dec 2023 23:24:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938abad0ae32738292038fe26fab14358cf3b2ff43939c996a3562737bae4956`  
		Last Modified: Tue, 21 Nov 2023 10:31:36 GMT  
		Size: 3.8 MB (3824739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6aa6ec090fcb6599a708afc1ccf97b1dfa6b9f5b89c5ed54f72a06920eb7b1`  
		Last Modified: Fri, 08 Dec 2023 23:27:38 GMT  
		Size: 201.2 MB (201153677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
