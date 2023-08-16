## `openjdk:21-rc-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:da16b602cb42d22b10a01e68321e3a3545d5bd32af9e67f697c6576a71c0de68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-rc-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:45439237a578d894da991c841ded06023dbb010853d41b727ae390ff90120f74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237312971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2532607810b4235adff65dea88e7f3f8241f56a444079c1ef3f14753514b4a26`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 15:17:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:18:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 16 Aug 2023 15:18:23 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 15:18:23 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 15:18:23 GMT
ENV JAVA_VERSION=21
# Wed, 16 Aug 2023 15:18:36 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Aug 2023 15:18:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c001491d10985337074f3c26c09f771a339e441538d4bf8d9c02c011154869a`  
		Last Modified: Wed, 16 Aug 2023 15:21:23 GMT  
		Size: 1.6 MB (1582459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70104573bcfaaa5efcd9c4ad14f6638ad9899a1d136b279c9ac41c3299a5a3`  
		Last Modified: Wed, 16 Aug 2023 15:23:47 GMT  
		Size: 204.3 MB (204312834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-rc-jdk-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:a5f6b875e0ce726f6cd53a4df272e1872c412030424bc5abad46ed9d8642f255
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234282206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3758981ab104c8b44eaf5d1bb15510e62bc37bff3eac55f5578afd739060419f`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:13:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:14:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Wed, 16 Aug 2023 04:14:52 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 04:14:53 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 04:14:53 GMT
ENV JAVA_VERSION=21
# Wed, 16 Aug 2023 04:15:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Aug 2023 04:15:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e2c1addb652758859700ef04f06dd69f6d667824444c9f7dced516b2cec271`  
		Last Modified: Wed, 16 Aug 2023 04:17:43 GMT  
		Size: 1.6 MB (1566481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e355885008701dfd64c1641414c9ac65462ff8597612f04b6b8f56bfd98f04f3`  
		Last Modified: Wed, 16 Aug 2023 04:19:48 GMT  
		Size: 202.7 MB (202652909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
