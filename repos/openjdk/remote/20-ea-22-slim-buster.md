## `openjdk:20-ea-22-slim-buster`

```console
$ docker pull openjdk@sha256:ff3396fd56b4e55749366338a0f365738716b5bef6a204295fe3ea8214f4fad8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-22-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:a56c3b9d381e2a0189dc9f2a1c2a132f7f5c6fb13832fa34e2de641d3fc5981c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229051730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e46d95b7c91037242398543dd15d3e3bc4d81e1289c9d1e029391a1ae8e318`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:29:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:29:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Tue, 25 Oct 2022 04:29:04 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 04:29:04 GMT
ENV LANG=C.UTF-8
# Mon, 07 Nov 2022 22:25:30 GMT
ENV JAVA_VERSION=20-ea+22
# Mon, 07 Nov 2022 22:25:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/22/GPL/openjdk-20-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='00d072b351777213b5d37223fbfa7fafc5232f339c4aaac2f60de584753ae1b3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/22/GPL/openjdk-20-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='b2f24beafa225a8591d09e4b5f2d907d136915fae9158c298a8abb5746be5de5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 07 Nov 2022 22:25:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04045c4766379cb0b4fc93bb96707506245d8d2e952cc00e74925a3994f6ec34`  
		Last Modified: Tue, 25 Oct 2022 04:33:18 GMT  
		Size: 3.3 MB (3275908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d5d7a2a53718e6f42eb511ba99ab24e7def33447d903a6ba6df66188c4bcc5`  
		Last Modified: Mon, 07 Nov 2022 22:31:45 GMT  
		Size: 198.6 MB (198634990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-22-slim-buster` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:397cfe84e1bb5586c8ee088ca8e97157569555cce529af60caa44442dc0d309f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226252706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ceb2fa6fd709ed3304b5407bf98e97a05102ea8e36fe6532188903d03663e2`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:13 GMT
ADD file:342233874a06722375663380e7e3a04502a995dfbbc425cd1913f10e96a50dcb in / 
# Tue, 25 Oct 2022 05:46:14 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 00:45:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 00:45:37 GMT
ENV JAVA_HOME=/usr/local/openjdk-20
# Wed, 26 Oct 2022 00:45:37 GMT
ENV PATH=/usr/local/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:45:37 GMT
ENV LANG=C.UTF-8
# Mon, 07 Nov 2022 22:30:09 GMT
ENV JAVA_VERSION=20-ea+22
# Mon, 07 Nov 2022 22:30:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/22/GPL/openjdk-20-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='00d072b351777213b5d37223fbfa7fafc5232f339c4aaac2f60de584753ae1b3'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/22/GPL/openjdk-20-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='b2f24beafa225a8591d09e4b5f2d907d136915fae9158c298a8abb5746be5de5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 07 Nov 2022 22:30:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f30c56efde95016859c51bdc10e665dd57dc3c8d22e7abbf384ae9722dfa19e`  
		Last Modified: Tue, 25 Oct 2022 05:49:47 GMT  
		Size: 25.9 MB (25914885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13616a3846ecd154918e95271126bfcebd73bd0090135c17f7836596878e708`  
		Last Modified: Wed, 26 Oct 2022 00:53:01 GMT  
		Size: 3.1 MB (3129308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9778385dc3e40b84a73346a3873242e45d92cd6edf526ed13a6e4a70f62658`  
		Last Modified: Mon, 07 Nov 2022 22:36:17 GMT  
		Size: 197.2 MB (197208513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
