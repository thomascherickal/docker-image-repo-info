## `openjdk:22-ea-27-bookworm`

```console
$ docker pull openjdk@sha256:3b4b9ab46014a2cf17a3594785faa508556f57590601a6cc28a15c3936ba1610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:22-ea-27-bookworm` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1c2ca379d6cda974616cfe40f474b42788c0c0597c3cf4b2036be5384bd77a19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.8 MB (355821745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a513013101b3614ae94d96713cc5f0419dfa2caace5867c42ee35554f182dc86`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:57:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:29:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:29:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-22
# Tue, 21 Nov 2023 10:29:23 GMT
ENV PATH=/usr/local/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:29:23 GMT
ENV LANG=C.UTF-8
# Fri, 08 Dec 2023 23:24:09 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 08 Dec 2023 23:24:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='102a2e0fa1174ba6e67f79685a98122609d7f3106f3745f7418a5224e55e8643'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='39341b5dba8789f64a9f1dd7310ede993d890a44ecde059955992c3260e82b78'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 08 Dec 2023 23:24:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdd9a70365f741a6b9f7a4e32cdb7d4aa29ac73da0b78ca0a83e937f285fdd5`  
		Last Modified: Tue, 21 Nov 2023 08:06:19 GMT  
		Size: 64.0 MB (63994275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb3b49b5f442227c66e95ff2e626b9a41b4c0f512bf33e32179c1f8ad50973a`  
		Last Modified: Tue, 21 Nov 2023 10:31:08 GMT  
		Size: 17.7 MB (17733389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b054ffc4e1f6d3297f559119fbde42d8288f035a1c6398b541cd3327e0a8afc6`  
		Last Modified: Fri, 08 Dec 2023 23:27:03 GMT  
		Size: 200.9 MB (200896555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
