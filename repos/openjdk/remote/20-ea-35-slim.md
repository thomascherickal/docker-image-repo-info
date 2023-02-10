## `openjdk:20-ea-35-slim`

```console
$ docker pull openjdk@sha256:300de15fa4d2e50ab158b61b624d4b0a16baeff1b8870f6d8895cb0266a8945e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:20-ea-35-slim` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ca044361821bf1fbd325de9f713d2b99779c94129e7794235e46e87e2cc12247
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228636718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8caa85c6dfa1f67b932624ba715d9078231f592fce43773a6cf098aba7026582`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:07:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:09:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Thu, 09 Feb 2023 10:09:20 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:09:21 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 01:58:51 GMT
ENV JAVA_VERSION=20-ea+35
# Fri, 10 Feb 2023 01:59:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/35/GPL/openjdk-20-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='2062453caf72cff8ad296b84d90108f2eb057d7415a5c7d109672fd6b613ef1f'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/35/GPL/openjdk-20-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='65541ed26e56fe91b7d3ba703bde269e5568313e3e7168d2476455f03f460eda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Feb 2023 01:59:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12ec23d1569af13aa4b739730163609a2c012fc5a8c00a55e2c980462802868`  
		Last Modified: Thu, 09 Feb 2023 10:14:41 GMT  
		Size: 1.6 MB (1566302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41fa463c476be035f562edcab87e1d507135e8df018b25a4597e500c0fba90f`  
		Last Modified: Fri, 10 Feb 2023 02:08:11 GMT  
		Size: 197.0 MB (197007907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
