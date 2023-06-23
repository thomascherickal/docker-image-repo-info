## `openjdk:21-ea-28-jdk-slim-bullseye`

```console
$ docker pull openjdk@sha256:69ee88a986a64e8a3a6a316ab5e9e89a1e5d7ff301309df64b88fd2e3de6b390
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-ea-28-jdk-slim-bullseye` - linux; amd64

```console
$ docker pull openjdk@sha256:9e6853df99c6b9935f4f3787aa4c312263861eb82f77f8007db6e3bc458fbf5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237230712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233b77cfb71b8e98fd41afc7257b9bca52f7521f9e00c86656cc22d1810fb13a`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:19:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:20:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 07:20:50 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:20:50 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 00:28:43 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 00:28:56 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c5ff4dc462286ead4a7f1480719f695a976a130005df30d33ba210aadc094ff9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='4f98a729913be1d28fda8491420394e394fbbf84c4d1f41f05b83ba4c8b989aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:28:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454a143e8504247dc2e9e60b33533bee1b7a6ce927b0222b0354c9ab465ce3bf`  
		Last Modified: Tue, 13 Jun 2023 07:22:50 GMT  
		Size: 1.6 MB (1582441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994e99cd8880530f7c9d73fe54502d1032ef6ac3254477a4ea920935423975dc`  
		Last Modified: Fri, 23 Jun 2023 00:36:28 GMT  
		Size: 204.2 MB (204230861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
