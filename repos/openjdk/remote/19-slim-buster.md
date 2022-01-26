## `openjdk:19-slim-buster`

```console
$ docker pull openjdk@sha256:449784662c87c96d4b3223da62a5eafbd331c4007002948d260b4434f4e96055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:eae03e2fae026e22d6baf22a8eb96e247a75f21d1b7aa8ef3b0b9fbd8bd9d865
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.4 MB (220413082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fbfcaaa6cefbd4cdb107feefb832bb1bc387813312ee139c2255b4c516029d`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:58:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 22:58:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Tue, 21 Dec 2021 22:58:36 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 22:58:36 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jan 2022 20:39:39 GMT
ENV JAVA_VERSION=19-ea+5
# Wed, 19 Jan 2022 20:39:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/5/GPL/openjdk-19-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='bb5a59a9573422be1df23754d298fce48e8d530e78af478756f219b2a8df34e1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/5/GPL/openjdk-19-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='27ef9cda6adaf16f8b57abfbdff8dbfef8a0ece62a0e47c0744f5e8dba8fb354'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 19 Jan 2022 20:40:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c983bcc370920d99695dc288c345343be841987206e4ce762a4e7599f28c96`  
		Last Modified: Tue, 21 Dec 2021 23:16:09 GMT  
		Size: 3.3 MB (3269567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9568406687e6b089ce1a100d0a1f450291d4f87a13a27d6335fffecfe3af682e`  
		Last Modified: Wed, 19 Jan 2022 20:53:50 GMT  
		Size: 190.0 MB (189989792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:4fe8ca1d6b0dac116e30bea2beb2f9f0891d42765cf17ad1ef423b6b3e727c49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.7 MB (217743241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee4dac4285cd5f97c8e854edfb20a863301368c62408f7198c206a10b552fa72`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:51:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:51:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 26 Jan 2022 05:51:03 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:51:04 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 05:51:05 GMT
ENV JAVA_VERSION=19-ea+5
# Wed, 26 Jan 2022 05:51:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/5/GPL/openjdk-19-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='bb5a59a9573422be1df23754d298fce48e8d530e78af478756f219b2a8df34e1'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/5/GPL/openjdk-19-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='27ef9cda6adaf16f8b57abfbdff8dbfef8a0ece62a0e47c0744f5e8dba8fb354'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 05:51:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a5c9716b24a17043a5d8ede1303daffeaaa07ff0393fa14caed54f01154833`  
		Last Modified: Wed, 26 Jan 2022 06:14:50 GMT  
		Size: 3.1 MB (3118858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c7bc2c4e5bb2fafaee35a7f30019784e8785dc68e41b3025af7f25d4a8ec`  
		Last Modified: Wed, 26 Jan 2022 06:15:09 GMT  
		Size: 188.7 MB (188701167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
